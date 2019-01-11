---
title: 枚举网站
description: 列出组织中的匹配提供的筛选器条件和查询选项可用 [站点] []。
localization_priority: Normal
ms.openlocfilehash: 87ce5b68ccadffa6e0422c413ab79ee784f361c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855816"
---
# <a name="enumerate-sites"></a><span data-ttu-id="4da7a-103">枚举网站</span><span class="sxs-lookup"><span data-stu-id="4da7a-103">Enumerate sites</span></span>

> <span data-ttu-id="4da7a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4da7a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4da7a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4da7a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4da7a-106">列出与提供的筛选器条件匹配并查询选项的组织中可用的[网站][]。</span><span class="sxs-lookup"><span data-stu-id="4da7a-106">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="4da7a-107">当前支持仅以下查询选项：</span><span class="sxs-lookup"><span data-stu-id="4da7a-107">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="4da7a-108">筛选语句</span><span class="sxs-lookup"><span data-stu-id="4da7a-108">Filter statement</span></span>             | <span data-ttu-id="4da7a-109">Select 语句</span><span class="sxs-lookup"><span data-stu-id="4da7a-109">Select statement</span></span>        | <span data-ttu-id="4da7a-110">Description</span><span class="sxs-lookup"><span data-stu-id="4da7a-110">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="4da7a-111">列出组织中的所有根级别网站集。</span><span class="sxs-lookup"><span data-stu-id="4da7a-111">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="4da7a-112">用于发现每个地理位置的主网站。</span><span class="sxs-lookup"><span data-stu-id="4da7a-112">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="4da7a-113">此外，您可能使用针对 / 网站集合的**[搜索][]** 查询查找匹配关键字给定的网站。</span><span class="sxs-lookup"><span data-stu-id="4da7a-113">In addition, you may use a **[search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[搜索]: site-search.md
[search]: site-search.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="4da7a-116">权限</span><span class="sxs-lookup"><span data-stu-id="4da7a-116">Permissions</span></span>

<span data-ttu-id="4da7a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4da7a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4da7a-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="4da7a-119">Permission type</span></span>                        | <span data-ttu-id="4da7a-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4da7a-120">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="4da7a-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4da7a-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="4da7a-122">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4da7a-122">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="4da7a-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4da7a-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4da7a-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="4da7a-124">Not supported.</span></span>
|<span data-ttu-id="4da7a-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="4da7a-125">Application</span></span>                            | <span data-ttu-id="4da7a-126">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4da7a-126">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="4da7a-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4da7a-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="4da7a-128">示例</span><span class="sxs-lookup"><span data-stu-id="4da7a-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4da7a-129">请求</span><span class="sxs-lookup"><span data-stu-id="4da7a-129">Request</span></span>

<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```

#### <a name="response"></a><span data-ttu-id="4da7a-130">响应</span><span class="sxs-lookup"><span data-stu-id="4da7a-130">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Contoso USA",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com",
        "dataLocationCode": "NAM",
        "root": { }
      },
      "webUrl": "https://contoso.sharepoint.com"
    },
    {
      "id": "contoso-jpn.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Contoso Japan",
      "root": { },
      "siteCollection": {
        "hostname": "contoso-jp.sharepoint.com",
        "dataLocationCode": "JPN",
        "root": { }
      },
      "webUrl": "https://contoso-jp.sharepoint.com"
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites"
} -->
