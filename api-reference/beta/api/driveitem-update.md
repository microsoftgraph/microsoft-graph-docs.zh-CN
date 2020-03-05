---
author: JeremyKelley
description: 按 ID 或路径更新 DriveItem 元数据。
ms.date: 09/10/2017
title: 更新文件或文件夹
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: cff8bc2d7f5c4daec1da7e26f6f07b873b55dbee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432311"
---
# <a name="update-driveitem-properties"></a><span data-ttu-id="87ed0-103">更新 DriveItem 属性</span><span class="sxs-lookup"><span data-stu-id="87ed0-103">Update DriveItem properties</span></span>

<span data-ttu-id="87ed0-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="87ed0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87ed0-105">按 ID 或路径更新 [DriveItem](../resources/driveitem.md) 元数据。</span><span class="sxs-lookup"><span data-stu-id="87ed0-105">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="87ed0-106">还可以通过更新项的 **parentReference** 属性，使用更新将[项移动到](driveitem-move.md)其他父级。</span><span class="sxs-lookup"><span data-stu-id="87ed0-106">You can also use update to [move an item](driveitem-move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="87ed0-107">权限</span><span class="sxs-lookup"><span data-stu-id="87ed0-107">Permissions</span></span>

<span data-ttu-id="87ed0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="87ed0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87ed0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="87ed0-110">Permission type</span></span>      | <span data-ttu-id="87ed0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="87ed0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87ed0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87ed0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="87ed0-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87ed0-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="87ed0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87ed0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87ed0-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87ed0-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="87ed0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="87ed0-116">Application</span></span> | <span data-ttu-id="87ed0-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87ed0-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87ed0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87ed0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="87ed0-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="87ed0-119">Optional request headers</span></span>

| <span data-ttu-id="87ed0-120">名称</span><span class="sxs-lookup"><span data-stu-id="87ed0-120">Name</span></span>          | <span data-ttu-id="87ed0-121">类型</span><span class="sxs-lookup"><span data-stu-id="87ed0-121">Type</span></span>   | <span data-ttu-id="87ed0-122">说明</span><span class="sxs-lookup"><span data-stu-id="87ed0-122">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="87ed0-123">if-match</span><span class="sxs-lookup"><span data-stu-id="87ed0-123">if-match</span></span>      | <span data-ttu-id="87ed0-124">String</span><span class="sxs-lookup"><span data-stu-id="87ed0-124">String</span></span> | <span data-ttu-id="87ed0-125">如果包含此请求标头，且提供的 eTag（或 cTag）与文件夹上的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应。</span><span class="sxs-lookup"><span data-stu-id="87ed0-125">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87ed0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="87ed0-126">Request body</span></span>

<span data-ttu-id="87ed0-127">在请求正文中，提供应更新的属性的值。</span><span class="sxs-lookup"><span data-stu-id="87ed0-127">In the request body, supply the values for properties that should be updated.</span></span>

<span data-ttu-id="87ed0-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="87ed0-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="87ed0-129">为了获得最佳性能，应用不应包括尚未更改的属性。</span><span class="sxs-lookup"><span data-stu-id="87ed0-129">For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="87ed0-130">响应</span><span class="sxs-lookup"><span data-stu-id="87ed0-130">Response</span></span>

<span data-ttu-id="87ed0-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [DriveItem](../resources/driveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="87ed0-131">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87ed0-132">示例</span><span class="sxs-lookup"><span data-stu-id="87ed0-132">Example</span></span>

<span data-ttu-id="87ed0-133">本示例将 DriveItem 资源重命名为“new-file-name.docx”。</span><span class="sxs-lookup"><span data-stu-id="87ed0-133">This example renames the DriveItem resource to "new-file-name.docx".</span></span>


# <a name="http"></a>[<span data-ttu-id="87ed0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="87ed0-134">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "update-item" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```
# <a name="c"></a>[<span data-ttu-id="87ed0-135">C#</span><span class="sxs-lookup"><span data-stu-id="87ed0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87ed0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87ed0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87ed0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87ed0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="87ed0-138">响应</span><span class="sxs-lookup"><span data-stu-id="87ed0-138">Response</span></span>

<span data-ttu-id="87ed0-139">如果成功，此方法将在响应正文中返回 [driveItem][item-resource] 资源。</span><span class="sxs-lookup"><span data-stu-id="87ed0-139">If successful, this method returns an [driveItem][item-resource] resource in the response body.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="87ed0-140">错误响应</span><span class="sxs-lookup"><span data-stu-id="87ed0-140">Error responses</span></span>

<span data-ttu-id="87ed0-141">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="87ed0-141">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of an item.",
  "keywords": "update,replace,contents,item",
  "section": "documentation",
  "tocPath": "Items/Update",
  "suppressions": [
  ]
}
-->
