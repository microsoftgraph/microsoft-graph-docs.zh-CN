---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 删除文件或文件夹
localization_priority: Normal
ms.openlocfilehash: 8357b170023f905494df73ca1e4420f87a914a77
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843363"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="04970-102">删除 DriveItem</span><span class="sxs-lookup"><span data-stu-id="04970-102">Delete a DriveItem</span></span>

> <span data-ttu-id="04970-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="04970-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04970-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="04970-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="04970-p102">通过使用其 ID 或路径删除 [DriveItem](../resources/driveitem.md)。注意，使用此方法删除项将把项移动到回收站中，而不是永久删除该项。</span><span class="sxs-lookup"><span data-stu-id="04970-p102">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="04970-107">权限</span><span class="sxs-lookup"><span data-stu-id="04970-107">Permissions</span></span>

<span data-ttu-id="04970-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="04970-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04970-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="04970-110">Permission type</span></span>      | <span data-ttu-id="04970-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="04970-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04970-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04970-112">Delegated (work or school account)</span></span> | <span data-ttu-id="04970-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04970-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="04970-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04970-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04970-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04970-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="04970-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="04970-116">Application</span></span> | <span data-ttu-id="04970-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04970-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04970-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04970-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="04970-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="04970-119">Optional request headers</span></span>

| <span data-ttu-id="04970-120">名称</span><span class="sxs-lookup"><span data-stu-id="04970-120">Name</span></span>          | <span data-ttu-id="04970-121">类型</span><span class="sxs-lookup"><span data-stu-id="04970-121">Type</span></span>   | <span data-ttu-id="04970-122">说明</span><span class="sxs-lookup"><span data-stu-id="04970-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="04970-123">if-match</span><span class="sxs-lookup"><span data-stu-id="04970-123">if-match</span></span>      | <span data-ttu-id="04970-124">String</span><span class="sxs-lookup"><span data-stu-id="04970-124">String</span></span> | <span data-ttu-id="04970-125">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="04970-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="04970-126">示例</span><span class="sxs-lookup"><span data-stu-id="04970-126">Example</span></span>

<span data-ttu-id="04970-127">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="04970-127">Here is an example of how to call this API.</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE /me/drive/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="04970-128">响应</span><span class="sxs-lookup"><span data-stu-id="04970-128">Response</span></span>

<span data-ttu-id="04970-129">如果成功，此调用将返回 `204 No Content` 响应，以指明资源已被删除，没有可返回的内容。</span><span class="sxs-lookup"><span data-stu-id="04970-129">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a><span data-ttu-id="04970-130">错误响应</span><span class="sxs-lookup"><span data-stu-id="04970-130">Error responses</span></span>

<span data-ttu-id="04970-131">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="04970-131">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete"
} -->
