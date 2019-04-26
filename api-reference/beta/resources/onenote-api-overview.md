---
title: 使用 OneNote REST API
description: 'Microsoft Graph 允许你的应用获取对个人或组织帐户中的用户 OneNote 笔记本、节和页面的授权访问权限。 使用适当的委派或应用程序权限, 您的应用程序可以访问已登录用户的 OneNote 数据或租户中的任何用户。 '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 6d92faecfd58c74f519802fe308071828a3713dc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345532"
---
# <a name="use-the-onenote-rest-api"></a>使用 OneNote REST API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph 允许你的应用获取对个人或组织帐户中的用户 OneNote 笔记本、节和页面的授权访问权限。 使用[适当的委派或应用程序权限](/graph/permissions-reference#notes-permissions), 您的应用程序可以访问已登录用户的 OneNote 数据或租户中的任何用户。 

## <a name="root-url"></a>根 URL
onenote 服务根 URL 对 onenote API 的所有调用使用以下格式。
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

URL `version`中的段表示要使用的 Microsoft Graph 的版本:

- `v1.0` 用于稳定的生产代码。
- `beta` 用于试用正在开发的功能。 beta 终结点中的特性和功能可能会发生变化;我们建议您不要在生产代码中使用它。

该位置可以是 office 365 上的用户笔记本, 也可以是 office 365 上的使用者 OneDrive、组笔记本或 SharePoint 网站托管的团队笔记本。 

![OneNote API 开发堆栈](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a>用户笔记本
若要访问消费者 OneDrive 或 OneDrive for business 上的个人笔记本, 请使用下列 url 之一:

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- `me` 用于为当前用户可以访问的 OneNote 内容（拥有和共享）。
- `users/{id}` 用于指定用户已与当前用户共享的 OneNote 内容（此 URL 中）。 使用[用户](users.md)API。
> **注意:** 您可以通过发出 get 请求来获取用户 id `https://graph.microsoft.com/v1.0/users`。

### <a name="group-notebooks"></a>组笔记本

若要访问组拥有的笔记本, 请使用以下服务根 URL:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a>SharePoint 网站笔记本
若要访问 SharePoint 团队网站拥有的笔记本, 请使用以下服务根 URL:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
