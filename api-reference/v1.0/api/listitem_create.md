---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: "在 SharePoint 列表中创建新条目"
ms.openlocfilehash: 55a3c52d7afb2a276055cdddfb826ebbcb574ae7
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="e180b-102">在列表中创建新项</span><span class="sxs-lookup"><span data-stu-id="e180b-102">Create a new item in a list</span></span>

<span data-ttu-id="e180b-103">在 [list][] 中创建新的 [listItem][]。</span><span class="sxs-lookup"><span data-stu-id="e180b-103">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="e180b-104">权限</span><span class="sxs-lookup"><span data-stu-id="e180b-104">Permissions</span></span>

<span data-ttu-id="e180b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e180b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e180b-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="e180b-107">Permission type</span></span>      | <span data-ttu-id="e180b-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e180b-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e180b-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e180b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="e180b-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e180b-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e180b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e180b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e180b-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e180b-112">Not supported.</span></span>    |
|<span data-ttu-id="e180b-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="e180b-113">Application</span></span> | <span data-ttu-id="e180b-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e180b-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e180b-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e180b-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="e180b-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="e180b-116">Request body</span></span>

<span data-ttu-id="e180b-117">在请求正文中，提供要创建的 [listItem][] 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e180b-117">In the request body, supply a JSON representation of the [DriveItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="e180b-118">示例</span><span class="sxs-lookup"><span data-stu-id="e180b-118">Example</span></span>

<span data-ttu-id="e180b-119">下面的示例展示了如何创建新的泛型列表项。</span><span class="sxs-lookup"><span data-stu-id="e180b-119">Here is an example of how to create a new folder.</span></span>

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
Content-Type: application/json

{
  "fields": {
    "Title": "Widget",
    "Color": "Purple",
    "Weight": 32
  }
}
```

## <a name="response"></a><span data-ttu-id="e180b-120">响应</span><span class="sxs-lookup"><span data-stu-id="e180b-120">Response</span></span>

<span data-ttu-id="e180b-121">如果成功，此方法在已创建列表项的响应正文中返回 [listItem][]。</span><span class="sxs-lookup"><span data-stu-id="e180b-121">If successful, this method returns a [driveItem][] object in the response body for the newly created file.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "20",
  "createdDateTime": "2016-08-30T08:26:00Z",
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  },
  "lastModifiedDateTime": "2016-08-30T08:26:00Z",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  }
}
```

<span data-ttu-id="e180b-122">**注意：**为清楚起见，将截断 Response 对象。</span><span class="sxs-lookup"><span data-stu-id="e180b-122">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="e180b-123">实际调用会返回默认属性。</span><span class="sxs-lookup"><span data-stu-id="e180b-123">All default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[listItem]: ../resources/listItem.md

<!-- {
  "type": "#page.annotation",
  "description": "Add a new item to a SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Create"
} -->
