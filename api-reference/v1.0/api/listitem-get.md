---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 从 SharePoint 列表中获取条目
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: e9d747e5405a5aeaf97dfdf7e9a97f6236164a5a
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480640"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="18a32-102">获取列表中的项</span><span class="sxs-lookup"><span data-stu-id="18a32-102">Get an item in a list</span></span>

<span data-ttu-id="18a32-103">返回[列表][]中某个[项][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="18a32-103">Returns the metadata for an [item][] in a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[项]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="18a32-106">权限</span><span class="sxs-lookup"><span data-stu-id="18a32-106">Permissions</span></span>

<span data-ttu-id="18a32-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18a32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18a32-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="18a32-109">Permission type</span></span>      | <span data-ttu-id="18a32-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18a32-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18a32-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18a32-111">Delegated (work or school account)</span></span> | <span data-ttu-id="18a32-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18a32-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="18a32-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18a32-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18a32-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="18a32-114">Not supported.</span></span>    |
|<span data-ttu-id="18a32-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="18a32-115">Application</span></span> | <span data-ttu-id="18a32-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18a32-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18a32-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18a32-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="18a32-118">示例</span><span class="sxs-lookup"><span data-stu-id="18a32-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="18a32-119">请求</span><span class="sxs-lookup"><span data-stu-id="18a32-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="18a32-120">响应</span><span class="sxs-lookup"><span data-stu-id="18a32-120">Response</span></span>

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
