---
title: 使用 OneNote REST API
description: 'Microsoft Graph 允许您获取授权的访问用户的 OneNote 笔记本、 节和页面中的个人或组织帐户的应用程序。 使用适当委派或应用程序权限，您的应用程序可以访问已登录的用户或租户中的任何用户的 OneNote 数据。 '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7db3024224dde7ee4c95d2e3840187709471cecd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525624"
---
# <a name="use-the-onenote-rest-api"></a>使用 OneNote REST API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph 允许您获取授权的访问用户的 OneNote 笔记本、 节和页面中的个人或组织帐户的应用程序。 使用[适当的委派或应用程序权限](/graph/permissions-reference#notes-permissions)，您的应用程序可以访问已登录的用户或租户中的任何用户的 OneNote 数据。 

## <a name="root-url"></a>根 URL
OneNote 服务根 URL 为 OneNote API 的所有调用使用以下格式。
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

`version` URL 中的段代表您想要使用的 Microsoft Graph 的版本：

- `v1.0` 用于稳定的生产代码。
- `beta` 用于试用正在开发的功能。 功能和 beta 终结点中的功能可能会更改;我们建议不要在生产代码中使用它。

位置可以是 Office 365 或消费者版 OneDrive 上的用户笔记本，还可以是 Office 365 上的组笔记本或 SharePoint 站点托管的团队笔记本。 

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
> **注意：** 可以通过在 `https://graph.microsoft.com/v1.0/users` 上发出 GET 请求来获取用户 ID。

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenote-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
