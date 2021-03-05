---
title: 枚举网站
description: 列出组织中与提供的筛选条件与查询选项匹配的可用 [sites][]。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: JeremyKelley
ms.openlocfilehash: c1b8af50227346e4440e4ca98873b20160ecd81b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475777"
---
# <a name="enumerate-sites"></a><span data-ttu-id="7c0b7-103">枚举网站</span><span class="sxs-lookup"><span data-stu-id="7c0b7-103">Enumerate sites</span></span>

<span data-ttu-id="7c0b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c0b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c0b7-105">列出组织中 [与提供的][] 筛选条件与查询选项相匹配的可用网站。</span><span class="sxs-lookup"><span data-stu-id="7c0b7-105">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="7c0b7-106">当前仅支持以下查询选项：</span><span class="sxs-lookup"><span data-stu-id="7c0b7-106">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="7c0b7-107">Filter 语句</span><span class="sxs-lookup"><span data-stu-id="7c0b7-107">Filter statement</span></span>             | <span data-ttu-id="7c0b7-108">Select 语句</span><span class="sxs-lookup"><span data-stu-id="7c0b7-108">Select statement</span></span>        | <span data-ttu-id="7c0b7-109">说明</span><span class="sxs-lookup"><span data-stu-id="7c0b7-109">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="7c0b7-110">列出组织的所有根级别网站集。</span><span class="sxs-lookup"><span data-stu-id="7c0b7-110">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="7c0b7-111">可用于发现每个地理位置的主页。</span><span class="sxs-lookup"><span data-stu-id="7c0b7-111">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="7c0b7-112">此外，您可以使用针对"/sites"$search查询来查找与给定关键字匹配的网站。 **[][]**</span><span class="sxs-lookup"><span data-stu-id="7c0b7-112">In addition, you may use a **[$search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[$search]: site-search.md
[网站]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="7c0b7-115">权限</span><span class="sxs-lookup"><span data-stu-id="7c0b7-115">Permissions</span></span>

<span data-ttu-id="7c0b7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c0b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c0b7-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c0b7-118">Permission type</span></span>                        | <span data-ttu-id="7c0b7-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c0b7-119">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="7c0b7-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c0b7-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c0b7-121">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c0b7-121">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="7c0b7-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c0b7-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c0b7-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c0b7-123">Not supported.</span></span>
|<span data-ttu-id="7c0b7-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c0b7-124">Application</span></span>                            | <span data-ttu-id="7c0b7-125">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c0b7-125">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="7c0b7-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c0b7-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites?$filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="7c0b7-127">示例</span><span class="sxs-lookup"><span data-stu-id="7c0b7-127">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7c0b7-128">请求</span><span class="sxs-lookup"><span data-stu-id="7c0b7-128">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7c0b7-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c0b7-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-sites" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites?$select=siteCollection,webUrl&$filter=siteCollection/root%20ne%20null
```
# <a name="c"></a>[<span data-ttu-id="7c0b7-130">C#</span><span class="sxs-lookup"><span data-stu-id="7c0b7-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c0b7-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c0b7-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c0b7-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c0b7-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c0b7-133">Java</span><span class="sxs-lookup"><span data-stu-id="7c0b7-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-sites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7c0b7-134">响应</span><span class="sxs-lookup"><span data-stu-id="7c0b7-134">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```http
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


