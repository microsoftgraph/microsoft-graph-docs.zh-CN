---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: 列出网站中的 SharePoint 列表
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f7adfeba7f46eb7ed8541405221a1257637c2157
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512442"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="44d48-102">枚举网站中的列表</span><span class="sxs-lookup"><span data-stu-id="44d48-102">Enumerate lists in a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44d48-103">获取 [site][] 的 [lists][] 的集合。</span><span class="sxs-lookup"><span data-stu-id="44d48-103">Get the collection of [lists][] for a [site][].</span></span>

[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="44d48-106">权限</span><span class="sxs-lookup"><span data-stu-id="44d48-106">Permissions</span></span>

<span data-ttu-id="44d48-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44d48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44d48-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="44d48-109">Permission type</span></span>      | <span data-ttu-id="44d48-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44d48-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44d48-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44d48-111">Delegated (work or school account)</span></span> | <span data-ttu-id="44d48-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44d48-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="44d48-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44d48-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44d48-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="44d48-114">Not supported.</span></span>    |
|<span data-ttu-id="44d48-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="44d48-115">Application</span></span> | <span data-ttu-id="44d48-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44d48-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44d48-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44d48-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="44d48-118">示例</span><span class="sxs-lookup"><span data-stu-id="44d48-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="44d48-119">请求</span><span class="sxs-lookup"><span data-stu-id="44d48-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="44d48-120">响应</span><span class="sxs-lookup"><span data-stu-id="44d48-120">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b57af081-936c-4803-a120-d94887b03864",
      "name": "Documents",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "documentLibrary"
       }
    },
    {
      "id": "1234-112-112-4",
      "name": "MicroFeed",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "genericList"
       }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="44d48-121">注解</span><span class="sxs-lookup"><span data-stu-id="44d48-121">Remarks</span></span>

<span data-ttu-id="44d48-122">默认情况下，将隐藏包含 [system][] Facet 的列表。</span><span class="sxs-lookup"><span data-stu-id="44d48-122">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="44d48-123">若要列出它们，请在 `$select` 语句中添加 `system`。</span><span class="sxs-lookup"><span data-stu-id="44d48-123">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate",
  "suppressions": [
    "Error: /api-reference/beta/api/list-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
