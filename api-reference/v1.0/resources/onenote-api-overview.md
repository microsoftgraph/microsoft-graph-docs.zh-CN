---
title: 使用 OneNote REST API
description: 'Microsoft Graph 可让应用程序获得对个人或组织帐户中用户的 OneNote 笔记本、节和页面的授权访问权限。 使用适当的委派或应用程序权限，你的应用程序可以访问已登录用户或租户中任何用户的 OneNote 数据。 '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ceb5ac30786ecfd207a2076d471e9d004b60f8d3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462954"
---
# <a name="use-the-onenote-rest-api"></a>使用 OneNote REST API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph 可让应用程序获得对个人或组织帐户中用户的 OneNote 笔记本、节和页面的授权访问权限。 使用[适当的委派或应用程序权限](/graph/permissions-reference#notes-permissions)，你的应用程序可以访问已登录用户或租户中任何用户的 OneNote 数据。 

## <a name="root-url"></a>根 URL
OneNote 服务根 URL 为 OneNote API 的所有调用使用以下格式。
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

URL 中的 `version` 段表示想要使用的 Microsoft Graph 的版本：

- `v1.0` 用于稳定的生产代码。
- `beta` 用于试用正在开发的功能。 Beta 终结点中的特性和功能可能改变；不推荐将其用于生产代码中。

位置可以是 Office 365 或消费者版 OneDrive 上的用户笔记本，还可以是 Office 365 上的组笔记本或 SharePoint 站点托管的团队笔记本。 

![OneNote API 开发堆栈](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a>用户笔记本
要访问消费者版 OneDrive 或 OneDrive for Business 上的个人笔记本，请使用下列 URL 之一：

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- `me` 用于为当前用户可以访问的 OneNote 内容（拥有和共享）。
- `users/{id}` 用于指定用户已与当前用户共享的 OneNote 内容（此 URL 中）。 使用 [users](users.md) API。
> **注意：** 可以通过在 `https://graph.microsoft.com/v1.0/users` 上发出 GET 请求来获取用户 ID。

### <a name="group-notebooks"></a>组笔记本

要访问组所有的笔记本，请使用下列服务根 URL：

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a>SharePoint 网站笔记本
要访问 SharePoint 团队网站拥有的笔记本，请使用下列服务根 URL：

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
