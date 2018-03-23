# text-htm-to-Virtualhyperscript-converter

This is my project that convert Text format of HTML into Virtual-Hyperscript 

example :-


     <div id="application">
          <p>{ message }</p>
          <button on:click="reverseMessage">Reverse Message</button>
          <ol>
            <li forloop="todo in todos">
              { todo.text }
            </li>
          </ol>
        </div>
        
        
        to:-
        
        
          {
      "type": "root",
      "children": [
       "   \n        ",
        {
        "type": "div",
        "props": {
        "id": {
       "name": "id",
       "value": "application",
       "meta": {}
       }
      },
      "children": [
       "\n          ",
       {
       "type": "p",
       "props": {},
       "children": [
        "{ message }"
       ]
      },
      "\n          ",
      {
       "type": "button",
       "props": {
        "on:click": {
         "name": "on",
         "value": "reverseMessage",
         "meta": {
          "args": "click"
         }
        }
       },
       "children": [
        "Reverse Message"
       ]
      },
      "\n          ",
      {
       "type": "ol",
       "props": {},
       "children": [
        "\n            ",
        {
         "type": "li",
         "props": {
          "forloop": {
           "name": "forloop",
           "value": "todo in todos",
           "meta": {}
          }
         },
         "children": [
           "\n              { todo.text }\n            "
         ]
        },
        "\n          "
       ]
      },
      "\n        "
     ]
    },
    "\n   "
    ]
    }
   
   
