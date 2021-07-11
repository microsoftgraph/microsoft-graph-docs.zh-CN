---
title: Azure AD 目录对象的高级查询功能
description: Azure AD 目录对象支持高级查询功能以高效访问数据。
author: Licantrop0
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 03210e9c46776c4fbc92057870737a87c7e47371
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366513"
---
# <a name="advanced-query-capabilities-on-azure-ad-directory-objects"></a><span data-ttu-id="a0e31-103">Azure AD 目录对象的高级查询功能</span><span class="sxs-lookup"><span data-stu-id="a0e31-103">Advanced query capabilities on Azure AD directory objects</span></span>

<span data-ttu-id="a0e31-104">随着 Azure AD 在稳定性、可用性和性能方面不断提供更多功能和改进，Microsoft Graph 也在不断改进和扩展以便高效访问数据。</span><span class="sxs-lookup"><span data-stu-id="a0e31-104">As Azure AD continues to deliver more capabilities and improvements in stability, availability, and performance, Microsoft Graph also continues to evolve and scale to efficiently access the data.</span></span> <span data-ttu-id="a0e31-105">一个途径是 Microsoft Graph 对各种 Azure AD 对象及其属性的高级查询功能加强支持。</span><span class="sxs-lookup"><span data-stu-id="a0e31-105">One way is through Microsoft Graph's increasing support for advanced query capabilities on various Azure AD objects and their properties.</span></span> <span data-ttu-id="a0e31-106">例如，在 2020 年 10 月，为 `$filter` 查询参数上添加了 **Not** (`NOT`)、**Not equals** (`ne`) 和 **Ends with** (`endsWith`) 运算符。</span><span class="sxs-lookup"><span data-stu-id="a0e31-106">For example, the addition of **Not** (`NOT`), **Not equals** (`ne`), and **Ends with** (`endsWith`) operators on the `$filter` query parameter in October 2020.</span></span>

