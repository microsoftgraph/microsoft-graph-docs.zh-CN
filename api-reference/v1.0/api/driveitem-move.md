---
author: JeremyKelley
ms.date: 09/10/2017
title: 移动文件或文件夹
localization_priority: Normal
ms.prod: sharepoint
description: 若要将 DriveItem 移动到新的父项，应用程序会请求更新要移动的 DriveItem 的 parentReference。
doc_type: apiPageType
ms.openlocfilehash: cf09789b370df585c9245376524f209cfb9e1bbf
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240239"
---
# <a name="move-a-driveitem-to-a-new-folder"></a><span data-ttu-id="ac4b8-103">将 DriveItem 移动到一个新的文件夹</span><span class="sxs-lookup"><span data-stu-id="ac4b8-103">Move a DriveItem to a new folder</span></span>

<span data-ttu-id="ac4b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac4b8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac4b8-105">若要将 DriveItem 移动到新的父项，应用程序会请求更新要移动的 DriveItem 的 **parentReference**。</span><span class="sxs-lookup"><span data-stu-id="ac4b8-105">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move.</span></span>

<span data-ttu-id="ac4b8-106">这是[更新](driveitem-update.md)方法的特殊用例。</span><span class="sxs-lookup"><span data-stu-id="ac4b8-106">This is a special case of the [Update](driveitem-update.md) method.</span></span>
<span data-ttu-id="ac4b8-107">你的应用程序可以将以下操作组合到单个请求中：将项目移动到新的容器和更新项目的其他属性。</span><span class="sxs-lookup"><span data-stu-id="ac4b8-107">Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="ac4b8-108">无法使用这一请求在[驱动器](../resources/drive.md)之间移动项目。</span><span class="sxs-lookup"><span data-stu-id="ac4b8-108">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac4b8-109">权限</span><span class="sxs-lookup"><span data-stu-id="ac4b8-109">Permissions</span></span>
<span data-ttu-id="ac4b8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac4b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac4b8-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac4b8-112">Permission type</span></span>      | <span data-ttu-id="ac4b8-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac4b8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac4b8-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac4b8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ac4b8-115">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac4b8-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ac4b8-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac4b8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac4b8-117">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac4b8-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ac4b8-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac4b8-118">Application</span></span> | <span data-ttu-id="ac4b8-119">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac4b8-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac4b8-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac4b8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="ac4b8-121">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="ac4b8-121">Optional request headers</span></span>

| <span data-ttu-id="ac4b8-122">名称</span><span class="sxs-lookup"><span data-stu-id="ac4b8-122">Name</span></span>          | <span data-ttu-id="ac4b8-123">类型</span><span class="sxs-lookup"><span data-stu-id="ac4b8-123">Type</span></span>   | <span data-ttu-id="ac4b8-124">说明</span><span class="sxs-lookup"><span data-stu-id="ac4b8-124">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ac4b8-125">if-match</span><span class="sxs-lookup"><span data-stu-id="ac4b8-125">if-match</span></span>      | <span data-ttu-id="ac4b8-126">String</span><span class="sxs-lookup"><span data-stu-id="ac4b8-126">String</span></span> | <span data-ttu-id="ac4b8-127">如果包含此请求标头，且提供的 eTag（或 cTag）与文件夹上的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应。</span><span class="sxs-lookup"><span data-stu-id="ac4b8-127">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac4b8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac4b8-128">Request body</span></span>

<span data-ttu-id="ac4b8-p103">在请求正文中，提供 **parentReference** 属性的新值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="ac4b8-p103">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="ac4b8-132">**注意：** 将项目移动到驱动器的根目录下时，应用程序不能使用 `"id:" "root"` 语法。</span><span class="sxs-lookup"><span data-stu-id="ac4b8-132">**Note:** When moving items to the root of a drive your app cannot use the `"id:" "root"` syntax.</span></span>
<span data-ttu-id="ac4b8-133">应用程序必须为父引用提供实际的根文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="ac4b8-133">Your app needs to provide the actual ID of the root folder for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="ac4b8-134">响应</span><span class="sxs-lookup"><span data-stu-id="ac4b8-134">Response</span></span>

<span data-ttu-id="ac4b8-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [DriveItem](../resources/driveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="ac4b8-135">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac4b8-136">示例</span><span class="sxs-lookup"><span data-stu-id="ac4b8-136">Example</span></span>

<span data-ttu-id="ac4b8-137">本示例将 {item-id} 指定的项目移动到用户驱动器中 ID 为 `new-parent-folder-id` 的文件夹中。</span><span class="sxs-lookup"><span data-stu-id="ac4b8-137">This example moves an item specified by {item-id} into a folder in the user's drive with the ID `new-parent-folder-id`.</span></span>


# <a name="http"></a>[<span data-ttu-id="ac4b8-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac4b8-138">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "move-item", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "parentReference": {
    "id": "{new-parent-folder-id}"
  },
  "name": "new-item-name.txt"
}
```
# <a name="c"></a>[<span data-ttu-id="ac4b8-139">C#</span><span class="sxs-lookup"><span data-stu-id="ac4b8-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/move-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac4b8-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac4b8-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/move-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac4b8-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac4b8-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/move-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac4b8-142">Java</span><span class="sxs-lookup"><span data-stu-id="ac4b8-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/move-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ac4b8-143">响应</span><span class="sxs-lookup"><span data-stu-id="ac4b8-143">Response</span></span>

<span data-ttu-id="ac4b8-144">以下示例显示了对此移动请求的响应。</span><span class="sxs-lookup"><span data-stu-id="ac4b8-144">The following example shows the response for this move request.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "new-item-name.txt",
  "parentReference":
  {
    "driveId": "11231001",
    "path": "/drive/root:/Documents",
    "id": "1231203102!1011"
  }
}
```

## <a name="error-responses"></a><span data-ttu-id="ac4b8-145">错误响应</span><span class="sxs-lookup"><span data-stu-id="ac4b8-145">Error responses</span></span>

<span data-ttu-id="ac4b8-146">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="ac4b8-146">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Move an item to another location or rename the item.",
  "keywords": "move,rename,mv,change location",
  "section": "documentation",
  "tocPath": "Items/Move",
  "suppressions": [
  ]
} -->

