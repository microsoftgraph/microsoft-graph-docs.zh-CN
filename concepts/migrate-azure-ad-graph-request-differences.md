---
title: 请求 Azure AD Graph 和 Microsoft Graph 之间的差异
description: 介绍 Microsoft Graph 请求与 Azure AD 请求的不同之处，这有助于将应用迁移到较新的服务。。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8130daf4037e6ef1a433ca537a8fecec996a34ce
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845906"
---
# <a name="request-differences-between-azure-ad-graph-and-microsoft-graph"></a>请求 Azure AD Graph 和 Microsoft Graph 之间的差异

本文是*第1步：查看*[迁移应用程序](migrate-azure-ad-graph-planning-checklist.md)的 API 差异的过程的一部分。

Microsoft Graph 和 Azure AD Graph API 都是 REST Api，它们分别支持查询参数的 ODATA 约定。 但是，这两个 Api 的语法各不相同。

使用[Graph 浏览器](https://aka.ms/ge)针对您自己的数据尝试这些请求模式，因为这是了解请求和响应差异的一种很好的方法。

## <a name="basic-requests"></a>基本请求

下表突出显示了这两个 Api 之间的主要请求差异：

|请求详细信息| Azure AD Graph | Microsoft Graph |
|---|---|---|
|请求语法| `https://graph.windows.net/{tenant_id}/` <br> `{resource}?{version}&query-parameters` | `https://graph.microsoft.com/`<br>`{version}/{resource}?query-parameters`|
|服务 &nbsp; 终结点：||
|-&nbsp;全局性|`https://graph.windows.net`|`https://graph.microsoft.com`|
|-&nbsp;US &nbsp; .Gov &nbsp; L4|`https://graph.microsoftazure.us`|`https://graph.microsoft.us`|
|-&nbsp;美国 &nbsp; .Gov &nbsp; L5 &nbsp; （DOD）|`https://graph.microsoftazure.us`|`https://dod-graph.microsoft.us`|
|-&nbsp;德国|`https://graph.cloudapi.de`|`https://graph.microsoft.de`|
|-&nbsp;中国 &nbsp; （世纪）| `https://graph.chinacloudapi.cn`|`https://microsoftgraph.chinacloudapi.cn`|
|{tenant_id}|指定请求中租户的 ID。|在请求中指定的租户 ID 是可从访问令牌推断出的可选方法。<br><br>如果您指定租户 ID，它将在 `{version}` `{resource}` 请求 URL 中的和之间。|
|版本|使用所需的查询参数在请求中指定 Azure AD Graph 的发布版本。|在请求中将 Microsoft Graph 的发布版本指定为服务终结点之后的 URL 路径的一部分。|

您可以继续在 Microsoft Graph 中使用与 Azure AD Graph 相同的查询参数。

### <a name="example-request-comparison"></a>示例请求比较

假设您需要一个名称以 "Dan" 开头的所有用户的列表。

在 Azure AD Graph 中，可以使用此请求：

`https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6`

此请求：

- 面向 Azure AD Graph 的版本1.6。
- 指定 `contoso.com` 为租户 ID。
- 调用用户资源。
- 使用 `$filter` 查询参数将响应限制为以开头的给定名称 `Dan` 。

结果包括名称如 Daniel、Danforth、Danielle、Danerys 等的用户。

Microsoft Graph 的类似请求如下：

`https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName,'Dan')`

如下

- 版本为 `v1.0` 。
- 租户 ID 是从访问令牌推断出的（未显示）。
- 资源和 `$filter` 查询参数与 AZURE AD 查询相同。

> **注意**：如果使用的是 Azure AD Graph .net 客户端库，请参阅[.net 客户端库](migrate-azure-ad-graph-client-libraries.md)，了解更多特定策略和帮助，以移动到 Microsoft Graph .net 客户端库。

### <a name="key-identifiers-objectid-vs-id"></a>键标识符： objectId vs id

在 Azure AD Graph 中，所有实体资源类型都具有一个名为**objectId**的唯一标识符（或键）。  大多数情况（除非另有说明）此同一标识符在 Microsoft Graph 中称为**id** 。

## <a name="default-properties-and-select"></a>默认属性和 $select

使用 `$select` GET requests 中的查询参数自定义响应，以包含您的应用程序所需的所有属性。

Microsoft Graph **get**或**list**操作对于用户或组资源，仅返回所有属性（称为_默认属性_）的子集。 默认属性表示资源的最常用属性。 另一方面，Azure AD Graph 将返回相应资源的所有属性的完整集。

若要获取 v1.0 中的其他属性，应用需要使用查询参数显式请求这些属性 `$select` 。 这包括您的应用程序可能使用的任何目录架构扩展。 最佳做法是仅请求应用程序真正需要的属性。

为了说明区别，请使用 Graph 浏览器运行以下请求并比较不同的响应。

```http
GET https://graph.microsoft.com/v1.0/me/
GET https://graph.microsoft.com/beta/me/
```

查看每个查询的响应。 您会注意到，地址信息是由/beta 版本（而不是/v1.0 版本）返回的。  这是因为地址属性不在默认属性集中。

如果您的应用程序依赖于地址属性，则需要更新您的 v1.0 请求以包含 `$select` 查询参数：

```http
https://graph.microsoft.com/v1.0/me/?$select=displayName,streetAddress,city,state,postalCode
```

此请求的响应将包括地址属性。  它还包括**displayName**属性，但仅由于它是由查询参数指定的。

若要了解详细信息，请参阅：

- 用户的默认属性，请参阅[users](/graph/api/resources/users?view=graph-rest-1.0)
- `$select`参数和其他受支持的 ODATA 查询参数，请参阅[使用查询参数自定义响应](/graph/query-parameters)。
- 此操作和其他建议的优化，请参阅[最佳实践](/graph/best-practices-concept)。

## <a name="relationships-and-navigation-properties"></a>关系和导航属性

关系（或导航属性）是 Azure AD Graph 和 Microsoft Graph 中的关键概念，创建了相关资源的网络。 例如， **manager**和**directReports**属性扩展了用户资源，以提供组织的层次结构。

关系还定义成员身份，如用户所属的组、属于某个组的成员或目录角色，等等。

Azure AD Graph 请求用于 `$link` 指示资源之间的关系。  在 Microsoft Graph 中，使用的是 ODATA 4.01 `$ref` 表示法。

下表显示了几个示例：

| Task | Azure AD Graph | Microsoft Graph |
|------|----------------|-----------------|
| 添加成员        | ```POST /groups/{id}/$link/members```        | ```POST /groups/{id}/members/$ref```        |
| 列出成员链接 | ```GET /groups/{id}/$link/members```         | ```GET /groups/{id}/members/$ref```         |
| 列出成员      | ```GET /groups/{id}/members```                | ```GET /groups/{id}/members```               |
| 删除成员     | ```DELETE /groups/{id}/$link/members/{id}``` | ```DELETE /groups/{id}/members/{id}/$ref``` |

将应用程序迁移到 Microsoft Graph 时，请查找使用 `$link` 关联资源的请求; 请将这些请求更改为改用 `$ref` 。

## <a name="next-steps"></a>后续步骤

- 了解 Azure AD Graph 与 Microsoft Graph 之间的[服务功能差异](migrate-azure-ad-graph-feature-differences.md)。
- 浏览[Microsoft Graph](/graph/overview)概念和实践。
- 使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。
