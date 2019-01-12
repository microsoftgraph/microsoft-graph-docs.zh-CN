---
title: 删除 plannerTask
description: 删除 **plannerTask**。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 0130a0599b075ea99c9022e4bb3a99838301b790
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948651"
---
# <a name="delete-plannertask"></a><span data-ttu-id="3e8ba-103">删除 plannerTask</span><span class="sxs-lookup"><span data-stu-id="3e8ba-103">Delete plannerTask</span></span>

<span data-ttu-id="3e8ba-104">删除 **plannerTask**。</span><span class="sxs-lookup"><span data-stu-id="3e8ba-104">Delete **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e8ba-105">权限</span><span class="sxs-lookup"><span data-stu-id="3e8ba-105">Permissions</span></span>
<span data-ttu-id="3e8ba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e8ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e8ba-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e8ba-108">Permission type</span></span>      | <span data-ttu-id="3e8ba-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e8ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e8ba-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e8ba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3e8ba-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e8ba-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3e8ba-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e8ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e8ba-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e8ba-113">Not supported.</span></span>    |
|<span data-ttu-id="3e8ba-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e8ba-114">Application</span></span> | <span data-ttu-id="3e8ba-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e8ba-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e8ba-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e8ba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/tasks/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3e8ba-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e8ba-117">Request headers</span></span>
| <span data-ttu-id="3e8ba-118">名称</span><span class="sxs-lookup"><span data-stu-id="3e8ba-118">Name</span></span>       | <span data-ttu-id="3e8ba-119">说明</span><span class="sxs-lookup"><span data-stu-id="3e8ba-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3e8ba-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e8ba-120">Authorization</span></span>  | <span data-ttu-id="3e8ba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e8ba-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e8ba-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="3e8ba-123">If-Match</span></span>  | <span data-ttu-id="3e8ba-p103">要删除的 **plannerTask** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="3e8ba-p103">Last known ETag value for the **plannerTask** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e8ba-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e8ba-126">Request body</span></span>
<span data-ttu-id="3e8ba-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3e8ba-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e8ba-128">响应</span><span class="sxs-lookup"><span data-stu-id="3e8ba-128">Response</span></span>

<span data-ttu-id="3e8ba-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3e8ba-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="3e8ba-p105">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="3e8ba-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="3e8ba-134">示例</span><span class="sxs-lookup"><span data-stu-id="3e8ba-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e8ba-135">请求</span><span class="sxs-lookup"><span data-stu-id="3e8ba-135">Request</span></span>
<span data-ttu-id="3e8ba-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3e8ba-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_plannertask"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/planner/tasks/{id}
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a><span data-ttu-id="3e8ba-137">响应</span><span class="sxs-lookup"><span data-stu-id="3e8ba-137">Response</span></span>
<span data-ttu-id="3e8ba-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3e8ba-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
