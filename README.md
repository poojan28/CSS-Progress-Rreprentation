# CSS-Progress-Rreprentation
![CSS-Progress](https://github.com/poojan28/CSS-Progress-Rreprentation/blob/master/css-progress.JPG)
# scss

    .box{
        width:100%;
        position: relative;
        display:flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        height:400px;
        border-radius: 0.5rem;
        background:#fff;
        box-shadow: 0 15px 65px rgba($color: #000000, $alpha: 0.2);

        .percent{
           width:150px;
           height: 150px;
           position: relative;
           svg{
               circle{
                   width:100%;
                   height:100%;
                   fill:none;
                   stroke-width: 10;
                   stroke:#000;
                   transform: translate(5px, 5px);
                   stroke-dasharray:440;
                   stroke-dashoffset: 440;
                   &:first-child{
                    stroke-dasharray:0;
                       stroke:#f3f3f3;
                   }
                   &:last-child{
                    
                       stroke:#03a9f4;
                   }
               }
           }
           .number{
               position: absolute;
               top:0;
               left:0;
               width:100%;
               height:100%;
               display:flex;
               align-items: center;
               justify-content: center;
               color:#999;
               h2{
                   font-size:48px;
                   span{
                       font-size:24px;
                   }
               }
           }

        }
        .text{
            color:#999;
            font-size: 24px;
        }
    }