<span data-ttu-id="a0e31-107">Microsoft Graph 查询引擎使用索引存储来满足查询请求。</span><span class="sxs-lookup"><span data-stu-id="a0e31-107">The Microsoft Graph query engine uses an index store to fulfill query requests.</span></span> <span data-ttu-id="a0e31-108">为了进一步支持某些属性的查询功能，这些属性现在在单独的服务器中编制索引。</span><span class="sxs-lookup"><span data-stu-id="a0e31-108">To add support for additional query capabilities on some properties, these properties are now indexed in a separate server.</span></span> <span data-ttu-id="a0e31-109">这种单独的索引使 Azure AD 可以增加支持并提高查询请求的性能。</span><span class="sxs-lookup"><span data-stu-id="a0e31-109">This separate indexing allows Azure AD to increase support and improve the performance of the query requests.</span></span> <span data-ttu-id="a0e31-110">然而，这些高级查询功能在默认情况下不可用，但是，请求者还必须将 **ConsistencyLevel** 标头设置为 `eventual` *和* (`$search`除外)，并使用 `$count` 查询参数(作为 [URL 段](/graph/query-parameters#other-odata-url-capabilities) 或 `$count=true` 查询字符串)。</span><span class="sxs-lookup"><span data-stu-id="a0e31-110">However, these advanced query capabilities are not available by default but, the requestor must also set the **ConsistencyLevel** header set to `eventual` *and*, with the exception of `$search`, use the `$count` query parameter (either as a [URL segment](/graph/query-parameters#other-odata-url-capabilities) or `$count=true` query string).</span></span> <span data-ttu-id="a0e31-111">**ConsistencyLevel** 标头和`$count`被称为 *高级查询参数*。</span><span class="sxs-lookup"><span data-stu-id="a0e31-111">The **ConsistencyLevel** header and `$count` are referred to as *advanced query parameters*.</span></span>

<span data-ttu-id="a0e31-112">例如，如果只想检索非活动用户帐户，则可以运行使用 `$filter` 查询参数的查询之一。</span><span class="sxs-lookup"><span data-stu-id="a0e31-112">For example, if you wish to retrieve only inactive user accounts, you can run either of these queries that use the `$filter` query parameter.</span></span>

+ <span data-ttu-id="a0e31-113">将 `$filter` 查询参数与 `eq` 运算符一起使用。</span><span class="sxs-lookup"><span data-stu-id="a0e31-113">Use the `$filter` query parameter with the `eq` operator.</span></span> <span data-ttu-id="a0e31-114">默认情况下，此请求将起作用，即请求不需要高级查询参数。</span><span class="sxs-lookup"><span data-stu-id="a0e31-114">This request will work by default, that is, the request does not require the advanced query parameters.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_users_enabled"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=accountEnabled eq false
```

+ <span data-ttu-id="a0e31-115">将 `$filter` 查询参数与 `ne` 运算符一起使用。</span><span class="sxs-lookup"><span data-stu-id="a0e31-115">Use the `$filter` query parameter with the `ne` operator.</span></span> <span data-ttu-id="a0e31-116">默认情况下不支持此请求，因为仅在高级查询中支持 `ne` 运算符。</span><span class="sxs-lookup"><span data-stu-id="a0e31-116">This request is not supported by default because the `ne` operator is only supported in advanced queries.</span></span> <span data-ttu-id="a0e31-117">因此，必须将 **ConsistencyLevel** 标头设置为 `eventual` *并* 使用 `$count=true` 查询字符串。</span><span class="sxs-lookup"><span data-stu-id="a0e31-117">Therefore, you must add the **ConsistencyLevel** header set to `eventual` *and* use the `$count=true` query string.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_users_not_enabled"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=accountEnabled ne true&$count=true
ConsistencyLevel: eventual
```

<span data-ttu-id="a0e31-118">这些高级查询功能仅在 Azure AD 对象上受支持，也就是以下资源及其派生自 [directoryObject](/graph/api/resources/directoryobject) 的关系:</span><span class="sxs-lookup"><span data-stu-id="a0e31-118">These advanced query capabilities are supported only on Azure AD objects, that is, the following resources and their relationships that derive from [directoryObject](/graph/api/resources/directoryobject):</span></span>

- [<span data-ttu-id="a0e31-119">application</span><span class="sxs-lookup"><span data-stu-id="a0e31-119">application</span></span>](/graph/api/resources/application)
- [<span data-ttu-id="a0e31-120">orgContact</span><span class="sxs-lookup"><span data-stu-id="a0e31-120">orgContact</span></span>](/graph/api/resources/orgcontact)
- [<span data-ttu-id="a0e31-121">设备</span><span class="sxs-lookup"><span data-stu-id="a0e31-121">device</span></span>](/graph/api/resources/device)
- [<span data-ttu-id="a0e31-122">组</span><span class="sxs-lookup"><span data-stu-id="a0e31-122">group</span></span>](/graph/api/resources/group)
- [<span data-ttu-id="a0e31-123">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="a0e31-123">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal)
- [<span data-ttu-id="a0e31-124">用户</span><span class="sxs-lookup"><span data-stu-id="a0e31-124">user</span></span>](/graph/api/resources/user)

<span data-ttu-id="a0e31-125">下表列出了仅在高级查询中支持的目录对象的查询方案。</span><span class="sxs-lookup"><span data-stu-id="a0e31-125">The following table lists query scenarios on directory objects that are supported only in advanced queries.</span></span>

| <span data-ttu-id="a0e31-126">说明</span><span class="sxs-lookup"><span data-stu-id="a0e31-126">Description</span></span>                                                              | <span data-ttu-id="a0e31-127">示例</span><span class="sxs-lookup"><span data-stu-id="a0e31-127">Example</span></span>                                                                                                                                                                                                                                                                                                                                                                                                                              |
|:-------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a0e31-128">使用 `$count` 作为 URL 段</span><span class="sxs-lookup"><span data-stu-id="a0e31-128">Use of `$count` as a URL segment</span></span>                                         | <span data-ttu-id="a0e31-129">[GET](https://developer.microsoft.com/graph/graph-explorer?request=groups%2F%24count&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups/$count`</span><span class="sxs-lookup"><span data-stu-id="a0e31-129">[GET](https://developer.microsoft.com/graph/graph-explorer?request=groups%2F%24count&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups/$count`</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="a0e31-130">使用 `$count` 作为查询字符串参数</span><span class="sxs-lookup"><span data-stu-id="a0e31-130">Use of `$count` as a query string parameter</span></span>                              | <span data-ttu-id="a0e31-131">[GET](https://developer.microsoft.com/graph/graph-explorer?request=servicePrincipals%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../servicePrincipals?$count=true`</span><span class="sxs-lookup"><span data-stu-id="a0e31-131">[GET](https://developer.microsoft.com/graph/graph-explorer?request=servicePrincipals%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../servicePrincipals?$count=true`</span></span>                                                                                                                                                     |
| <span data-ttu-id="a0e31-132">使用 `$search`</span><span class="sxs-lookup"><span data-stu-id="a0e31-132">Use of `$search`</span></span>                                                         | <span data-ttu-id="a0e31-133">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24search%3D%22displayName%3ABrowser%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$search="displayName:Browser"`</span><span class="sxs-lookup"><span data-stu-id="a0e31-133">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24search%3D%22displayName%3ABrowser%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$search="displayName:Browser"`</span></span>                                                                                                                     |
| <span data-ttu-id="a0e31-134">对选择属性使用 `$orderby`</span><span class="sxs-lookup"><span data-stu-id="a0e31-134">Use of `$orderby` on select properties</span></span>                                   | <span data-ttu-id="a0e31-135">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$count=true`</span><span class="sxs-lookup"><span data-stu-id="a0e31-135">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$count=true`</span></span>                                                                                                               |
| <span data-ttu-id="a0e31-136">将 `$filter` 与 `endsWith` 运算符结合使用</span><span class="sxs-lookup"><span data-stu-id="a0e31-136">Use of `$filter` with the `endsWith` operator</span></span>                            | <span data-ttu-id="a0e31-137">[GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40outlook.com')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@outlook.com')`</span><span class="sxs-lookup"><span data-stu-id="a0e31-137">[GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40outlook.com')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@outlook.com')`</span></span>                                                                                       |
| <span data-ttu-id="a0e31-138">在同一查询中使用`$filter`和`$orderby`</span><span class="sxs-lookup"><span data-stu-id="a0e31-138">Use of `$filter` and `$orderby` in the same query</span></span>                        | <span data-ttu-id="a0e31-139">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24filter%3DstartsWith(displayName%2C%20'Box')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$filter=startsWith(displayName, 'Box')&$count=true`</span><span class="sxs-lookup"><span data-stu-id="a0e31-139">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24filter%3DstartsWith(displayName%2C%20'Box')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$filter=startsWith(displayName, 'Box')&$count=true`</span></span>                       |
| <span data-ttu-id="a0e31-140">对特定属性将 `$filter` 与 `startsWith` 运算符结合使用.</span><span class="sxs-lookup"><span data-stu-id="a0e31-140">Use of `$filter` with the `startsWith` operators on specific properties.</span></span> | <span data-ttu-id="a0e31-141">[GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24filter%3DstartsWith(mobilePhone%2C%20'25478')%20OR%20startsWith(mobilePhone%2C%20'25473')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=startsWith(mobilePhone, '25478') OR startsWith(mobilePhone, '25473')&$count=true`</span><span class="sxs-lookup"><span data-stu-id="a0e31-141">[GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24filter%3DstartsWith(mobilePhone%2C%20'25478')%20OR%20startsWith(mobilePhone%2C%20'25473')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=startsWith(mobilePhone, '25478') OR startsWith(mobilePhone, '25473')&$count=true`</span></span> |
| <span data-ttu-id="a0e31-142">将 `$filter` 与 `ne` 和 `NOT` 运算符结合使用</span><span class="sxs-lookup"><span data-stu-id="a0e31-142">Use of `$filter` with `ne` and `NOT` operators</span></span>                           | <span data-ttu-id="a0e31-143">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`</span><span class="sxs-lookup"><span data-stu-id="a0e31-143">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`</span></span>                     |
| <span data-ttu-id="a0e31-144">将 `$filter` 与 `NOT` 和 `startsWith` 运算符结合使用</span><span class="sxs-lookup"><span data-stu-id="a0e31-144">Use of `$filter` with `NOT` and `startsWith` operators</span></span>                   | <span data-ttu-id="a0e31-145">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=%2Fusers%3F%24filter%3DNOT%20startsWith(displayName%2C%20'Conf')%26%24count%3Dtrue&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=NOT startsWith(displayName, 'Conf')&$count=true`</span><span class="sxs-lookup"><span data-stu-id="a0e31-145">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=%2Fusers%3F%24filter%3DNOT%20startsWith(displayName%2C%20'Conf')%26%24count%3Dtrue&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=NOT startsWith(displayName, 'Conf')&$count=true`</span></span>                                                                |
| <span data-ttu-id="a0e31-146">将 OData 强制转换与其他查询参数一起使用</span><span class="sxs-lookup"><span data-stu-id="a0e31-146">Use of OData cast with another query parameter</span></span>                           | <span data-ttu-id="a0e31-147">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true`</span><span class="sxs-lookup"><span data-stu-id="a0e31-147">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true`</span></span>                                                                                             |

> [!NOTE]
> <span data-ttu-id="a0e31-148">这些高级查询功能在 Azure AD B2C 租户中不可用。</span><span class="sxs-lookup"><span data-stu-id="a0e31-148">These advanced query capabilities are not available in Azure AD B2C tenants.</span></span>

## <a name="support-for-filter-on-properties-of-azure-ad-directory-objects"></a><span data-ttu-id="a0e31-149">支持筛选 Azure AD 目录对象的属性</span><span class="sxs-lookup"><span data-stu-id="a0e31-149">Support for filter on properties of Azure AD directory objects</span></span>

<span data-ttu-id="a0e31-150">目录对象的属性对查询参数的支持行为各不相同。</span><span class="sxs-lookup"><span data-stu-id="a0e31-150">Properties of directory objects behave differently in their support for query parameters.</span></span> <span data-ttu-id="a0e31-151">以下是目录对象的常见应用场景:</span><span class="sxs-lookup"><span data-stu-id="a0e31-151">The following are common scenarios for directory objects:</span></span>

+ <span data-ttu-id="a0e31-152">除另有指示外，跨目录资源的同名属性支持相同的 `$filter` 运算符。</span><span class="sxs-lookup"><span data-stu-id="a0e31-152">Unless otherwise indicated, properties with the same name across directory resources support the same `$filter` operators.</span></span> <span data-ttu-id="a0e31-153">例如，**application**、**group**、**organization** 和 **user** 资源中提供了 **createdDateTime** 属性。</span><span class="sxs-lookup"><span data-stu-id="a0e31-153">For example, the **createdDateTime** property is available in **application**, **group**, **organization**, and **user** resources.</span></span> <span data-ttu-id="a0e31-154">默认情况下，它支持 `eq`、 `ge`和 `le` 运算符，并且仅在高级查询中支持 `in`、 `ne`和 `NOT` 运算符。</span><span class="sxs-lookup"><span data-stu-id="a0e31-154">It supports the `eq`, `ge`, and `le` operators by default and the `in`, `ne`, and `NOT` operators only in advanced queries.</span></span>
+ <span data-ttu-id="a0e31-155">仅有 **mail** 和 **userPrincipalName** 属性支持`endsWith`运算符。</span><span class="sxs-lookup"><span data-stu-id="a0e31-155">The `endsWith` operator is supported only on **mail** and **userPrincipalName** properties.</span></span>
+ <span data-ttu-id="a0e31-156">默认情况下支持的查询也适用于高级查询。</span><span class="sxs-lookup"><span data-stu-id="a0e31-156">Queries that are supported by default will also work in advanced queries.</span></span>
+ <span data-ttu-id="a0e31-157">仅在高级查询中支持 `NOT` 和 `ne` 求反运算符。</span><span class="sxs-lookup"><span data-stu-id="a0e31-157">The `NOT` and `ne` negation operators are supported only in advanced queries.</span></span> 
  + <span data-ttu-id="a0e31-158">支持 `eq` 运算符的所有属性也支持 `ne` 或 `NOT` 运算符。</span><span class="sxs-lookup"><span data-stu-id="a0e31-158">All properties that support the `eq` operator also support the `ne` or `NOT` operators.</span></span>
  + <span data-ttu-id="a0e31-159">当`eq`运算符的计算结果为 `true`时，`ne`运算符求反。</span><span class="sxs-lookup"><span data-stu-id="a0e31-159">The `ne` operator negates where the `eq` operator would otherwise evaluate to `true`.</span></span> <span data-ttu-id="a0e31-160">对于使用 `any` lambda 运算符的查询，请使用 `NOT` 运算符。</span><span class="sxs-lookup"><span data-stu-id="a0e31-160">For queries that use the `any` lambda operator, use the `NOT` operator.</span></span> <span data-ttu-id="a0e31-161">请参阅[使用 lambda 运算符的筛选器](/graph/query-parameters#filter-using-lambda-operators)。</span><span class="sxs-lookup"><span data-stu-id="a0e31-161">See [Filter using lambda operators](/graph/query-parameters#filter-using-lambda-operators).</span></span>

<span data-ttu-id="a0e31-162">下表汇总了[users](/graph/api/resources/user)目录对象的属性对`$filter`运算符的支持。</span><span class="sxs-lookup"><span data-stu-id="a0e31-162">The following table summarizes support for `$filter` operators by properties on the [users](/graph/api/resources/user) directory object.</span></span>

- <span data-ttu-id="a0e31-163">![默认情况下有效。</span><span class="sxs-lookup"><span data-stu-id="a0e31-163">![Works by default.</span></span> <span data-ttu-id="a0e31-164">不需要高级查询参数。](/graph/images/advanced-query-parameters/default.png)</span><span class="sxs-lookup"><span data-stu-id="a0e31-164">Does not require advanced query parameters.](/graph/images/advanced-query-parameters/default.png)</span></span> <span data-ttu-id="a0e31-165">默认情况下，该属性支持`$filter`使用运算符。</span><span class="sxs-lookup"><span data-stu-id="a0e31-165">The property supports `$filter` with the operator by default.</span></span>
- <span data-ttu-id="a0e31-166">![需要高级查询参数。](/graph/images/advanced-query-parameters/advanced.png)</span><span class="sxs-lookup"><span data-stu-id="a0e31-166">![Requires advanced query parameters.](/graph/images/advanced-query-parameters/advanced.png)</span></span> <span data-ttu-id="a0e31-167">特定的 `$filter` 运算符需要 *高级查询参数*:</span><span class="sxs-lookup"><span data-stu-id="a0e31-167">The specific `$filter` operator requires *advanced query parameters*:</span></span>
  - <span data-ttu-id="a0e31-168">`ConsistencyLevel=eventual` 标头</span><span class="sxs-lookup"><span data-stu-id="a0e31-168">`ConsistencyLevel=eventual` header</span></span>
  - <span data-ttu-id="a0e31-169">`$count=true` 查询字符串</span><span class="sxs-lookup"><span data-stu-id="a0e31-169">`$count=true` query string</span></span>
- <span data-ttu-id="a0e31-170">空白单元格表示该属性不支持 `$filter` 使用运算符。</span><span class="sxs-lookup"><span data-stu-id="a0e31-170">Blank cells indicate that the property does not support the use of `$filter` with the operator.</span></span>
- <span data-ttu-id="a0e31-171">**null value** 列表明属性可根据 `null` 值进行筛选。</span><span class="sxs-lookup"><span data-stu-id="a0e31-171">The **null values** column indicates that the property is filterable on `null` values.</span></span>
- <span data-ttu-id="a0e31-172">此处未列出的属性不支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="a0e31-172">Properties that are not listed here do not support `$filter`.</span></span>

[!INCLUDE [filter-directory-objects](../includes/filter-directory-objects.md)]


## <a name="error-handling-for-advanced-queries-on-directory-objects"></a><span data-ttu-id="a0e31-173">针对目录对象的高级查询的错误处理</span><span class="sxs-lookup"><span data-stu-id="a0e31-173">Error handling for advanced queries on directory objects</span></span>

<span data-ttu-id="a0e31-174">仅支持使用高级查询参数对目录对象进行计数。</span><span class="sxs-lookup"><span data-stu-id="a0e31-174">Counting directory objects is only supported using the advanced queries parameters.</span></span> <span data-ttu-id="a0e31-175">如果未指定 `ConsistencyLevel=eventual` 标头，则在使用 `$count` URL 段时，请求将返回错误或以无提示方式忽略 `$count` 查询参数(`?$count=true`)。</span><span class="sxs-lookup"><span data-stu-id="a0e31-175">If the `ConsistencyLevel=eventual` header is not specified, the request returns an error when the `$count` URL segment is used or silently ignores the `$count` query parameter (`?$count=true`) if it's used.</span></span>

```http
https://graph.microsoft.com/v1.0/users/$count
```

```json
{
    "error": {
        "code": "Request_BadRequest",
        "message": "$count is not currently supported.",
        "innerError": {
            "date": "2021-05-18T19:03:10",
            "request-id": "d9bbd4d8-bb2d-44e6-99a1-71a9516da744",
            "client-request-id": "539da3bd-942f-25db-636b-27f6f6e8eae4"
        }
    }
}
```

<span data-ttu-id="a0e31-176">派生自 [directoryObject](/graph/api/resources/directoryobject)的 Azure AD 资源中的`$search`仅适用于高级查询。</span><span class="sxs-lookup"><span data-stu-id="a0e31-176">`$search` on Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject) works only in advanced queries.</span></span> <span data-ttu-id="a0e31-177">如果未指定 **ConsistencyLevel** 标头，则请求将返回错误。</span><span class="sxs-lookup"><span data-stu-id="a0e31-177">If the **ConsistencyLevel** header is not specified, the request returns an error.</span></span>

```http
https://graph.microsoft.com/v1.0/applications?$search="displayName:Browser"
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "Request with $search query parameter only works through MSGraph with a special request header: 'ConsistencyLevel: eventual'",
        "innerError": {
            "date": "2021-05-27T14:26:47",
            "request-id": "9b600954-ba11-4899-8ce9-6abad341f299",
            "client-request-id": "7964ef27-13a3-6ca4-ed7b-73c271110867"
        }
    }
}
```

<span data-ttu-id="a0e31-178">如果 URL 中的属性或查询参数仅在高级查询中受支持，但缺少 **ConsistencyLevel** 标头或 `$count=true` 查询字符串，则请求将返回错误。</span><span class="sxs-lookup"><span data-stu-id="a0e31-178">If a property or query parameter in the URL is supported only in advanced queries but either the **ConsistencyLevel** header or the `$count=true` query string is missing, the request returns an error.</span></span>

```http
https://graph.microsoft.com/beta/users?$filter=endsWith(mail,'@outlook.com')
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "Unsupported Query.",
        "innerError": {
            "date": "2021-05-18T19:12:36",
            "request-id": "63f2093c-399c-4350-9609-3ce9b62abe3c",
            "client-request-id": "e60ed0ba-df5d-e190-f056-f9c0318456d7"
        }
    }
}
```

<span data-ttu-id="a0e31-179">如果尚未为某个属性编制索引以支持查询参数，即使指定了高级查询参数，请求也将返回错误。</span><span class="sxs-lookup"><span data-stu-id="a0e31-179">If a property has not been indexed to support a query parameter, even if the advanced query parameters are specified, the request returns an error.</span></span>

```http
https://graph.microsoft.com/v1.0/users?$filter=id ge '398164b1-5196-49dd-ada2-364b49f99b27'&$count=true
ConsistencyLevel: eventual
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "The request uses a filter property that is not indexed",
        "innerError": {
            "date": "2021-06-10T19:32:01",
            "request-id": "5625ba13-0c9f-4fce-a853-4b52f3e0bd09",
            "client-request-id": "76fe4cd8-df3a-f8c3-659b-594274b6bb31"
        }
    }
}
```

<span data-ttu-id="a0e31-180">但是，值得注意的是请求中指定的查询参数可能会自行失败。</span><span class="sxs-lookup"><span data-stu-id="a0e31-180">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="a0e31-181">不支持的查询参数以及不支持的查询参数组合的情况就是如此。</span><span class="sxs-lookup"><span data-stu-id="a0e31-181">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="a0e31-182">在这些情况下，应检查请求返回的数据，以确定指定的查询参数是否具有所需的效果。</span><span class="sxs-lookup"><span data-stu-id="a0e31-182">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> <span data-ttu-id="a0e31-183">例如，在下面的示例中，即使查询成功， `@odata.count` 参数也缺失。</span><span class="sxs-lookup"><span data-stu-id="a0e31-183">For example, in the following example, the `@odata.count` parameter is missing even if the query is successful.</span></span>

```http
https://graph.microsoft.com/v1.0/users?$count=true
```

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "value":[
    {
      "displayName":"Oscar Ward",
      "mail":"oscarward@contoso.com",
      "userPrincipalName":"oscarward@contoso.com"
    },
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="a0e31-184">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a0e31-184">See also</span></span>

- [<span data-ttu-id="a0e31-185">使用查询参数自定义响应</span><span class="sxs-lookup"><span data-stu-id="a0e31-185">Use query parameters to customize responses</span></span>](/graph/query-parameters)
- [<span data-ttu-id="a0e31-186">查询参数限制</span><span class="sxs-lookup"><span data-stu-id="a0e31-186">Query parameter limitations</span></span>](known-issues.md#query-parameter-limitations)
- [<span data-ttu-id="a0e31-187">使用$search查询参数匹配搜索条件</span><span class="sxs-lookup"><span data-stu-id="a0e31-187">Use the $search query parameter to match a search criterion</span></span>](/graph/search-query-parameter)
