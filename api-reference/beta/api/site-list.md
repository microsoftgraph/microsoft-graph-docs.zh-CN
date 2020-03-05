---
title: 枚举网站
description: 列出组织中符合提供的筛选条件和查询选项的可用 [sites] []。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: ''
ms.openlocfilehash: 266f88af6b71317b271bec5ede1d2984d4e704fa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453210"
---
# <a name="enumerate-sites"></a><span data-ttu-id="e6ad6-103">枚举网站</span><span class="sxs-lookup"><span data-stu-id="e6ad6-103">Enumerate sites</span></span>

<span data-ttu-id="e6ad6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e6ad6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6ad6-105">列出组织中符合提供的筛选条件和查询选项的可用[网站][]。</span><span class="sxs-lookup"><span data-stu-id="e6ad6-105">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="e6ad6-106">目前仅支持以下查询选项：</span><span class="sxs-lookup"><span data-stu-id="e6ad6-106">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="e6ad6-107">Filter 语句</span><span class="sxs-lookup"><span data-stu-id="e6ad6-107">Filter statement</span></span>             | <span data-ttu-id="e6ad6-108">Select 语句</span><span class="sxs-lookup"><span data-stu-id="e6ad6-108">Select statement</span></span>        | <span data-ttu-id="e6ad6-109">说明</span><span class="sxs-lookup"><span data-stu-id="e6ad6-109">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="e6ad6-110">列出组织中的所有根级别网站集。</span><span class="sxs-lookup"><span data-stu-id="e6ad6-110">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="e6ad6-111">对于发现每个地理位置的主站点很有用。</span><span class="sxs-lookup"><span data-stu-id="e6ad6-111">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="e6ad6-112">此外，您可以对 "/sites" 集合使用**[$search][]** 查询，以查找与给定关键字匹配的网站。</span><span class="sxs-lookup"><span data-stu-id="e6ad6-112">In addition, you may use a **[$search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[$search]: site-search.md
[网站]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="e6ad6-115">权限</span><span class="sxs-lookup"><span data-stu-id="e6ad6-115">Permissions</span></span>

<span data-ttu-id="e6ad6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6ad6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6ad6-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6ad6-118">Permission type</span></span>                        | <span data-ttu-id="e6ad6-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6ad6-119">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="e6ad6-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6ad6-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6ad6-121">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6ad6-121">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="e6ad6-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6ad6-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6ad6-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6ad6-123">Not supported.</span></span>
|<span data-ttu-id="e6ad6-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6ad6-124">Application</span></span>                            | <span data-ttu-id="e6ad6-125">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6ad6-125">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="e6ad6-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6ad6-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites?$filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="e6ad6-127">示例</span><span class="sxs-lookup"><span data-stu-id="e6ad6-127">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e6ad6-128">请求</span><span class="sxs-lookup"><span data-stu-id="e6ad6-128">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e6ad6-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6ad6-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-sites" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites?$select=siteCollection,webUrl&$filter=siteCollection/root%20ne%20null
```
# <a name="c"></a>[<span data-ttu-id="e6ad6-130">C#</span><span class="sxs-lookup"><span data-stu-id="e6ad6-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6ad6-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6ad6-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6ad6-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6ad6-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e6ad6-133">响应</span><span class="sxs-lookup"><span data-stu-id="e6ad6-133">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
  ]
}
-->
