---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 复制文件或文件夹
localization_priority: Normal
ms.prod: sharepoint
description: 以异步方式在新父项下或使用新名称创建一个 driveItem 副本（包括任何子项）。
doc_type: apiPageType
ms.openlocfilehash: e730d2ecd72a3a88c465373eabd8993c329e8601
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015556"
---
# <a name="copy-a-driveitem"></a><span data-ttu-id="e8356-103">复制 DriveItem</span><span class="sxs-lookup"><span data-stu-id="e8356-103">Copy a DriveItem</span></span>

<span data-ttu-id="e8356-104">以异步方式在新父项下或使用新名称创建一个 [driveItem][item-resource] 副本（包括任何子项）。</span><span class="sxs-lookup"><span data-stu-id="e8356-104">Asynchronously creates a copy of an [driveItem][item-resource] (including any children), under a new parent item or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8356-105">权限</span><span class="sxs-lookup"><span data-stu-id="e8356-105">Permissions</span></span>

<span data-ttu-id="e8356-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8356-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8356-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8356-108">Permission type</span></span>      | <span data-ttu-id="e8356-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8356-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8356-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8356-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8356-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8356-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8356-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8356-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8356-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8356-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8356-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8356-114">Application</span></span> | <span data-ttu-id="e8356-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8356-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8356-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8356-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a><span data-ttu-id="e8356-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8356-117">Request body</span></span>

<span data-ttu-id="e8356-118">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e8356-118">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="e8356-119">名称</span><span class="sxs-lookup"><span data-stu-id="e8356-119">Name</span></span>            | <span data-ttu-id="e8356-120">值</span><span class="sxs-lookup"><span data-stu-id="e8356-120">Value</span></span>                                          | <span data-ttu-id="e8356-121">说明</span><span class="sxs-lookup"><span data-stu-id="e8356-121">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e8356-122">parentReference</span><span class="sxs-lookup"><span data-stu-id="e8356-122">parentReference</span></span> | [<span data-ttu-id="e8356-123">ItemReference</span><span class="sxs-lookup"><span data-stu-id="e8356-123">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="e8356-p102">可选。引用在其中创建副本的父项。</span><span class="sxs-lookup"><span data-stu-id="e8356-p102">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="e8356-126">name</span><span class="sxs-lookup"><span data-stu-id="e8356-126">name</span></span>            | <span data-ttu-id="e8356-127">string</span><span class="sxs-lookup"><span data-stu-id="e8356-127">string</span></span>                                         | <span data-ttu-id="e8356-p103">可选。副本的新名称。如果未提供新名称，将同一名称用作原始名称。</span><span class="sxs-lookup"><span data-stu-id="e8356-p103">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="e8356-131">**注意：**_parentReference_ 应包括目标文件夹的 `driveId` 和 `id` 参数。</span><span class="sxs-lookup"><span data-stu-id="e8356-131">**Note:** The _parentReference_ should include the `driveId` and `id` parameters for the target folder.</span></span>

## <a name="example"></a><span data-ttu-id="e8356-132">示例</span><span class="sxs-lookup"><span data-stu-id="e8356-132">Example</span></span>

<span data-ttu-id="e8356-133">本示例将由 `{item-id}` 标识的文件复制到使用 `driveId` 和 `id` 值标识的文件夹。</span><span class="sxs-lookup"><span data-stu-id="e8356-133">This example copies a file identified by `{item-id}` into a folder identified with a `driveId` and `id` value.</span></span>
<span data-ttu-id="e8356-134">该文件的新副本将被命名为 `contoso plan (copy).txt`。</span><span class="sxs-lookup"><span data-stu-id="e8356-134">The new copy of the file will be named `contoso plan (copy).txt`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e8356-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e8356-135">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite", "tags": "service.graph", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "driveId": "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B",
    "id": "DCD0D3AD-8989-4F23-A5A2-2C086050513F"
  },
  "name": "contoso plan (copy).txt"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e8356-136">C#</span><span class="sxs-lookup"><span data-stu-id="e8356-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/copy-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8356-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="e8356-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/copy-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e8356-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="e8356-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/copy-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e8356-139">Java</span><span class="sxs-lookup"><span data-stu-id="e8356-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/copy-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="e8356-140">响应</span><span class="sxs-lookup"><span data-stu-id="e8356-140">Response</span></span>

<span data-ttu-id="e8356-141">返回有关如何在接受请求时[监视复制操作进度](/graph/long-running-actions-overview)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e8356-141">Returns details about how to [monitor the progress](/graph/long-running-actions-overview) of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="e8356-p105">`Location` 头值提供的服务 URL 将返回复制操作的最新状态。 可以根据此信息[确定复制操作完成时间](/graph/long-running-actions-overview)。</span><span class="sxs-lookup"><span data-stu-id="e8356-p105">The value of the `Location` header provides a URL for a service that will return the current state of the copy operation. You can use this info to [determine when the copy has finished](/graph/long-running-actions-overview).</span></span>

### <a name="remarks"></a><span data-ttu-id="e8356-144">注解</span><span class="sxs-lookup"><span data-stu-id="e8356-144">Remarks</span></span>

<span data-ttu-id="e8356-p106">在许多情况下，复制操作采用异步执行。API 响应仅指明复制操作获得接受还是遭到拒绝（比如说，由于目标文件名已被其他对象使用而遭到拒绝）。</span><span class="sxs-lookup"><span data-stu-id="e8356-p106">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
} -->
