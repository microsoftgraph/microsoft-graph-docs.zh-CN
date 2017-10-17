---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: "从 SharePoint 列表中获取条目"
ms.openlocfilehash: 29db5f5a3005aca0003489db4bdb13219e612a96
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="f7ade-102">获取列表中的项</span><span class="sxs-lookup"><span data-stu-id="f7ade-102">Get an item in a list</span></span>

<span data-ttu-id="f7ade-103">返回 [list][] 中 [item][] 的元数据。</span><span class="sxs-lookup"><span data-stu-id="f7ade-103">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listItem.md

## <a name="permissions"></a><span data-ttu-id="f7ade-106">权限</span><span class="sxs-lookup"><span data-stu-id="f7ade-106">Permissions</span></span>

<span data-ttu-id="f7ade-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f7ade-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f7ade-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7ade-109">Permission type</span></span>      | <span data-ttu-id="f7ade-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7ade-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7ade-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7ade-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f7ade-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7ade-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7ade-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7ade-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7ade-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7ade-114">Not supported.</span></span>    |
|<span data-ttu-id="f7ade-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7ade-115">Application</span></span> | <span data-ttu-id="f7ade-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7ade-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7ade-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7ade-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="f7ade-118">示例</span><span class="sxs-lookup"><span data-stu-id="f7ade-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f7ade-119">请求</span><span class="sxs-lookup"><span data-stu-id="f7ade-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="f7ade-120">响应</span><span class="sxs-lookup"><span data-stu-id="f7ade-120">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata"
} -->
