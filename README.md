carousel-react-js
=================

Infinite loop carousel with CSS3 transition. Really fluid animation with translate3d animation.

How to use it ?

```
var React = require('react/addons'),
    Caroussel = require('./ui-components/caroussel'),
    domready = require('domready');

var content = [
    {
        img: "img/illus-login_1.jpg",
        title: "Gros titre n°1",
        descr: "1 - Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor..."
    },
    {
        img: "img/illus-login_2.jpg",
        title: "Gros titre n°2",
        descr: "2 - Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor..."
    },
    {
        img: "img/illus-login_3.jpg",
        title: "Gros titre n°3",
        descr: "3 - Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor..."
    }
];

domready(function() {
    React.renderComponent(
        <Caroussel width="632" data={content} />,
        document.getElementsByClassName("caroussel__rp")[0]
    );
});
```
