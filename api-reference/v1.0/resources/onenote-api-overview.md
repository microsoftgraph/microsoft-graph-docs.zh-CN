---
title: 使用 OneNote REST API
description: Microsoft Graph 可让应用获得授权，访问个人或组织帐户中用户的 OneNote 笔记本、分区和页面。使用适当的委托权限或应用程序权限，应用可以访问已登录用户或租户中任何用户的 OneNote 数据。
localization_priority: Priority
author: jewan-microsoft
ms.prod: onenote
doc_type: conceptualPageType
ms.openlocfilehash: 1d9543a7192d8f4f4d6603d1ccd6df237b2ee4bf84d3f1d1882492901175ee48
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141411"
---
# <a name="use-the-onenote-rest-api"></a>使用 OneNote REST API

Microsoft Graph 可让应用程序获得对个人或组织帐户中用户的 OneNote 笔记本、节和页面的授权访问权限。 使用[适当的委派或应用程序权限](/graph/permissions-reference#notes-permissions)，你的应用程序可以访问已登录用户或租户中任何用户的 OneNote 数据。

## <a name="root-url"></a>根 URL
OneNote 服务根 URL 为 OneNote API 的所有调用使用以下格式。
```http
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
URL 中的 `version` 段表示想要使用的 Microsoft Graph 的版本：

- `v1.0` 用于稳定的生产代码。
- `beta` 用于试用正在开发的功能。 Beta 终结点中的特性和功能可能改变；不推荐将其用于生产代码中。

位置可以是 Microsoft 365 的用户笔记簿，或是消费者版 OneDrive ，或者是组笔记，或者可以是Microsoft 365 上的 SharePoint 站点托管团队笔记本。 

![OneNote API 开发堆栈](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

## <a name="user-notebooks"></a>用户笔记本
要访问消费者版 OneDrive 或 OneDrive for Business 上的个人笔记本，请使用下列 URL 之一：

```http
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- `me` 用于为当前用户可以访问的 OneNote 内容（拥有和共享）。
- `users/{id}` 用于指定用户已与当前用户共享的 OneNote 内容（此 URL 中）。 使用 [users](users.md) API。
> **注意：** 可以通过在 `https://graph.microsoft.com/v1.0/users` 上发出 GET 请求来获取用户 ID。

## <a name="group-notebooks"></a>组笔记本
要访问组所有的笔记本，请使用下列服务根 URL：

```http
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="sharepoint-site-notebooks"></a>SharePoint 网站笔记本

要访问 SharePoint 团队网站拥有的笔记本，请使用下列服务根 URL：

```http
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

