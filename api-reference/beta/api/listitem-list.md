---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: 检索 SharePoint 列表中的项
localization_priority: Normal
ms.openlocfilehash: eaecf297e612f8eb832f13751571816dfe950942
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874478"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="92d8e-102">枚举列表中的项</span><span class="sxs-lookup"><span data-stu-id="92d8e-102">Enumerate items in a list</span></span>

> <span data-ttu-id="92d8e-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="92d8e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92d8e-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="92d8e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="92d8e-105">获取[列表][]中[项][item]的集合。</span><span class="sxs-lookup"><span data-stu-id="92d8e-105">Get the collection of [items][item] in a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="92d8e-107">权限</span><span class="sxs-lookup"><span data-stu-id="92d8e-107">Permissions</span></span>

<span data-ttu-id="92d8e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92d8e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92d8e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="92d8e-110">Permission type</span></span>      | <span data-ttu-id="92d8e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92d8e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92d8e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92d8e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="92d8e-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92d8e-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="92d8e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92d8e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92d8e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="92d8e-115">Not supported.</span></span>    |
|<span data-ttu-id="92d8e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="92d8e-116">Application</span></span> | <span data-ttu-id="92d8e-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92d8e-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="92d8e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92d8e-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="92d8e-119">示例</span><span class="sxs-lookup"><span data-stu-id="92d8e-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="92d8e-120">请求</span><span class="sxs-lookup"><span data-stu-id="92d8e-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="92d8e-121">响应</span><span class="sxs-lookup"><span data-stu-id="92d8e-121">Response</span></span>

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
