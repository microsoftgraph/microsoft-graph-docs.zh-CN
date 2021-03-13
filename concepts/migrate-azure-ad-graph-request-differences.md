---
title: 请求 Azure AD Graph 和 Microsoft Graph 之间的差异
description: 介绍 Microsoft Graph 请求与 Azure AD 请求的区别，这有助于将应用迁移到较新的服务。
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: e30a0c98aaf7ec0d042787f511872d02529aaa5c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760663"
---
# <a name="request-differences-between-azure-ad-graph-and-microsoft-graph"></a>请求 Azure AD Graph 和 Microsoft Graph 之间的差异

本文是步骤 *1：查看迁移应用的* 过程的 API [差异的一部分](migrate-azure-ad-graph-planning-checklist.md)。

Microsoft Graph 和 Azure AD Graph API 都是 REST API，它们各自支持查询参数的 ODATA 约定。 但是，语法因这两个 API 而异。

使用 [Graph 浏览器](https://aka.ms/ge) 针对你自己的数据尝试这些请求模式，因为它是了解请求和响应差异的一种很好的方法。

## <a name="basic-requests"></a>基本请求

下表突出显示了两个 API 之间的主要请求差异：

|请求详细信息| Azure AD Graph | Microsoft Graph |
|---|---|---|
|请求语法| `https://graph.windows.net/{tenant_id}/` <br> `{resource}?{version}&query-parameters` | `https://graph.microsoft.com/`<br>`{version}/{resource}?query-parameters`|
|服务 &nbsp; 终结点：||
|-&nbsp;全局|`https://graph.windows.net`|`https://graph.microsoft.com`|
|-&nbsp;美国 &nbsp; Gov &nbsp; L4|`https://graph.microsoftazure.us`|`https://graph.microsoft.us`|
|-&nbsp;美国 &nbsp; Gov &nbsp; L5 &nbsp; (DOD) |`https://graph.microsoftazure.us`|`https://dod-graph.microsoft.us`|
|-&nbsp;德国|`https://graph.cloudapi.de`|`https://graph.microsoft.de`|
|-&nbsp;中国 &nbsp; (世纪) | `https://graph.chinacloudapi.cn`|`https://microsoftgraph.chinacloudapi.cn`|
|{tenant_id}|在请求中指定租户的 ID。|可以选择在请求中指定租户 ID，因为这是从访问令牌推断出来的。<br><br>如果指定租户 ID，它将在 请求 URL 中的 `{version}` `{resource}` 和 之间。|
|{version}|使用必需的查询参数在请求中指定 Azure AD Graph 的发布版本。|在请求中指定 Microsoft Graph 的发布版本作为 URL 路径的一部分，就在服务终结点之后。|

可以在 Microsoft Graph 中继续使用与 Azure AD Graph 相同的查询参数。

### <a name="example-request-comparison"></a>示例请求比较

假设您需要一个名称以"Dan"开头的所有用户的列表。

在 Azure AD Graph 中，可以使用此请求：

`GET https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6` 或 

`GET https://graph.windows.net/myOrganization/users?$filter=startswith(givenName,'Dan')&api-version=1.6`


此请求：

- 面向 Azure AD Graph 版本 1.6。
- 指定为 `contoso.com` 租户 ID。 替代项显示根据访问 `myOrganization` 令牌中的租户 ID 使用别名。
- 调用 users 资源。
- 使用 `$filter` query 参数将响应限制为以 开头的给定名称 `Dan` 。

结果包括用户名为 Daniel、Danforth、Danielle、Danerys 等的用户。

对 Microsoft Graph 的类似请求是：

`GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName,'Dan')`

此处：

- 版本为 `v1.0` 。
- 租户 ID 从访问令牌推断 (未) 。
- resource 和 `$filter` query 参数与 Azure AD 查询相同。

> **注意**：如果你使用的是 Azure AD Graph .NET 客户端库，请参阅 [.NET](migrate-azure-ad-graph-client-libraries.md) 客户端库，了解更具体的策略和移动到 Microsoft Graph .NET 客户端库的帮助。

### <a name="key-identifiers-objectid-vs-id"></a>密钥标识符：objectId 与 id

在 Azure AD Graph 中，所有实体资源类型都有一个唯一标识符 (或密钥) **objectId**。  大多数情况下， (除非另有) 在 Microsoft Graph 中称为 **id。**

## <a name="default-properties-and-select"></a>默认属性和$select

在 `$select` GET 请求中，使用查询参数自定义响应以包含应用需要的所有属性。

用户 **或** 组 **资源的** Microsoft Graph 获取或列表操作仅返回所有属性的子集，称为 _默认属性_。 默认属性表示资源最常用的属性。 另一方面，Azure AD Graph 返回相应资源的所有属性的完整集。

若要获取 v1.0 中的其他属性，你的应用需要使用查询参数显式请求 `$select` 它们。 这包括你的应用可能使用的任何目录架构扩展。 最佳做法是仅请求应用真正需要的属性。

为了说明这一区别，请使用 Graph 浏览器运行以下请求并比较不同的响应。

```http
GET https://graph.microsoft.com/v1.0/me/
GET https://graph.microsoft.com/beta/me/
```

查看每个查询的响应。 你会注意到地址信息由 /beta 版本而不是 /v1.0 版本返回。  这是因为地址属性不在默认属性集内。

如果你的应用依赖于地址属性，则需要更新 v1.0 请求以包含 `$select` 查询参数：

```http
https://graph.microsoft.com/v1.0/me/?$select=displayName,streetAddress,city,state,postalCode
```

此请求的响应将包括地址属性。  它还包括 **displayName** 属性，但仅仅是因为它由查询参数指定。

若要了解有关：

- 用户的默认属性，请参阅 [用户](/graph/api/resources/users?view=graph-rest-1.0)
- 参数 `$select` 和其他支持的 ODATA 查询参数，请参阅使用 [查询参数自定义响应](./query-parameters.md)。
- 这和其他建议的优化，请参阅 [最佳做法](./best-practices-concept.md)。

## <a name="relationships-and-navigation-properties"></a>关系和导航属性

关系 (或导航) 是 Azure AD Graph 和 Microsoft Graph 中的关键概念，用于创建相关资源网络。 例如 **，manager 和** **directReports** 属性扩展用户资源以提供组织层次结构。

关系还定义成员身份，如用户所属的组、属于组或目录角色的成员等。

Azure AD Graph 请求 `$link` 用于指示资源之间的关系。  在 Microsoft Graph 中，它改为使用 ODATA 4.01 `$ref` 表示法。

下表显示了几个示例：

| 任务 | Azure AD Graph | Microsoft Graph |
|------|----------------|-----------------|
| 添加成员        | ```POST /groups/{id}/$link/members```        | ```POST /groups/{id}/members/$ref```        |
| 列出成员链接 | ```GET /groups/{id}/$link/members```         | ```GET /groups/{id}/members/$ref```         |
| 列出成员      | ```GET /groups/{id}/members```                | ```GET /groups/{id}/members```               |
| 删除成员     | ```DELETE /groups/{id}/$link/members/{id}``` | ```DELETE /groups/{id}/members/{id}/$ref``` |

将应用迁移到 Microsoft Graph 时，查找用于关联资源的请求; `$link` 将其更改为 `$ref` 使用。

## <a name="next-steps"></a>后续步骤

- 了解 Azure AD Graph [和](migrate-azure-ad-graph-feature-differences.md) Microsoft Graph 之间的服务功能差异。
- 再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。