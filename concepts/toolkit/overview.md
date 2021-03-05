---
title: Microsoft Graph Toolkit：适用于 Microsoft Graph 的 UI 组件和身份验证提供程序
description: Microsoft Graph Toolkit是身份验证提供程序和可重用的、与框架无关的 Web 组件的集合，用于访问和使用 Microsoft Graph。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 01f406c288ebca1dde5c6b1577fd2acdc7631d5b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470534"
---
# <a name="microsoft-graph-toolkit-ui-components-and-authentication-providers-for-microsoft-graph"></a>Microsoft Graph Toolkit：适用于 Microsoft Graph 的 UI 组件和身份验证提供程序 

Microsoft Graph Toolkit是可重用的、与框架无关的组件和身份验证提供程序的集合，用于访问和使用 Microsoft Graph。 这些组件具有开箱即用的功能，内置提供程序使用 Microsoft Graph 进行身份验证并提取数据。

Microsoft Graph Toolkit可轻松在应用程序中使用 Microsoft Graph。 在下面的示例中，登录用户及其日历事件使用登录和议程组件只显示两[行代码。](./components/agenda.md) [](./components/login.md)

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a>What's in the Microsoft Graph Toolkit?

### <a name="components"></a>组件

Microsoft Graph Toolkit包括一组 Web 组件，用于由 Microsoft Graph API 支持的最常用体验。 

这些组件也作为 [React 组件提供](./get-started/mgt-react.md)。

|组件|说明|
|---------|-----------|
|[登录](./components/login.md)|一个按钮和一个飞出控件，用于使用 Microsoft Identity 平台对用户进行身份验证，在登录时显示用户配置文件信息。|
|[人员](./components/person.md)|按个人或联系人的照片、姓名和/或电子邮件地址显示此人或联系人。|
|[人员](./components/people.md)|按照片或缩写显示一组人员或联系人。|
|[议程](./components/agenda.md)|显示用户或组的日历中的事件。|
|[任务](./components/tasks.md)|显示并启用添加、删除、完成或编辑 Microsoft Planner 或 Microsoft To Do 中的任务。|
|[人员选取器](./components/people-picker.md)|提供搜索人员并呈现结果列表的能力。|
|[个人卡片](./components/person-card.md)|在人员组件上用于显示有关用户的更多配置文件信息的飞出。|
|[获取](./components/get.md)|直接在 HTML 中对任意 Microsoft Graph API 进行 GET 查询。|
|[通道选取器](./components/teams-channel-picker.md)|提供搜索 Microsoft Teams 频道以从呈现的结果列表中选择频道的能力。|
|[待办事项](./components/todo.md)|显示并启用添加、删除、完成或编辑 Microsoft To Do 中的任务。|

### <a name="providers"></a>提供程序

[提供程序](/providers/providers.md) 启用身份验证并提供在各种平台上获取访问令牌的实现，并公开用于调用 Microsoft Graph API 的 Microsoft Graph 客户端。 组件在与提供程序一起使用时效果最佳，但提供程序可以自行使用。

|提供程序|说明|
|---------|-----------|
|[Msal](./providers/msal.md)|使用MSAL.js登录用户并获取用于 Microsoft Graph 的令牌。|
|[云](./providers/electron.md)|验证并提供 Microsoft Graph 对"一线"应用内组件的访问|
|[SharePoint](./providers/sharepoint.md)|对 SharePoint Web 部件内的组件进行身份验证并提供 Microsoft Graph 访问。|
|[Teams](./providers/teams.md)|对 Microsoft Teams 选项卡内的组件进行身份验证并提供 Microsoft Graph 访问。|
|[代理](./providers/proxy.md)|允许通过后端路由对 Microsoft Graph 的所有调用来使用后端身份验证。|
|[自定义](./providers/custom.md)|创建自定义提供程序以使用应用程序的现有身份验证代码启用身份验证并访问 Microsoft Graph。|

## <a name="why-use-the-microsoft-graph-toolkit"></a>为什么使用 Microsoft Graph Toolkit？

Microsoft Graph Toolkit使由 Microsoft Graph 支持的共同体验快速轻松地集成到你自己的应用程序中。

:::row:::
   :::column span="":::
    **剪切开发时间**

    连接到 Microsoft Graph API 和在 UI 中呈现数据（外观和感觉就像 Microsoft365 体验）的工作已由你完成，无需进行自定义。
  :::column-end:::
  :::column span="":::
    **适用于任何地方**

    所有组件均基于 Web 标准，可与 React、Angular、Vue 等 (浏览器和 Web 框架无缝) 。 
  :::column-end:::
  :::column span="":::
    **美观但灵活**

    这些组件旨在外观与 Microsoft365 体验类似，但也可使用 [CSS](./customize-components/style.md) 自定义属性和 [模板进行自定义](./customize-components/templates.md)。
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a>谁应该使用它？

Microsoft Graph Toolkit对于希望开发连接到 Microsoft Graph 和从 Microsoft Graph 访问数据的应用（例如：
- Web 应用
- Microsoft Teams 选项卡
- 渐进式 Web App (PWA) 
- 光化应用
- SharePoint Web 部件

## <a name="where-can-i-use-it"></a>在哪里可以使用？

以下Toolkit支持 Microsoft Graph 浏览器。

|![Microsoft Edge](images/edgeIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![三星 Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|**Microsoft Edge**|**Firefox**|**Chrome**|**Safari**|**Opera**|**Samsung**|

## <a name="next-steps"></a>后续步骤

- 尝试在运动场 [中的组件](https://mgt.dev)。
- [Microsoft](./get-started/overview.md) Graph Toolkit。
- 查看 GitHub 上的 Microsoft Graph [Toolkit。](https://aka.ms/mgt)
