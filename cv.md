# Olga Furs
![foto](./foto-resume.jpg)
## Contact Info
- **Phone:   +375 (29) 346-75-65**
- **Email:     olga.mhl.furs@gmail.com**
           - **olga.m.furs@mail.ru**
- **Skype:    olga.m.furs.**
- **Linkedin: https://www.linkedin.com/in/olgafurs/**

## Objective
Front-end Developer (Junior)

## Summary
Work on the result, teamwork, attentiveness, responsibility, determination, high learning, the desire for development, goodwill.

## Skills 

-	Layout of web pages based on the hypertext markup language of web pages (HTML), cascading style sheet (CSS);
-	Knowledge and work with the CSS-based SASS preprocessor and with the GULP task manager;
-	Web page layout using Flexbox technology, Grid Layout;
-	Writing media queries to create an adaptive version of sites (web pages);
-	Experience using the Bootstrap 4 framework;
-	Skills and experience in the multifunctional graphic editor Adobe Photoshop 2018, a web service for hosting GitHub IT projects;
-	Basic knowledge of the concept of developing web applications MVC (Model-View-Controller).
-	Development of web applications in JavaScript (certificate of IT-academy)
-	Microsoft Visual Studio 2019;
-	Microsoft SQL Server.

**English Proficiency**: Pre-Intermediate (I read technical literature, conduct business correspondence, can briefly communicate on some topics).

## Code Examples

```JavaScript

"use strict";

import React from 'react';
import ReactDOM from 'react-dom';
import RainbowFrameParentHOC   from './components/RainbowFrameParentHOC';

ReactDOM.render( 
  <RainbowFrameParentHOC  />, document.getElementById('container')
);

```

```JavaScript
import React from 'react';
import {Fragment} from 'react';
import './RainbowFrameParentHOC.css';
import DoubleButton from './DoubleButton';
import {withRainbowFrame} from './withRainbowFrame';

class RainbowFrameParentHOC  extends React.Component {  

  render() {
     let colors = ['#ff0000','#ffa500', '#ffff00','#66ff00', '#00BFFF', '#0000ff', '#800080']; 
     let FramedDoubleButton=withRainbowFrame(colors)(DoubleButton);
    return (
     <Fragment>
       <DoubleButton caption1="однажды" caption2="пору" cbPressed={ num => alert(num) } >в студёную зимнюю</DoubleButton>
       <FramedDoubleButton caption1="я из лесу" caption2="мороз" cbPressed={ num => alert(num) }>вышел, был сильный</FramedDoubleButton>
     </Fragment>
    );       
  }
}

export default RainbowFrameParentHOC;
```

```JavaScript
import React from 'react';
import PropTypes from 'prop-types';
import './DoubleButton.css';

class DoubleButton  extends React.Component {  
  
  static propTypes = { 
    caption1: PropTypes.string.isRequired,
    caption2: PropTypes.string.isRequired,
    cbPressed: PropTypes.func.isRequired,
  }; 
  
  clickCaption1 = (EO) => {
    this.props.cbPressed(EO.target.value);
  }
  
  clickCaption2 = (EO) => {
    this.props.cbPressed(EO.target.value);
  }

  render() {          
      return (
        <div className="DoubleButton">
          <input type="button" value={this.props.caption1} onClick={this.clickCaption1}/>
          {this.props.children}        
          <input type="button" value={this.props.caption2} onClick={this.clickCaption2}/> 
        </div>     
      );       
  }
}


export default DoubleButton;
```

```JavaScript
import React from 'react';

function withRainbowFrame(color) {
    return function(Comp) {       
        return props => {                
            let code = <Comp {...props} />;
            color.forEach(col => 
                code=<div style={{border: "solid 7px" + col, padding:"10px"}}>{code}</div> 
            );
            return code;
        }       
    }
}

export { withRainbowFrame };
```

## Education 
**April 2020 – July 2020 – Educational Center for Programming and High Tech**<br/>
*Course*: React and Angular web application development<br/>
*Description*: 
- React events, component state, npm.
- Project dependency management, project build, JSX.
- Component life cycle, rendering optimization.
- Routing, testing, Fetch API.
- The architectural pattern of Redux. TypeScript.
- Angular, input and output properties, class and style management. Channels, directives, services.
- Development of directives, RxJS, routing, testing.

**November 2019 – March 2020 – Educational Center for Programming and High Tech**<br/>
*Course*: JavaScript web application development<br/>
*Description*: 
- Introduction Functions Arrays and hashes
- Short circuits. OOP. Class Description
- Built-in classes. Work with the DOM. Debugging and testing Event code. Event handling
- Event object. Mouse, keyboard, touchscreen, drag & drop events
- Event handling delegation. Debugging, code testing. SVG Canvas. Timers. Animation. Animation Performance
- Render tree. Hardware acceleration of animations. Animation Canvas Seamless animation. Rendering methods
- Multimedia. JSON Data storage on the client. MVC AJAX. SPA (Single Page Application)
- Modularity. Cross-browser compatibility. Regular expressions

**August 2019 – October 2019 – Educational Center for Programming and High Tech**<br/>
*Course*: Website development using HTML, CSS and JavaScript<br/>
*Description*:
- Introduction to HTML. References
- Images. CSS introduction
- Fonts Borders. Dimensions
- Indentation. Background. Tables
- Flow around. Layout layouts. Selectors
- Hierarchical selectors. Cascading. Display and Visibility
- Media queries. Adaptive layout
- Forms. HTML5
- Multimedia. CSS3 Animation. Flex Grid

**April 2018 – October 2019 – Belarusian State University of Informatics and Radioelectronics**<br/>
Specialization: Institute of Information Technology, software engineer.

**September 2008 – June 2013 – Belarusian State University**<br/>
Specialization: Faculty of Chemistry, research chemist

## Work experience 
**March 2020 – Educational Center for Programming and High Tech**<br/>
**Project description**: interactive SPA with animation. Periodic table of chemical elements and models of atoms.<br/>
**Project role**: The spa implementation, the tabs of which are: an interactive periodic table of chemical elements (using event delegation, requests to web-api, mvc pattern); Boron atom models (svg animation used); description of the quantum-mechanical model of the atom (the Chart js library was used to plot the graphs). Implemented cross-browser compatibility and adaptability.

**May 2013 - December 2018** – Process engineer, AluminTechno<br/>
**Main responsibilities**: Conducting chemical analyzes and physical and mechanical tests, monitoring the production process of anodizing and painting the aluminum profile. Passing inspections to confirm the Qualicoat and Qualanod certificates. Writing technological documentation (technological and working instructions, route maps). Work in the AluminTechno database.

## Additional Information
**Portfolio**: <br/>
- https://github.com/olgafurs/
- http://periodic-table-olgafurs.surge.sh/
- https://olgafurs.github.io/care-point/

## Professional interests:  
 
- https://developer.mozilla.org/ru/docs/Web/JavaScript
- https://learn.javascript.ru/
- http://itbeard.ru/
- https://www.youtube.com/user/iliakan/featured/ 
- https://www.youtube.com/user/dmitrylavr/featured 
- https://ru.stackoverflow.com

## References
Letter of recommendation from Educational Center for Programming and High Tech (IT-Academy)










