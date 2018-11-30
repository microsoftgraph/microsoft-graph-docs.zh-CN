---
title: 使用 OneNote REST API
description: Microsoft Graph 允许您获取授权的访问用户的 OneNote 笔记本、 节和页面中的个人或组织帐户的应用程序。 使用适当委派或应用程序权限，您的应用程序可以访问已登录的用户或租户中的任何用户的 OneNote 数据。
ms.openlocfilehash: c439e7896eea85e84d567e54aaa57bb5191a70d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008023"
---
# <a name="use-the-onenote-rest-api"></a>使用 OneNote REST API

Microsoft Graph 允许您获取授权的访问用户的 OneNote 笔记本、 节和页面中的个人或组织帐户的应用程序。 使用[适当的委派或应用程序权限](/graph/permissions-reference#notes-permissions)，您的应用程序可以访问已登录的用户或租户中的任何用户的 OneNote 数据。

## <a name="root-url"></a>根 URL
OneNote 服务根 URL 为 OneNote API 的所有调用使用以下格式。
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
`version` URL 中的段代表您想要使用的 Microsoft Graph 的版本：

- `v1.0` 用于稳定的生产代码。
- `beta` 用于试用正在开发的功能。 功能和 beta 终结点中的功能可能会更改;我们建议不要在生产代码中使用它。

位置可以是在 Office 365 或使用者 OneDrive 用户笔记本、 组笔记本或在 Office 365 上的 SharePoint 网站承载团队笔记本。 

![OneNote API 开发堆栈](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a>用户笔记本
若要访问 OneDrive 或 OneDrive for Business 的使用者上的个人笔记本，请使用以下 Url 之一：

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- `me` 用于为当前用户可以访问的 OneNote 内容（拥有和共享）。
- `users/{id}` 用于指定用户已与当前用户共享的 OneNote 内容（此 URL 中）。 使用[用户](users.md)API。
> **注意：** 您可以通过 GET 请求上获取用户 Id `https://graph.microsoft.com/v1.0/users`。

### <a name="group-notebooks"></a>组笔记本
若要访问一组由拥有的笔记本，请使用以下服务根 URL:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a>SharePoint 网站笔记本

若要访问笔记本所拥有的 SharePoint 工作组网站，请使用以下服务根 URL:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

