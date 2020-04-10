---
title: Microsoft Graph 工具包：由 Microsoft Graph 提供支持的 Web 组件
description: Microsoft Graph 工具包是 resuable、框架不可知的 web 组件以及用于访问和使用 Microsoft Graph 的帮助程序的集合。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 2ba11a66dcec1eaec276b3fe71427fcf356cbcde
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181614"
---
# <a name="microsoft-graph-toolkit-web-components-powered-by-microsoft-graph"></a>Microsoft Graph 工具包：由 Microsoft Graph 提供支持的 Web 组件

Microsoft Graph 工具包是用于访问和使用 Microsoft Graph 的可重用、框架不可知 web 组件和帮助器的集合。 组件在现成的功能中完全正常，内置提供程序，可通过 Microsoft Graph 中的数据进行身份验证和获取数据。

使用 Microsoft Graph 工具包，可以轻松地在应用程序中使用 Microsoft Graph。 在下面的示例中，查看登录用户及其日历事件如何使用[登录](./components/login.md)和[议程](./components/agenda.md)组件仅显示两行代码。

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[在 "dev" 中打开此示例](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的内容是什么？

### <a name="components"></a>组件

Microsoft Graph 工具包包含一系列 web 组件，用于 Microsoft Graph Api 所支持的最常见的构建体验。

|组件|说明|
|---------|-----------|
|[登录](./components/login.md)|一个按钮和一个浮出控件，用于对用户进行身份验证，以使用 Microsoft 标识平台并在登录时显示用户的配置文件信息。|
|[人员](./components/person.md)|按照片、姓名和/或电子邮件地址显示人员或联系人。|
|[人员](./components/people.md)|按照片或缩写显示一组人或联系人。|
|[日程](./components/agenda.md)|显示用户或组的日历中的事件。|
|[任务](./components/tasks.md)|显示并允许添加、删除、完成或编辑 Microsoft Planner 或 Microsoft To Do 中的任务。|
|[人员选取器](./components/people-picker.md)|提供搜索人员并呈现结果列表的功能。|
|[个人卡片](./components/person-card.md)|在 person 组件上使用的浮出控件，用于显示有关用户的更多配置文件信息。|
|[获取](./components/get.md)|在 HTML 中直接向任何 Microsoft Graph API 发出 GET 查询。|
|[频道选取器](./components/teams-channel-picker.md)|提供搜索 Microsoft 团队频道以从呈现的结果列表中选择频道的功能。|

### <a name="providers"></a>提供程序

与[提供程序](/providers/providers.md)配合使用时，组件的工作效果最佳。 提供程序启用身份验证，并提供用于获取调用 Microsoft Graph Api 的访问令牌的实现。

|提供程序|Description|
|---------|-----------|
|[Msal](./providers/msal.md)|使用 MSAL 登录用户并获取令牌以用于 Microsoft Graph。|
|[SharePoint](./providers/sharepoint.md)|对 SharePoint web 部件内的组件进行身份验证并提供 Microsoft Graph 访问权限。|
|[Teams](./providers/teams.md)|对 Microsoft 团队选项卡内的组件进行身份验证并提供 Microsoft Graph 访问权限。|
|[代理](./providers/proxy.md)|通过将对 Microsoft Graph 的所有调用通过后端路由，允许使用后端身份验证。|
|[自定义](./providers/custom.md)|创建自定义提供程序，以便通过应用程序的现有身份验证代码启用对 Microsoft Graph 的身份验证和访问。|

## <a name="why-use-the-microsoft-graph-toolkit"></a>为什么要使用 Microsoft Graph 工具包？

Microsoft Graph 工具包将 Microsoft Graph 所支持的常见体验集成到您自己的应用程序中，快速轻松地实现。

:::row:::
   :::column span="":::
    **缩短开发时间**

    连接到 Microsoft Graph Api 并在 UI 中呈现数据的工作在外观和感觉像 Microsoft365 体验的 UI 中，无需进行自定义。
  :::column-end:::
  :::column span="":::
    **随处工作**

    所有组件都基于 web 标准，并可与任何新式浏览器和 web 框架无缝协作（反应、角度、Vue 等）。 
  :::column-end:::
  :::column span="":::
    **漂亮但灵活**

    这些组件设计为外观和感觉像 Microsoft365，但也可以使用[CSS 自定义属性](./style.md)和[模板](./templates.md)进行自定义。
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a>谁应使用它？

Microsoft Graph 工具包非常适合于开发用于开发 web 应用程序、Microsoft 团队选项卡或 SharePoint web 部件的所有体验级别，这些应用程序将连接到 Microsoft Graph 中的数据并对其进行访问。

## <a name="where-can-i-use-it"></a>在哪里可以使用它？

以下浏览器支持 Microsoft Graph 工具包。

|![Microsoft Edge](images/edgeIcon.png)|![Internet Explorer 11](images/internetExplorerIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|**Microsoft Edge**|**IE 11**|**Firefox**|**Chrome**|**Safari**|**Opera**|**Samsung**|

## <a name="next-steps"></a>后续步骤

- 尝试[样本](https://mgt.dev)中的组件。
- [开始](get-started.md)使用 Microsoft Graph 工具包。
