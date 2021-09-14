---
title: 使用 OneNote REST API
description: Microsoft Graph 可让应用获得授权，访问个人或组织帐户中用户的 OneNote 笔记本、分区和页面。使用适当的委托权限或应用程序权限，应用可以访问已登录用户或租户中任何用户的 OneNote 数据。
ms.localizationpriority: high
author: jewan-microsoft
ms.prod: onenote
doc_type: conceptualPageType
ms.openlocfilehash: 9d34da129e354134a55efb682c5be098c73baaad
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094182"
---
# <a name="use-the-onenote-rest-api"></a>使用 OneNote REST API

通过 Microsoft Graph，应用可以获得授权，以访问个人或组织帐户中用户的 OneNote 笔记本、分区和页面。使用 [适当的委派权限或应用程序权限](/graph/permissions-reference#notes-permissions)，应用可以访问已登录用户或租户中任何用户的 OneNote 数据。

## <a name="root-url"></a>根 URL
OneNote 服务根 URL 为 OneNote API 的所有调用使用以下格式。
```http
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
URL 中的 `version` 段表示想要使用的 Microsoft Graph 的版本：

- `v1.0` 用于稳定的生产代码。
- `beta` 是试用开发中的功能。beta 版终结点中的特性和功能可能会更改；不建议将其用于生产代码中。

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
- `users/{id}` 适用于指定用户（此 URL 中）已与当前用户共享的 OneNote 内容。请使用 [用户](users.md) API。
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

