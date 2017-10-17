---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: "检索 SharePoint 列表中的项"
ms.openlocfilehash: a7f66db11ef201d0ae5afb2cc49887ee10dc89d7
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="0f738-102">枚举列表中的项</span><span class="sxs-lookup"><span data-stu-id="0f738-102">Enumerate items in a list</span></span>

<span data-ttu-id="0f738-103">获取[列表][]中[项][item]的集合。</span><span class="sxs-lookup"><span data-stu-id="0f738-103">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listItem.md

## <a name="permissions"></a><span data-ttu-id="0f738-105">权限</span><span class="sxs-lookup"><span data-stu-id="0f738-105">Permissions</span></span>

<span data-ttu-id="0f738-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0f738-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0f738-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f738-108">Permission type</span></span>      | <span data-ttu-id="0f738-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0f738-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f738-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f738-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0f738-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f738-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0f738-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f738-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f738-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f738-113">Not supported.</span></span>    |
|<span data-ttu-id="0f738-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f738-114">Application</span></span> | <span data-ttu-id="0f738-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f738-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f738-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f738-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="0f738-117">示例</span><span class="sxs-lookup"><span data-stu-id="0f738-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0f738-118">请求</span><span class="sxs-lookup"><span data-stu-id="0f738-118">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="0f738-119">响应</span><span class="sxs-lookup"><span data-stu-id="0f738-119">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Enumerate"
} -->
