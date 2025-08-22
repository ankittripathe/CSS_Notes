/ Notes:
\*{
margin:0;
padding:0;
box-sizing:border-box;
}

div{
height: 100px;
width:100px;
padding:20px;
border:5px solid black;
}

Agar universal me(_) box-sizing: border-box kr diya toh.
Given Height, width me padding margin adjust hoga. Maan lo Box ka height=100px & width=100px hai to padding and border usi 100px me adjust hoga.
_/

       display: inline/ block / inline-block / none;
        inline = Takes only the space required by the elements.(no margin/ padding)
        block = Takes full space available in width.
        inline-block = Similar to inline but we can set margin & padding
        none = To remove elemets from document flow


        /* margin-left: 10%; */
        font-size: 0.5em;  /* half of parents's size */
        /* font-size: 2em;    2 times of parents's size 2*30= 60px   */
        /* width me font size of itself dekha jaega na ki parent ka (font size of child se multiply ho jaega. here breakdown font-size = 2em = double of its parent 2*30 = 60px,
        60px* 10em= 600 px
        */
        width: 10em;
        /* parent ke font size se pahle child wala font-size multiply hoga phir child wale font size se width wala multiply hoga */

Topic: rem(root em) => relative to font size of the root elements(root means HTML)

In short: Relative shifts visually, but reserves its old space in the layout.

<!-- *********************************** -->
Box4 is relative → keeps its old space in the flow.
→ That’s why content below it adjusts downward.

Box5 is absolute → doesn’t affect siblings.
→ It’s only “floating” inside Box4, so its position doesn’t disturb other boxes.

So the real “pushing” effect is because of Box4 (relative positioning), not Box5.