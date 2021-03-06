---
title: Microsoft Graph Toolkit：Microsoft Graph 的 UI 组件和身份验证提供程序
description: Microsoft Graph Toolkit是一组身份验证提供程序和可重用的、与框架无关的 Web 组件，用于访问和使用 Microsoft Graph。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 3b9dd368f9fe565164f3025c1f3de81645ad22df
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629159"
---
# <a name="microsoft-graph-toolkit-ui-components-and-authentication-providers-for-microsoft-graph"></a>Microsoft Graph Toolkit：Microsoft Graph 的 UI 组件和身份验证提供程序 

Microsoft Graph Toolkit是可重用的、与框架无关的组件和身份验证提供程序的集合，用于访问和使用 Microsoft Graph。 这些组件具有开箱即用的功能，内置提供程序使用 Microsoft Graph 进行身份验证和提取数据。

Microsoft Graph Toolkit使你能够轻松地在应用程序中Graph Microsoft 应用程序。 在下面的示例中，登录用户及其日历事件使用 [Login](./components/login.md) 和 [Agenda](./components/agenda.md) 组件只显示两行代码。

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[在"打开"mgt.dev](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a>Microsoft Graph Toolkit？

### <a name="components"></a>组件

Microsoft Graph Toolkit包括一组 Web 组件，用于由 Microsoft Graph API 支持的最常用体验。 

这些组件还可作为React[组件。](./get-started/mgt-react.md)

|组件|说明|
|---------|-----------|
|[登录](./components/login.md)|一个按钮和一个飞出控件，用于使用 Microsoft Identity 平台对用户进行身份验证，在登录时显示用户配置文件信息。|
|[人员](./components/person.md)|按照片、姓名和/或电子邮件地址显示个人或联系人。|
|[人员](./components/people.md)|按照片或缩写显示一组人员或联系人。|
|[议程](./components/agenda.md)|显示用户或组的日历中的事件。|
|[人员选取器](./components/people-picker.md)|提供搜索人员并呈现结果列表的能力。|
|[个人卡片](./components/person-card.md)|在人员组件上用于显示有关用户的更多个人资料信息的飞出图。|
|[文件](./components/file.md)|表示包含图标、文件名、作者等的文件或文件夹。|
|[文件列表](./components/file-list.md)|显示多个文件或文件夹的列表。|
|[获取](./components/get.md)|直接在 HTML 中对任意 Microsoft Graph API 进行 GET 查询。|
|[通道选取器](./components/teams-channel-picker.md)|提供搜索特定Microsoft Teams以从呈现的结果列表中选择通道的能力。|
|[待办事项](./components/todo.md)|显示并启用在任务中添加、删除、完成或编辑任务微软待办。|
|[Tasks](./components/tasks.md)|显示并启用添加、删除、完成或编辑 Microsoft Planner 或 微软待办。|

### <a name="providers"></a>提供程序

[提供程序](/providers/providers.md)启用身份验证并提供用于在各种平台上获取访问令牌的实现，并公开用于调用 Microsoft Graph API 的 Microsoft Graph 客户端。 这些组件在用于提供程序时效果最佳，但提供程序可自行使用。

|提供程序|说明|
|---------|-----------|
|[Msal](./providers/msal.md)|使用 MSAL.js 登录用户并获取与 Microsoft Graph 一Graph。|
|[Msal 2.0](./providers/msal2.md)| 使用 msal-browser 登录用户并获取与 Microsoft Graph 一Graph。|
|[百年](./providers/electron.md)|通过身份验证并提供 Microsoft Graph访问"一线"应用内的组件|
|[SharePoint](./providers/sharepoint.md)|通过身份验证并提供 Microsoft Graph访问 Web 部件内SharePoint权限。|
|[Teams](./providers/teams.md)|通过身份验证并提供 Microsoft Graph访问选项卡内的组件Microsoft Teams权限。|
|[代理](./providers/proxy.md)|允许通过后端将所有调用路由到 Microsoft Graph后端身份验证。|
|[自定义](./providers/custom.md)|创建自定义提供程序以使用应用程序的现有身份验证代码Graph访问 Microsoft 客户端。|

## <a name="why-use-the-microsoft-graph-toolkit"></a>为什么使用 Microsoft Graph Toolkit？

Microsoft Graph Toolkit使由 Microsoft 支持的共同体验Graph轻松快速地集成到你自己的应用程序中。

:::row:::
   :::column span="":::
    **剪切开发时间**

    连接到 Microsoft Graph API 和在 UI 中呈现数据（外观和感觉就像 Microsoft365 体验）的工作已由你完成，无需进行自定义。
  :::column-end:::
  :::column span="":::
    **适用于任何地方**

    所有组件均基于 Web 标准，可与任何新式浏览器和 Web 框架 (React、Angular、Vue 等) 。 
  :::column-end:::
  :::column span="":::
    **美观但灵活**

    这些组件旨在外观与 Microsoft365 体验类似，但也可使用 [CSS](./customize-components/style.md) 自定义属性和 [模板进行自定义](./customize-components/templates.md)。
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a>Who应该使用它？

Microsoft Graph Toolkit非常适用于希望开发连接到 Microsoft Graph 和访问数据的应用的所有体验级别的开发人员，例如：
- Web 应用
- Microsoft Teams选项卡
- 渐进式 Web 应用 (PWA) 
- 中国应用
- SharePoint Web 部件

## <a name="where-can-i-use-it"></a>在哪里可以使用它？

以下Graph Toolkit支持 Microsoft 浏览器。

|![Microsoft Edge](images/edgeIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|**Microsoft Edge**|**Firefox**|**Chrome**|**Safari**|**Opera**|**三星**|

## <a name="next-steps"></a>后续步骤

- 尝试在运动场中的 [组件](https://mgt.dev)。
- [开始使用](./get-started/overview.md)Microsoft Graph Toolkit。
- 请查看 Microsoft Graph Toolkit上的[GitHub。](https://aka.ms/mgt)
