---
subtitle: 工具箱概述?
title: Polymer App Toolbox
---

Polymer App Toolbox包括了使用Polymer用来构建
[Progressive Web Apps](https://developers.google.com/web/progressive-web-apps)
组件，工具和模板。 App Toolbox 特点:

-   使用Polymer和web components的基于组件架构。
-   使用[app layout components](https://elements.polymer-project.org/elements/app-layout)的响应式设计。
-   使用
    [`<app-route>`](https://elements.polymer-project.org/elements/app-route)组件进行模块化路由。
-   使用
    [`<app-localize-behavior>`](https://elements.polymer-project.org/elements/app-localize-behavior)进行本地化。
-   基于
    [app storage elements](https://elements.polymer-project.org/elements/app-storage)的本地存储支持.
-   使用service worker进行离线缓存，便于持续改进.
-   内置工具支持应用的多种访问：基于HTTP/2的非绑定服务器推送，基于HTTP/1.的绑定式推送。

可以单独使用某个组件或同时使用多个组件来构建全功能的rogressive web app。最重要的是，每个组件都是_additive_。对于一个简单应用来说，你只需要app-layout。随着应用越来越复杂，不断添加路由，离线缓存，当然这些功能都需要一个高性能服务器来支持。

访问[Shop demo](https://shop.polymer-project.org/)以便获得这些组件功能更直观的感受。Shop是一个全功能的购物网站，它符合 Progressive web
app并使用Toolbox构建。点击这里查看Shop是如何构建的R[Case study: the Shop app](case-study)。

立即开始使用App Toolbox，点击[Build an app with App Toolbox](/1.0/start/toolbox/set-up)。

了解更多[Responsive app layout](app-layout)。

<a href="/1.0/start/toolbox/set-up" class="blue-button">构建一个应用
</a>

<a href="app-layout" class="blue-button">响应式应用布局</a>
