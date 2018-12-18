---
title: 永久删除项目
description: 永久删除已删除的项目中的项目
author: lleonard-msft
ms.openlocfilehash: cdea85ee1b46b4d3c7156a599081a93f31318eac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336468"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="15621-103">永久删除项目</span><span class="sxs-lookup"><span data-stu-id="15621-103">Permanently delete item</span></span>

> <span data-ttu-id="15621-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="15621-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15621-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="15621-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15621-106">永久删除[已删除的项目](../resources/directory.md)中的项目</span><span class="sxs-lookup"><span data-stu-id="15621-106">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="15621-107">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="15621-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="15621-108">可以永久删除“已删除的项目”中的项目。</span><span class="sxs-lookup"><span data-stu-id="15621-108">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="15621-109">但当某个项目永久删除后，将**无法**还原。</span><span class="sxs-lookup"><span data-stu-id="15621-109">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="15621-110">权限</span><span class="sxs-lookup"><span data-stu-id="15621-110">Permissions</span></span>
<span data-ttu-id="15621-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="15621-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="15621-113">用户： User.ReadWrite.All、 Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="15621-113">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="15621-114">组： Group.ReadWrite.All、 Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="15621-114">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="15621-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15621-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="15621-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="15621-116">Request headers</span></span>
| <span data-ttu-id="15621-117">Name</span><span class="sxs-lookup"><span data-stu-id="15621-117">Name</span></span>       | <span data-ttu-id="15621-118">说明</span><span class="sxs-lookup"><span data-stu-id="15621-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="15621-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="15621-119">Authorization</span></span>  | <span data-ttu-id="15621-120">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="15621-120">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="15621-121">Accept</span><span class="sxs-lookup"><span data-stu-id="15621-121">Accept</span></span>  | <span data-ttu-id="15621-122">application/json</span><span class="sxs-lookup"><span data-stu-id="15621-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="15621-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="15621-123">Request body</span></span>
<span data-ttu-id="15621-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="15621-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15621-125">响应</span><span class="sxs-lookup"><span data-stu-id="15621-125">Response</span></span>

<span data-ttu-id="15621-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="15621-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15621-128">示例</span><span class="sxs-lookup"><span data-stu-id="15621-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15621-129">请求</span><span class="sxs-lookup"><span data-stu-id="15621-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="15621-130">响应</span><span class="sxs-lookup"><span data-stu-id="15621-130">Response</span></span>
<span data-ttu-id="15621-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="15621-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->