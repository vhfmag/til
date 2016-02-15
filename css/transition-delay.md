# How transition delay works

I know that should be pretty obvious, but FML.
When using CSS's transition-delay, the value set inside the resultant class is used, not the departing one. It's so that:
>  .before-anim {
>    width: 100px;
>    transition-delay: 200ms;
>  }
>  
>  .after-anim {
>    width: 0px;
>    transition-delay: 0ms;
>  }

Will have no delay at when reducing the width, but will have it when growing.
