---
title: 枚举网站
description: 列出组织中的匹配提供的筛选器条件和查询选项可用 [站点] []。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f225d9990637f8251ae40e3f66b0f993bbf74f32
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520338"
---
# <a name="enumerate-sites"></a><span data-ttu-id="877f7-103">枚举网站</span><span class="sxs-lookup"><span data-stu-id="877f7-103">Enumerate sites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="877f7-104">列出与提供的筛选器条件匹配并查询选项的组织中可用的[网站][]。</span><span class="sxs-lookup"><span data-stu-id="877f7-104">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="877f7-105">当前支持仅以下查询选项：</span><span class="sxs-lookup"><span data-stu-id="877f7-105">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="877f7-106">筛选语句</span><span class="sxs-lookup"><span data-stu-id="877f7-106">Filter statement</span></span>             | <span data-ttu-id="877f7-107">SELECT 语句</span><span class="sxs-lookup"><span data-stu-id="877f7-107">Select statement</span></span>        | <span data-ttu-id="877f7-108">说明</span><span class="sxs-lookup"><span data-stu-id="877f7-108">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="877f7-109">列出组织中的所有根级别网站集。</span><span class="sxs-lookup"><span data-stu-id="877f7-109">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="877f7-110">用于发现每个地理位置的主网站。</span><span class="sxs-lookup"><span data-stu-id="877f7-110">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="877f7-111">此外，您可能使用针对 / 网站集合的**[搜索][]** 查询查找匹配关键字给定的网站。</span><span class="sxs-lookup"><span data-stu-id="877f7-111">In addition, you may use a **[search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[Search]: site-search.md
[search]: site-search.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="877f7-114">权限</span><span class="sxs-lookup"><span data-stu-id="877f7-114">Permissions</span></span>

<span data-ttu-id="877f7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="877f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="877f7-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="877f7-117">Permission type</span></span>                        | <span data-ttu-id="877f7-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="877f7-118">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="877f7-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="877f7-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="877f7-120">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="877f7-120">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="877f7-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="877f7-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="877f7-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="877f7-122">Not supported.</span></span>
|<span data-ttu-id="877f7-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="877f7-123">Application</span></span>                            | <span data-ttu-id="877f7-124">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="877f7-124">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="877f7-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="877f7-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="877f7-126">示例</span><span class="sxs-lookup"><span data-stu-id="877f7-126">Example</span></span>

#### <a name="request"></a><span data-ttu-id="877f7-127">请求</span><span class="sxs-lookup"><span data-stu-id="877f7-127">Request</span></span>

<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```

#### <a name="response"></a><span data-ttu-id="877f7-128">响应</span><span class="sxs-lookup"><span data-stu-id="877f7-128">Response</span></span>

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
    "Error: /api-reference/beta/api/site-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
