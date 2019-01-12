---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: 在 SharePoint 列表中创建新条目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7e977b635ec854e2e35bb1a12fdc0db22ddec722
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919440"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="174f5-102">在列表中创建新项</span><span class="sxs-lookup"><span data-stu-id="174f5-102">Create a new item in a list</span></span>

> <span data-ttu-id="174f5-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="174f5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="174f5-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="174f5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="174f5-105">在[列表][]中创建新的 [listItem][]。</span><span class="sxs-lookup"><span data-stu-id="174f5-105">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="174f5-106">权限</span><span class="sxs-lookup"><span data-stu-id="174f5-106">Permissions</span></span>

<span data-ttu-id="174f5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="174f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="174f5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="174f5-109">Permission type</span></span>      | <span data-ttu-id="174f5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="174f5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="174f5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="174f5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="174f5-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="174f5-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="174f5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="174f5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="174f5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="174f5-114">Not supported.</span></span>    |
|<span data-ttu-id="174f5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="174f5-115">Application</span></span> | <span data-ttu-id="174f5-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="174f5-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="174f5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="174f5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="174f5-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="174f5-118">Request body</span></span>

<span data-ttu-id="174f5-119">在请求正文中，提供要创建的 [listItem][] 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="174f5-119">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="174f5-120">示例</span><span class="sxs-lookup"><span data-stu-id="174f5-120">Example</span></span>

<span data-ttu-id="174f5-121">下面的示例展示了如何创建新的泛型列表项。</span><span class="sxs-lookup"><span data-stu-id="174f5-121">Here is an example of how to create a new generic list item.</span></span>

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

## <a name="response"></a><span data-ttu-id="174f5-122">响应</span><span class="sxs-lookup"><span data-stu-id="174f5-122">Response</span></span>

<span data-ttu-id="174f5-123">如果成功，此方法在已创建列表项的响应正文中返回 [listItem][]。</span><span class="sxs-lookup"><span data-stu-id="174f5-123">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

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

<span data-ttu-id="174f5-124">**注意：** 为清楚起见，将截断 Response 对象。</span><span class="sxs-lookup"><span data-stu-id="174f5-124">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="174f5-125">实际调用会返回默认属性。</span><span class="sxs-lookup"><span data-stu-id="174f5-125">Default properties will be returned from the actual call.</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[listItem]: ../resources/listitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Add a new item to a SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Create"
} -->
