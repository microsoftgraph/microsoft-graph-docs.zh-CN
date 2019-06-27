---
title: 枚举网站
description: 列出组织中符合提供的筛选条件和查询选项的可用 [sites] []。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b4097d3da8dfa9acf9ab913a1aa1a8cb2326b027
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271545"
---
# <a name="enumerate-sites"></a><span data-ttu-id="043eb-103">枚举网站</span><span class="sxs-lookup"><span data-stu-id="043eb-103">Enumerate sites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="043eb-104">列出组织中符合提供的筛选条件和查询选项的可用[网站][]。</span><span class="sxs-lookup"><span data-stu-id="043eb-104">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="043eb-105">目前仅支持以下查询选项:</span><span class="sxs-lookup"><span data-stu-id="043eb-105">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="043eb-106">Filter 语句</span><span class="sxs-lookup"><span data-stu-id="043eb-106">Filter statement</span></span>             | <span data-ttu-id="043eb-107">Select 语句</span><span class="sxs-lookup"><span data-stu-id="043eb-107">Select statement</span></span>        | <span data-ttu-id="043eb-108">说明</span><span class="sxs-lookup"><span data-stu-id="043eb-108">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="043eb-109">列出组织中的所有根级别网站集。</span><span class="sxs-lookup"><span data-stu-id="043eb-109">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="043eb-110">对于发现每个地理位置的主站点很有用。</span><span class="sxs-lookup"><span data-stu-id="043eb-110">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="043eb-111">此外, 您可以对 "/sites" 集合使用**[搜索][]** 查询来查找与给定关键字匹配的网站。</span><span class="sxs-lookup"><span data-stu-id="043eb-111">In addition, you may use a **[search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[查询]: site-search.md
[search]: site-search.md
[网站]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="043eb-114">权限</span><span class="sxs-lookup"><span data-stu-id="043eb-114">Permissions</span></span>

<span data-ttu-id="043eb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="043eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="043eb-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="043eb-117">Permission type</span></span>                        | <span data-ttu-id="043eb-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="043eb-118">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="043eb-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="043eb-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="043eb-120">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="043eb-120">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="043eb-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="043eb-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="043eb-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="043eb-122">Not supported.</span></span>
|<span data-ttu-id="043eb-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="043eb-123">Application</span></span>                            | <span data-ttu-id="043eb-124">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="043eb-124">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="043eb-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="043eb-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="043eb-126">示例</span><span class="sxs-lookup"><span data-stu-id="043eb-126">Example</span></span>

#### <a name="request"></a><span data-ttu-id="043eb-127">请求</span><span class="sxs-lookup"><span data-stu-id="043eb-127">Request</span></span>

<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```

#### <a name="response"></a><span data-ttu-id="043eb-128">响应</span><span class="sxs-lookup"><span data-stu-id="043eb-128">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="043eb-129">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="043eb-129">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="043eb-130">C#</span><span class="sxs-lookup"><span data-stu-id="043eb-130">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list-sites-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="043eb-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="043eb-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list-sites-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="043eb-132">目标-C</span><span class="sxs-lookup"><span data-stu-id="043eb-132">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/list-sites-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
    "Error: /api-reference/beta/api/site-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/site-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/site-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
