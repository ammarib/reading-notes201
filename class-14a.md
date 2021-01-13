# Transitions and animations     
An evolution of CSS3 has been the ability to define behavior for transitions and animations.     
Front-end developers have been asking for years to implement these interactions within HTML and CSS,     
without using JavaScript or Flash. Now their dream has come true.     
     
          

With CSS3 transitions, you have the potential to change the appearance and behavior of an element whenever     
its state changes, such as when an element is hovered over, it gains focus, becomes active, or the element is navigated through a link.     
     
          

Animation in CSS3 allows you to change the appearance and behavior of an element using multiple keyframes.     
Transitions provide a transition from one state to another, while an animation can set multiple transition points through different keyframes.     
     
          
          

## Transitions   
As mentioned, for a transition to take place, an element must receive a state change, and different styles must be defined for each state.     
The easiest way to style different states is to use the: hover,: focus,: active, and: target pseudo-classes.     



There are four properties associated with transitions in general, transition-property, transition-duration, transition-timing-function, and transition-delay.     
Not all of them are required to create a transition, the first three are the most popular.

In the example below, the block will change its background color within one second in a linear fashion.     

> .square {     
>   background: # 2db34a;      
>   transition-property: background;     
>   transition-duration: 1s;     
>   transition-timing-function: linear;     
> }     
> .square: hover {     
>   background: # ff7b29;      
> }        




## Animation    
Transitions do a great job of creating visual interactions from one state to another and are ideal for these kinds of single state changes.    
However,when more control is required, multiple states are needed for transitions. From this point on, transitions go away, and animation comes into play.     

### Animation keyframes
To set multiple points at which an element should transition, use the @keyframes rule.     
This rule includes the name of the animation, any number of breakpoints, and the properties for the animation.       

> @keyframe slide {  
  0% {  
    left: 0;  
    top: 0;  
  }  
  50% {  
    left: 244px;  
    top: 100px;  
  }  
  100% {  
    left: 488px;  
    top: 0;  
  }  
}        



The animation above is called slide, the states start immediately after opening the @keyframes rule.  
The different breakpoints of keyframes are set using percentages, starting at 0% and working up to 100%,  
with an intermediate point of 50%. If desired, the from and to keywords can be used instead of 0% and 100%.  
In addition to 50%, additional control points can also be specified. The properties of the elements to animate  
are listed inside each control point, left and top in the above example.

