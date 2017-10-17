---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "移动文件或文件夹"
ms.openlocfilehash: ebffe8451c6cf5ce7f025b70225054cfb8080cf6
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="move-a-driveitem-to-a-new-folder"></a><span data-ttu-id="04344-102">将 DriveItem 移动到新文件夹</span><span class="sxs-lookup"><span data-stu-id="04344-102">Move a DriveItem to a new folder</span></span>

<span data-ttu-id="04344-103">若要将 DriveItem 移动到新的父项，应用会请求更新要移动的 DriveItem 的 **parentReference**。</span><span class="sxs-lookup"><span data-stu-id="04344-103">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move.</span></span>

<span data-ttu-id="04344-104">这是 [Update](driveitem_update.md) 方法的特殊情况。</span><span class="sxs-lookup"><span data-stu-id="04344-104">This is a special case of the [update](driveitem_update.md) method.</span></span>
<span data-ttu-id="04344-105">你的应用可以将以下操作组合到单个请求中：将项目移动到新的容器和更新项目的其他属性。</span><span class="sxs-lookup"><span data-stu-id="04344-105">To move a DriveItem to a new parent item, your app requests to update the parentReference of the DriveItem to move. This is a special case of the Update method. Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="04344-106">无法使用此请求在[驱动器](../resources/drive.md)之间移动项目。</span><span class="sxs-lookup"><span data-stu-id="04344-106">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="permissions"></a><span data-ttu-id="04344-107">权限</span><span class="sxs-lookup"><span data-stu-id="04344-107">Permissions</span></span>
<span data-ttu-id="04344-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="04344-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="04344-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="04344-110">Permission type</span></span>      | <span data-ttu-id="04344-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="04344-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04344-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04344-112">Delegated (work or school account)</span></span> | <span data-ttu-id="04344-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04344-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="04344-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04344-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04344-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04344-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="04344-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="04344-116">Application</span></span> | <span data-ttu-id="04344-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04344-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04344-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04344-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="04344-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="04344-119">Optional request headers</span></span>

| <span data-ttu-id="04344-120">名称</span><span class="sxs-lookup"><span data-stu-id="04344-120">Name</span></span>          | <span data-ttu-id="04344-121">类型</span><span class="sxs-lookup"><span data-stu-id="04344-121">Type</span></span>   | <span data-ttu-id="04344-122">说明</span><span class="sxs-lookup"><span data-stu-id="04344-122">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="04344-123">if-match</span><span class="sxs-lookup"><span data-stu-id="04344-123">if-match</span></span>      | <span data-ttu-id="04344-124">String</span><span class="sxs-lookup"><span data-stu-id="04344-124">String</span></span> | <span data-ttu-id="04344-125">如果包含此请求标头，且提供的 eTag（或 cTag）与文件夹上的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应。</span><span class="sxs-lookup"><span data-stu-id="04344-125">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04344-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="04344-126">Request body</span></span>

<span data-ttu-id="04344-p103">在请求正文中，提供 **parentReference** 属性的新值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="04344-p103">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="04344-130">**注意：**将项目移动到驱动器的根目录时，应用无法使用 `"id:" "root"` 语法。</span><span class="sxs-lookup"><span data-stu-id="04344-130">**Note:** When moving items to the root of a drive your app cannot use the `"id:" "root"` syntax.</span></span>
<span data-ttu-id="04344-131">应用需要为父引用提供根文件夹的实际 ID。</span><span class="sxs-lookup"><span data-stu-id="04344-131">Your app needs to provide the actual ID of the root folder for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="04344-132">响应</span><span class="sxs-lookup"><span data-stu-id="04344-132">Response</span></span>

<span data-ttu-id="04344-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [DriveItem](../resources/driveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="04344-133">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04344-134">示例</span><span class="sxs-lookup"><span data-stu-id="04344-134">Example</span></span>

<span data-ttu-id="04344-135">本示例将由 {item-id} 指定的项目移动到 ID 为 `new-parent-folder-id` 的用户驱动器的文件夹中。</span><span class="sxs-lookup"><span data-stu-id="04344-135">This example moves an item specified by {item-id} into the `new-parent-folder-id` folder in the user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "move-item", "scopes": "files.readwrite" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "parentReference": {
    "id": "new-parent-folder-id"
  },
  "name": "new-item-name.txt"
}
```

### <a name="response"></a><span data-ttu-id="04344-136">响应</span><span class="sxs-lookup"><span data-stu-id="04344-136">Response</span></span>

<span data-ttu-id="04344-137">以下示例显示此移动请求的响应。</span><span class="sxs-lookup"><span data-stu-id="04344-137">The following example shows the response for this move request.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="04344-138">错误响应</span><span class="sxs-lookup"><span data-stu-id="04344-138">Error responses</span></span>

<span data-ttu-id="04344-139">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="04344-139">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md

<!-- {
  "type": "#page.annotation",
  "description": "Move an item to another location or rename the item.",
  "keywords": "move,rename,mv,change location",
  "section": "documentation",
  "tocPath": "Items/Move"
} -->
