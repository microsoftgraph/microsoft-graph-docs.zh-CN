---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 移动文件或文件夹
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: db51a1c20803dc734d684f75686b115bb350e356
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272812"
---
# <a name="move-a-driveitem-to-a-new-folder"></a><span data-ttu-id="82696-102">将 DriveItem 移动到一个新的文件夹</span><span class="sxs-lookup"><span data-stu-id="82696-102">Move a DriveItem to a new folder</span></span>

<span data-ttu-id="82696-103">若要将 DriveItem 移动到新的父项，应用程序会请求更新要移动的 DriveItem 的 **parentReference**。</span><span class="sxs-lookup"><span data-stu-id="82696-103">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move.</span></span>

<span data-ttu-id="82696-104">这是[更新](driveitem-update.md)方法的特殊用例。</span><span class="sxs-lookup"><span data-stu-id="82696-104">This is a special case of the [Update](driveitem-update.md) method.</span></span>
<span data-ttu-id="82696-105">你的应用程序可以将以下操作组合到单个请求中：将项目移动到新的容器和更新项目的其他属性。</span><span class="sxs-lookup"><span data-stu-id="82696-105">Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="82696-106">无法使用这一请求在[驱动器](../resources/drive.md)之间移动项目。</span><span class="sxs-lookup"><span data-stu-id="82696-106">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="permissions"></a><span data-ttu-id="82696-107">权限</span><span class="sxs-lookup"><span data-stu-id="82696-107">Permissions</span></span>
<span data-ttu-id="82696-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82696-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82696-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="82696-110">Permission type</span></span>      | <span data-ttu-id="82696-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82696-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82696-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82696-112">Delegated (work or school account)</span></span> | <span data-ttu-id="82696-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82696-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="82696-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82696-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82696-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82696-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="82696-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="82696-116">Application</span></span> | <span data-ttu-id="82696-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82696-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82696-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82696-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="82696-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="82696-119">Optional request headers</span></span>

| <span data-ttu-id="82696-120">名称</span><span class="sxs-lookup"><span data-stu-id="82696-120">Name</span></span>          | <span data-ttu-id="82696-121">类型</span><span class="sxs-lookup"><span data-stu-id="82696-121">Type</span></span>   | <span data-ttu-id="82696-122">说明</span><span class="sxs-lookup"><span data-stu-id="82696-122">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="82696-123">if-match</span><span class="sxs-lookup"><span data-stu-id="82696-123">if-match</span></span>      | <span data-ttu-id="82696-124">String</span><span class="sxs-lookup"><span data-stu-id="82696-124">String</span></span> | <span data-ttu-id="82696-125">如果包含此请求标头，且提供的 eTag（或 cTag）与文件夹上的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应。</span><span class="sxs-lookup"><span data-stu-id="82696-125">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82696-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="82696-126">Request body</span></span>

<span data-ttu-id="82696-p103">在请求正文中，提供 **parentReference** 属性的新值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="82696-p103">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="82696-130">**注意：** 将项目移动到驱动器的根目录下时，应用程序不能使用 `"id:" "root"` 语法。</span><span class="sxs-lookup"><span data-stu-id="82696-130">**Note:** When moving items to the root of a drive your app cannot use the `"id:" "root"` syntax.</span></span>
<span data-ttu-id="82696-131">应用程序必须为父引用提供实际的根文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="82696-131">Your app needs to provide the actual ID of the root folder for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="82696-132">响应</span><span class="sxs-lookup"><span data-stu-id="82696-132">Response</span></span>

<span data-ttu-id="82696-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [DriveItem](../resources/driveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="82696-133">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82696-134">示例</span><span class="sxs-lookup"><span data-stu-id="82696-134">Example</span></span>

<span data-ttu-id="82696-135">本示例将 {item-id} 指定的项目移动到用户驱动器中 ID 为 `new-parent-folder-id` 的文件夹中。</span><span class="sxs-lookup"><span data-stu-id="82696-135">This example moves an item specified by {item-id} into a folder in the user's drive with the ID `new-parent-folder-id`.</span></span>

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

### <a name="response"></a><span data-ttu-id="82696-136">响应</span><span class="sxs-lookup"><span data-stu-id="82696-136">Response</span></span>

<span data-ttu-id="82696-137">以下示例显示了对此移动请求的响应。</span><span class="sxs-lookup"><span data-stu-id="82696-137">The following example shows the response for this move request.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="82696-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="82696-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="82696-139">C#</span><span class="sxs-lookup"><span data-stu-id="82696-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/move-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82696-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="82696-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/move-item-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="82696-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="82696-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/move-item-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="error-responses"></a><span data-ttu-id="82696-142">错误响应</span><span class="sxs-lookup"><span data-stu-id="82696-142">Error responses</span></span>

<span data-ttu-id="82696-143">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="82696-143">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Move an item to another location or rename the item.",
  "keywords": "move,rename,mv,change location",
  "section": "documentation",
  "tocPath": "Items/Move",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitem-move.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/driveitem-move.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-move.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
