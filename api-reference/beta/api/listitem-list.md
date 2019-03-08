---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 检索 SharePoint 列表中的项
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 26d2aa28566a666692e49bc0d07305bf793e21d1
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481690"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="118e6-102">枚举列表中的项</span><span class="sxs-lookup"><span data-stu-id="118e6-102">Enumerate items in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="118e6-103">获取[列表][]中[项][item]的集合。</span><span class="sxs-lookup"><span data-stu-id="118e6-103">Get the collection of [items][item] in a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="118e6-105">权限</span><span class="sxs-lookup"><span data-stu-id="118e6-105">Permissions</span></span>

<span data-ttu-id="118e6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="118e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="118e6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="118e6-108">Permission type</span></span>      | <span data-ttu-id="118e6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="118e6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="118e6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="118e6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="118e6-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="118e6-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="118e6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="118e6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="118e6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="118e6-113">Not supported.</span></span>    |
|<span data-ttu-id="118e6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="118e6-114">Application</span></span> | <span data-ttu-id="118e6-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="118e6-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="118e6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="118e6-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="118e6-117">示例</span><span class="sxs-lookup"><span data-stu-id="118e6-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="118e6-118">请求</span><span class="sxs-lookup"><span data-stu-id="118e6-118">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="118e6-119">响应</span><span class="sxs-lookup"><span data-stu-id="118e6-119">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItem)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "2",
      "fields": {
        "Name": "Gadget",
        "Color": "Red",
        "Quantity": 503
       }
    },
    {
      "id": "4",
      "fields": {
        "Name": "Widget",
        "Color": "Blue",
        "Quantity": 2357
       }
    },
    {
      "id": "7",
      "fields": {
        "Name": "Gizmo",
        "Color": "Green",
        "Quantity": 92
       }
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
  "tocPath": "ListItem/Enumerate",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
