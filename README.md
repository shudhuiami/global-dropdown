# Global-DropDown (A simple pure javascript based DropDown plugin)

Simple, easy to use and small in size plugin.
Based on pure Javascript.

#View Demo

View [Global Drop-down](https://shudhuiami.github.io/projects/global-dropdown) live demo. 

# Getting started

> ### Installation

#### Quick Start with GIT with [Documentation](https://github.com/shudhuiami/global-dropdown)
```
git clone https://github.com/shudhuiami/global-dropdown.git
```


#### Quick Start with NPM
* Install with [NPM](https://www.npmjs.com/package/global-dropdown) ```npm install global-dropdown```

> ##Usage

####JavaScript

Import **app.js**

```
<script src="global-dropdown/app.js" type="text/javascript"></script>
```
**OR**
```
@import 'global-dropdown/app.js';
```

####HTML

> #####Important Parts:

* data-query="dropdown-wrapper"
* data-query="dropdown-trigger"
* data-query="dropdown-box"

Those parts should not be changed and structured as follow.

```
    <div class="dropdown-wrapper" data-query="dropdown-wrapper">
        <a class="action-triiger" data-query="dropdown-trigger">DropDown-1</a>
        <div class="dropdown-box" data-query="dropdown-box">
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Product</a></li>
                <li><a href="#">About us</a></li>
                <li><a href="#">Contact us</a></li>
            </ul>
        </div>
    </div>
```

You can design or create the inner element as you want.



####CSS
style as you want but basic structure should be like this.

> #####Important Parts: 

* The Drop-down element(dropdown-box) should have a class called **_active** as following css shows.
    
    
```
.dropdown-wrapper {
  position: relative;
  width: auto;
  height: auto;
  display: table;
  float: left;
  margin: 0 20px;
  .action-triiger {
    width: 100px;
    height: 40px;
    line-height: 40px;
    float: left;
    background-color: #fff;
    color: #222;
    cursor: pointer;
    border: 1px solid #dfdfdf;
  }
  .dropdown-box {
    position: absolute;
    left: 0;
    top: 100%;
    width: 200px;
    height: auto;
    display: table;
    background-color: #fff;
    border: 1px solid #dfdfdf;
    visibility: hidden;
    padding: 10px 0 0 0;
    ul {
      margin: 0;
      padding: 0;
      li {
        list-style: none;
        a {
          padding: 5px 20px;
          width: 100%;
          display: block;
          text-decoration: none;
          color: #222;
          text-align: left;
          box-sizing: border-box;
          border-bottom: 1px solid transparent;
          &:hover {
            border-bottom: 1px solid #dfdfdf;
          }
        }
      }
    }
    &._active {
      visibility: visible;
    }
  }
}
```

##That's all have fun.