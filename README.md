# Angular13docs

String Interpolation 
>> String interpolation is binding of a data inside curely bases.
ex.
<p>{{allowNewUser}}</p>

******************************************************************************************************* 
Property Binding 
>> Property Binding is a one-way data-binding technique. In property binding, we bind a property of a DOM element to a field which is a defined property in our component TypeScript code. Actually, Angular internally converts string interpolation into property binding.

Syntax:

<element [property]= 'typescript_property'>

--------------------------------------------------------------------------------------------------

app.component.html

<input style = "color:green;
                margin-top: 40px; 
                margin-left: 100px;" 
[value]='title'>
--------------------------------------------------------------------------------------------------
app.component.ts

import { Component } from '@angular/core';    
@Component({    
  selector: 'app-root',    
  templateUrl: './app.component.html',    
  styleUrls: ['./app.component.css']    
})    
export class AppComponent {   
  title = 'GeeksforGeeks'; 
}



*********************************************************************************************
Event Binding
Definition:
In Angular 8, event binding is used to handle the events raised by the user actions like button click, mouse movement, keystrokes, etc. When the DOM event happens at an element(e.g. click, keydown, keyup), it calls the specified method in the particular component.

import { Component } from '@angular/core';    
@Component({    
  selector: 'app-root',    
  templateUrl: './app.component.html',    
  styleUrls: ['./app.component.css']    
})    
export class AppComponent {    
  gfg(event) {
    console.log(event.toElement.value);
  }    
}

Syntax :
< element (event) = function() >
Example:
<h1>
  GeeksforGeeks
</h1>
<input (click)="gfg($event)" value="Geeks">
*********************************************************************************************


