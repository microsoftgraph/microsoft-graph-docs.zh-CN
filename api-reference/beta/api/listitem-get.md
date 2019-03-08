---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 从 SharePoint 列表中获取条目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 60a413060a3b86264cd1b1ae1a2fbc632c98e7bf
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481242"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="ef2bc-102">获取列表中的项</span><span class="sxs-lookup"><span data-stu-id="ef2bc-102">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef2bc-103">返回[列表][]中某个[项][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="ef2bc-103">Returns the metadata for an [item][] in a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[项]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="ef2bc-106">权限</span><span class="sxs-lookup"><span data-stu-id="ef2bc-106">Permissions</span></span>

<span data-ttu-id="ef2bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef2bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef2bc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef2bc-109">Permission type</span></span>      | <span data-ttu-id="ef2bc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ef2bc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef2bc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef2bc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ef2bc-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef2bc-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef2bc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef2bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef2bc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef2bc-114">Not supported.</span></span>    |
|<span data-ttu-id="ef2bc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef2bc-115">Application</span></span> | <span data-ttu-id="ef2bc-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef2bc-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef2bc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef2bc-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="ef2bc-118">示例</span><span class="sxs-lookup"><span data-stu-id="ef2bc-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ef2bc-119">请求</span><span class="sxs-lookup"><span data-stu-id="ef2bc-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="ef2bc-120">响应</span><span class="sxs-lookup"><span data-stu-id="ef2bc-120">Response</span></span>

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
