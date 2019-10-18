---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 更新文件或文件夹
localization_priority: Priority
ms.prod: sharepoint
description: 按 ID 或路径更新 DriveItem 元数据。
doc_type: apiPageType
ms.openlocfilehash: fbeae35750f46d8f205e489b8d830d3ffa0885e0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370548"
---
# <a name="update-driveitem-properties"></a><span data-ttu-id="30be9-103">更新 DriveItem 属性</span><span class="sxs-lookup"><span data-stu-id="30be9-103">Update DriveItem properties</span></span>

<span data-ttu-id="30be9-104">按 ID 或路径更新 [DriveItem](../resources/driveitem.md) 元数据。</span><span class="sxs-lookup"><span data-stu-id="30be9-104">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="30be9-105">还可以通过更新项的 **parentReference** 属性，使用更新将[项移动到](driveitem-move.md)其他父级。</span><span class="sxs-lookup"><span data-stu-id="30be9-105">You can also use update to [move an item](driveitem-move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="30be9-106">权限</span><span class="sxs-lookup"><span data-stu-id="30be9-106">Permissions</span></span>

<span data-ttu-id="30be9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="30be9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30be9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="30be9-109">Permission type</span></span>      | <span data-ttu-id="30be9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="30be9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30be9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30be9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="30be9-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30be9-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="30be9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30be9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30be9-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30be9-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="30be9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="30be9-115">Application</span></span> | <span data-ttu-id="30be9-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30be9-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="30be9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30be9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="30be9-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="30be9-118">Optional request headers</span></span>

| <span data-ttu-id="30be9-119">名称</span><span class="sxs-lookup"><span data-stu-id="30be9-119">Name</span></span>          | <span data-ttu-id="30be9-120">类型</span><span class="sxs-lookup"><span data-stu-id="30be9-120">Type</span></span>   | <span data-ttu-id="30be9-121">说明</span><span class="sxs-lookup"><span data-stu-id="30be9-121">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="30be9-122">if-match</span><span class="sxs-lookup"><span data-stu-id="30be9-122">if-match</span></span>      | <span data-ttu-id="30be9-123">String</span><span class="sxs-lookup"><span data-stu-id="30be9-123">String</span></span> | <span data-ttu-id="30be9-124">如果包含此请求标头，且提供的 eTag（或 cTag）与文件夹上的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应。</span><span class="sxs-lookup"><span data-stu-id="30be9-124">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30be9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="30be9-125">Request body</span></span>

<span data-ttu-id="30be9-126">在请求正文中，提供应更新的属性的值。</span><span class="sxs-lookup"><span data-stu-id="30be9-126">In the request body, supply the values for properties that should be updated.</span></span>

<span data-ttu-id="30be9-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="30be9-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="30be9-128">为了获得最佳性能，应用不应包括尚未更改的属性。</span><span class="sxs-lookup"><span data-stu-id="30be9-128">For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="30be9-129">响应</span><span class="sxs-lookup"><span data-stu-id="30be9-129">Response</span></span>

<span data-ttu-id="30be9-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [DriveItem](../resources/driveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="30be9-130">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30be9-131">示例</span><span class="sxs-lookup"><span data-stu-id="30be9-131">Example</span></span>

<span data-ttu-id="30be9-132">本示例将 DriveItem 资源重命名为“new-file-name.docx”。</span><span class="sxs-lookup"><span data-stu-id="30be9-132">This example renames the DriveItem resource to "new-file-name.docx".</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="30be9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="30be9-133">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "update-item", "tags": "service.graph" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="30be9-134">C#</span><span class="sxs-lookup"><span data-stu-id="30be9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="30be9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30be9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="30be9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30be9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="30be9-137">Java</span><span class="sxs-lookup"><span data-stu-id="30be9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="30be9-138">响应</span><span class="sxs-lookup"><span data-stu-id="30be9-138">Response</span></span>

<span data-ttu-id="30be9-139">如果成功，此方法将在响应正文中返回 [driveItem][item-resource] 资源。</span><span class="sxs-lookup"><span data-stu-id="30be9-139">If successful, this method returns an [driveItem][item-resource] resource in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "name": "new-file-name.docx",
  "file": { }
}
```

## <a name="error-responses"></a><span data-ttu-id="30be9-140">错误响应</span><span class="sxs-lookup"><span data-stu-id="30be9-140">Error responses</span></span>

<span data-ttu-id="30be9-141">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="30be9-141">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of an item.",
  "keywords": "update,replace,contents,item",
  "section": "documentation",
  "tocPath": "Items/Update",
  "suppressions": [
  ]
} -->
