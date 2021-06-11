

import React from 'react';
import ReactDOM from 'react-dom';
import Sdata , {ro ,me ,ne ,ke ,de } from "./Sdata";
import "./index.css"



 let Card = (props) => 
     <div className="cards">
      <div className="card">

        <img src={props.imgsrc} alt="no pic" className="card_image" />
          <div className="card_info">
            <span className="card_category">{props.team}</span>
            <h3 className="card_title">{props.player}</h3>
            <a href={props.link} target="blank">
              <button>More Pics</button>
            </a>
            </div>
         </div>
       </div>
      

ReactDOM.render(
  <>
<h1 className="heading_style" >TOP 5 footballers</h1>
  
    <Card imgsrc={ro}  team="Juventus" player="RONALDO" link="https://www.pinterest.com/pin/774056254699619866/"  />
    <Card imgsrc={de}  team="Juventus" player="DYBALA" link="https://www.google.com/search?source=univ&tbm=isch&q=dybala+hd+pics&sa=X&ved=2ahUKEwjLtMGbzI_xAhVTILcAHeZLCeUQjJkEegQIBxAC"  />
    <Card imgsrc={me}  team="Barcelona FC" player="MESSI" link="https://www.pinterest.com/search/pins/?rs=ac&len=2&q=messi%20wallpaper%20full%20hd%204k&eq=messi&etslf=6896&term_meta[]=messi%7Cautocomplete%7C2&term_meta[]=wallpaper%7Cautocomplete%7C2&term_meta[]=full%7Cautocomplete%7C2&term_meta[]=hd%7Cautocomplete%7C2&term_meta[]=4k%7Cautocomplete%7C2" />
    <Card imgsrc={ne}  team="PSG" player="NEYMAR" link="https://www.pinterest.com/search/pins/?q=neymar%20pics&rs=typed&term_meta[]=neymar%7Ctyped&term_meta[]=pics%7Ctyped" />
    <Card imgsrc={ke} team="Manchester City"  player="KEVIN DE BRYUYNE" link="https://www.pinterest.com/search/pins/?q=kevin%20de%20bruyne%20pics&rs=typed&term_meta[]=kevin%7Ctyped&term_meta[]=de%7Ctyped&term_meta[]=bruyne%7Ctyped&term_meta[]=pics%7Ctyped" />
  

  </>  
    
          , document.getElementById("root")
          );
