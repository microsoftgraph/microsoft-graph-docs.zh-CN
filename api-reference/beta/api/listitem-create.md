---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 在 SharePoint 列表中创建新条目
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 1af6162fd12c9c3dfc470b97e42a25d0cad8ebea
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541008"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="867aa-102">在列表中创建新项</span><span class="sxs-lookup"><span data-stu-id="867aa-102">Create a new item in a list</span></span>

<span data-ttu-id="867aa-103">在[列表][]中创建新的 [listItem][]。</span><span class="sxs-lookup"><span data-stu-id="867aa-103">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="867aa-104">权限</span><span class="sxs-lookup"><span data-stu-id="867aa-104">Permissions</span></span>

<span data-ttu-id="867aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="867aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="867aa-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="867aa-107">Permission type</span></span>      | <span data-ttu-id="867aa-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="867aa-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="867aa-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="867aa-109">Delegated (work or school account)</span></span> | <span data-ttu-id="867aa-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="867aa-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="867aa-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="867aa-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="867aa-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="867aa-112">Not supported.</span></span>    |
|<span data-ttu-id="867aa-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="867aa-113">Application</span></span> | <span data-ttu-id="867aa-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="867aa-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="867aa-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="867aa-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="867aa-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="867aa-116">Request body</span></span>

<span data-ttu-id="867aa-117">在请求正文中，提供要创建的 [listItem][] 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="867aa-117">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="867aa-118">示例</span><span class="sxs-lookup"><span data-stu-id="867aa-118">Example</span></span>

<span data-ttu-id="867aa-119">下面的示例展示了如何创建新的泛型列表项。</span><span class="sxs-lookup"><span data-stu-id="867aa-119">Here is an example of how to create a new generic list item.</span></span>

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
Content-Type: application/json

{
  "fields": {
    "Title": "Widget",
    "Color": "Purple",
    "Weight": 32
  }
}
```

## <a name="response"></a><span data-ttu-id="867aa-120">响应</span><span class="sxs-lookup"><span data-stu-id="867aa-120">Response</span></span>

<span data-ttu-id="867aa-121">如果成功，此方法在已创建列表项的响应正文中返回 [listItem][]。</span><span class="sxs-lookup"><span data-stu-id="867aa-121">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

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

<span data-ttu-id="867aa-122">**注意：** 为清楚起见，将截断 Response 对象。</span><span class="sxs-lookup"><span data-stu-id="867aa-122">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="867aa-123">实际调用会返回默认属性。</span><span class="sxs-lookup"><span data-stu-id="867aa-123">Default properties will be returned from the actual call.</span></span>

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
