---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: 从 SharePoint 列表中获取条目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 248208542b954c11992908529d4f21a9b7d96673
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512190"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="eb57a-102">获取列表中的项</span><span class="sxs-lookup"><span data-stu-id="eb57a-102">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb57a-103">返回[列表][]中某个[项][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="eb57a-103">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="eb57a-106">权限</span><span class="sxs-lookup"><span data-stu-id="eb57a-106">Permissions</span></span>

<span data-ttu-id="eb57a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb57a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb57a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb57a-109">Permission type</span></span>      | <span data-ttu-id="eb57a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb57a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb57a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb57a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eb57a-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb57a-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb57a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb57a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb57a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb57a-114">Not supported.</span></span>    |
|<span data-ttu-id="eb57a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb57a-115">Application</span></span> | <span data-ttu-id="eb57a-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb57a-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb57a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb57a-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="eb57a-118">示例</span><span class="sxs-lookup"><span data-stu-id="eb57a-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="eb57a-119">请求</span><span class="sxs-lookup"><span data-stu-id="eb57a-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="eb57a-120">响应</span><span class="sxs-lookup"><span data-stu-id="eb57a-120">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "d14922d8-43e6-4c8a-b029-e35c5b4e0d63",
  "listItemId": 2,
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
