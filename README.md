<p align="center">
  <a href="https://perfectscrollbar.com/?utm_source=GitHub&utm_medium=PerfectScrollbar">
    <img src="https://perfectscrollbar.com/logo2.png" width="300" height="200">
  </a>
</p>

<h1 align="center">perfect-scrollbar (with custom classnames!)</h1>

<p align="center">Minimalistic but perfect custom scrollbar plugin, and now you can overwrite classnames!<p>

<p align="center">  
  <a href="https://npmcharts.com/compare/perfect-scrollbar?minimal=true"><img src="https://img.shields.io/npm/dm/perfect-scrollbar.svg" alt="Downloads"></a>
  <a href="https://github.com/mdbootstrap/bootstrap-material-design/blob/master/License.pdf"><img src="https://img.shields.io/badge/license-MIT-green.svg" alt="License"></a> 
  <a href="https://badge.fury.io/js/perfect-scrollbar"><img src="https://badge.fury.io/js/perfect-scrollbar.svg" alt="npm"></a> 
<a href="https://twitter.com/intent/tweet/?text=Thanks+@mdbootstrap+for+maintaining+amazing+and+free+Perfect+Scrollbar+Plugin%20https://perfectscrollbar.com/&hashtags=javascript,code,webdesign,bootstrap"><img src="https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Let%20us%20know%20you%20were%20here%21&"></a>
<a href="https://www.youtube.com/watch?v=c9B4TPnak1A"><img alt="YouTube Video Views" src="https://img.shields.io/youtube/views/c9B4TPnak1A?label=Bootstrap%205%20Tutorial%20Views&style=social"></a>
</p>

---

## How to overwrite classnames

```
const ps = new PerfectScrollbar('#my-thing-contaner', {
  classes: {
    main: 'my-thing',
    rtl: 'my-thing__rtl',
    element: {
      thumb: (x) => `my-thing__thumb-${x}`,
      rail: (x) => `my-thing__rail-${x}`,
      consuming: 'my-thing__child--consume',
    },
    state: {
      focus: 'my-thing--focus',
      clicking: 'my-thing--clicking',
      active: (x) => `my-thing--active-${x}`,
      scrolling: (x) => `my-thing--scrolling-${x}`,
    },
  },
});
```
