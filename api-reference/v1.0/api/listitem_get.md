---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: 从 SharePoint 列表中获取条目
ms.openlocfilehash: 418c64534fe20cd74ddba607fa9c765dc20bac42
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "23270046"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="a908c-102">获取列表中的项</span><span class="sxs-lookup"><span data-stu-id="a908c-102">Get an item in a list</span></span>

<span data-ttu-id="a908c-103">返回[列表][]中某个[项][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="a908c-103">Returns the metadata for an [item][] in a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[项]: ../resources/listItem.md
[item]: ../resources/listItem.md

## <a name="permissions"></a><span data-ttu-id="a908c-106">权限</span><span class="sxs-lookup"><span data-stu-id="a908c-106">Permissions</span></span>

<span data-ttu-id="a908c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a908c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a908c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a908c-109">Permission type</span></span>      | <span data-ttu-id="a908c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a908c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a908c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a908c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a908c-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a908c-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a908c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a908c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a908c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a908c-114">Not supported.</span></span>    |
|<span data-ttu-id="a908c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a908c-115">Application</span></span> | <span data-ttu-id="a908c-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a908c-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a908c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a908c-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="a908c-118">示例</span><span class="sxs-lookup"><span data-stu-id="a908c-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a908c-119">请求</span><span class="sxs-lookup"><span data-stu-id="a908c-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="a908c-120">响应</span><span class="sxs-lookup"><span data-stu-id="a908c-120">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "5",
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
