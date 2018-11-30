---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: 从 SharePoint 列表中获取条目
ms.openlocfilehash: 240f9f285178407f167cfb66b790224aa24c35d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046823"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="fa17a-102">获取列表中的项</span><span class="sxs-lookup"><span data-stu-id="fa17a-102">Get an item in a list</span></span>

> <span data-ttu-id="fa17a-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fa17a-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa17a-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fa17a-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa17a-105">返回[列表][]中某个[项][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="fa17a-105">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[项]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="fa17a-108">权限</span><span class="sxs-lookup"><span data-stu-id="fa17a-108">Permissions</span></span>

<span data-ttu-id="fa17a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa17a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa17a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa17a-111">Permission type</span></span>      | <span data-ttu-id="fa17a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa17a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa17a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa17a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fa17a-114">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa17a-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fa17a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa17a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa17a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa17a-116">Not supported.</span></span>    |
|<span data-ttu-id="fa17a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa17a-117">Application</span></span> | <span data-ttu-id="fa17a-118">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa17a-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa17a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa17a-119">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="fa17a-120">示例</span><span class="sxs-lookup"><span data-stu-id="fa17a-120">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fa17a-121">请求</span><span class="sxs-lookup"><span data-stu-id="fa17a-121">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="fa17a-122">响应</span><span class="sxs-lookup"><span data-stu-id="fa17a-122">Response</span></span>

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
