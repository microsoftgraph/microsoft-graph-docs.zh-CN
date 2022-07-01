---
title: Microsoft Graph 工具包概述
description: 使用 Microsoft Graph 工具包查找身份验证提供程序和可重用、框架不可知的 Web 组件，以便访问和使用 Microsoft Graph。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: a448d79a789f142a2e05bca0e4096db9df127158
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577803"
---
# <a name="microsoft-graph-toolkit-overview"></a>Microsoft Graph 工具包概述 

Microsoft Graph 工具包 是可重复使用、与框架 无关的组件和身份认证提供程序的集合，用于访问和使用 Microsoft Graph。 这些组件开箱即可正常运行，附带的内置提供程序可以与 Microsoft Graph 进行身份验证并从之提取数据。

Microsoft Graph 工具包 可以使得在应用程序中使用 Microsoft Graph 变得轻松。 在下面的示例中，登录用户及其日历事件仅使用[登录和](./components/login.md)[议程](./components/agenda.md)组件显示两行代码。

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)。

## <a name="whats-in-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的内容是什么？

### <a name="components"></a>组件

Microsoft Graph 工具包包含 Web 组件的集合，用于 Microsoft Graph API 提供支持的最常见的生成体验。

这些组件还可作为 [React 组件](./get-started/mgt-react.md) 使用。

|组件|说明|
|---------|-----------|
|[登录](./components/login.md)|一个按钮和一个浮出控件，用于使用 Microsoft 标识平台对用户进行身份验证，并在用户登录时显示其个人资料信息。|
|[人员](./components/person.md)|通过照片、姓名和/或电子邮件地址显示人员或联系人。|
|[人员](./components/people.md)|按照照片或首字母缩写显示一组人员或联系人。|
|[议程](./components/agenda.md)|在用户或组的日历中显示事件。|
|[人员选取器](./components/people-picker.md)|提供搜索人员和呈现结果列表的功能。|
|[个人卡片](./components/person-card.md)|用于显示有关用户的更多个人资料信息的人员组件上的浮出控件。|
|[文件](./components/file.md)|表示具有图标、文件名、作者等的文件或文件夹。|
|[文件列表](./components/file-list.md)|显示多个文件或文件夹的列表。|
|[获取](./components/get.md)|允许直接在 HTML 中对任何 Microsoft 图形 API进行 GET 查询。|
|[频道选取器](./components/teams-channel-picker.md)|提供搜索 Microsoft Teams 频道以从呈现的结果列表中选择频道的功能。|
|[待办事项](./components/todo.md)|显示并启用添加、删除、完成或编辑微软待办中的任务。|
|[Tasks](./components/tasks.md)|显示并启用添加、删除、完成或编辑 Microsoft Planner 或微软待办中的任务。|

### <a name="providers"></a>提供程序

[提供程序](./providers/providers.md) 启用身份验证，提供用于在各种平台上获取访问令牌的实现，并公开用于调用 Microsoft Graph API 的 Microsoft Graph 客户端。 组件在与提供程序一起使用时效果最佳，但提供程序也可以自行使用。

|提供程序|说明|
|---------|-----------|
|[MSAL](./providers/msal.md)|使用 msal.js 登录用户并获取用于 Microsoft Graph 的令牌。|
|[MSAL2](./providers/msal2.md)| 使用 msal-browser 登录用户并获取用于 Microsoft Graph 的令牌。|
|[电子](./providers/electron.md)|对电子应用中的组件进行身份验证并提供 Microsoft Graph 访问权限。|
|[SharePoint](./providers/sharepoint.md)|对 SharePoint Web 部件中的组件进行身份验证并提供对组件的 Microsoft Graph 访问权限。|
|[Teams](./providers/teams.md)|使用msal.js在 Microsoft Teams 选项卡上登录用户并获取客户端上的令牌。|
|[Teams MSAL2](./providers/teams-msal2.md)|使用 msal-browser 在 Microsoft Teams 选项卡上登录用户和获取令牌。 支持使用自定义后端的单一登录 (SSO) 。 |
|[代理](./providers/proxy.md)|通过后端将所有调用路由到 Microsoft Graph 以允许使用后端身份验证。|
|[自定义](./providers/custom.md)|创建自定义提供程序，以使用应用程序的现有身份验证代码启用身份验证和访问 Microsoft Graph。|

## <a name="why-use-microsoft-graph-toolkit"></a>为什么要使用 Microsoft Graph 工具包？

借助 Microsoft Graph 工具包，可以快速轻松地将 Microsoft Graph 支持的常见体验集成到自己的应用程序中。 工具包：

- **缩短开发时间**。 连接到 Microsoft Graph API 并在 UI 中呈现数据（看起来和感觉类似于 Microsoft 365 体验）的工作是为你完成的，无需自定义。

- **可在任何地方工作**。 所有组件都基于 Web 标准，可与任何新式浏览器和 Web 框架 (（如 React、Angular 或 Vue) ）无缝配合使用。 

- **是美丽，但灵活**。 这些组件的设计外观类似于 Microsoft 365 体验，但也可使用 [CSS 自定义属性](./customize-components/style.md) 和 [模板](./customize-components/templates.md)进行自定义。

## <a name="who-should-use-it"></a>谁应该使用它?

Microsoft Graph 工具包非常适合所有体验级别的开发人员，他们想要开发连接到 Microsoft Graph 并访问数据的应用，例如：
- Web 应用
- Microsoft Teams 选项卡
- 渐进式 Web 应用 (PWA)
- 电子应用
- SharePoint Web 部件

## <a name="where-can-i-use-it"></a>在哪里可以使用它?

以下浏览器支持 Microsoft Graph 工具包：

|![Microsoft Edge](images/edgeIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|**Microsoft Edge**|**Firefox**|**Chrome**|**Safari**|**Opera**|**Samsung**|

## <a name="next-steps"></a>后续步骤

- 在[样本](https://mgt.dev)中试用组件。
- [Microsoft](./get-started/overview.md) Graph 工具包入门。
- 查看 [GitHub](https://aka.ms/mgt) 上的 Microsoft Graph 工具包。
