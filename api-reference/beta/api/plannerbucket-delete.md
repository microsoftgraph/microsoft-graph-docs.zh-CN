---
title: 删除 plannerBucket
description: 删除 **plannerBucket**。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: d1c3f0540b3a27a396229fa19dac2bcfe3a231de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933223"
---
# <a name="delete-plannerbucket"></a><span data-ttu-id="c37ff-103">删除 plannerBucket</span><span class="sxs-lookup"><span data-stu-id="c37ff-103">Delete plannerBucket</span></span>

> <span data-ttu-id="c37ff-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c37ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c37ff-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c37ff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c37ff-106">删除 **plannerBucket**。</span><span class="sxs-lookup"><span data-stu-id="c37ff-106">Delete **plannerBucket**.</span></span>
## <a name="permissions"></a><span data-ttu-id="c37ff-107">权限</span><span class="sxs-lookup"><span data-stu-id="c37ff-107">Permissions</span></span>
<span data-ttu-id="c37ff-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c37ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c37ff-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c37ff-110">Permission type</span></span>      | <span data-ttu-id="c37ff-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c37ff-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c37ff-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c37ff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c37ff-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c37ff-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c37ff-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c37ff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c37ff-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c37ff-115">Not supported.</span></span>    |
|<span data-ttu-id="c37ff-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c37ff-116">Application</span></span> | <span data-ttu-id="c37ff-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c37ff-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c37ff-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c37ff-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/buckets/<id>
```
## <a name="request-headers"></a><span data-ttu-id="c37ff-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c37ff-119">Request headers</span></span>
| <span data-ttu-id="c37ff-120">名称</span><span class="sxs-lookup"><span data-stu-id="c37ff-120">Name</span></span>       | <span data-ttu-id="c37ff-121">说明</span><span class="sxs-lookup"><span data-stu-id="c37ff-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c37ff-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c37ff-122">Authorization</span></span>  | <span data-ttu-id="c37ff-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c37ff-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c37ff-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="c37ff-125">If-Match</span></span>  | <span data-ttu-id="c37ff-p104">要删除的 **plannerBucket** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="c37ff-p104">Last known ETag value for the **plannerBucket** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c37ff-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c37ff-128">Request body</span></span>
<span data-ttu-id="c37ff-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c37ff-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c37ff-130">响应</span><span class="sxs-lookup"><span data-stu-id="c37ff-130">Response</span></span>

<span data-ttu-id="c37ff-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c37ff-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="c37ff-p106">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="c37ff-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="c37ff-136">示例</span><span class="sxs-lookup"><span data-stu-id="c37ff-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c37ff-137">请求</span><span class="sxs-lookup"><span data-stu-id="c37ff-137">Request</span></span>
<span data-ttu-id="c37ff-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c37ff-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_plannerbucket"
}-->
```http
DELETE https://graph.microsoft.com/beta/planner/buckets/<id>
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a><span data-ttu-id="c37ff-139">响应</span><span class="sxs-lookup"><span data-stu-id="c37ff-139">Response</span></span>
<span data-ttu-id="c37ff-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c37ff-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
