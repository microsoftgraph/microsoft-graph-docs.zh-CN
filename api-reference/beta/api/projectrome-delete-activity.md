---
title: 删除活动
description: 删除应用程序的现有用户活动。
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ailae
ms.openlocfilehash: 293c6abe64aec124f280e5e33239f63339753733
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010590"
---
# <a name="delete-an-activity"></a><span data-ttu-id="fc35d-103">删除活动</span><span class="sxs-lookup"><span data-stu-id="fc35d-103">Delete an activity</span></span>

<span data-ttu-id="fc35d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc35d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc35d-105">删除应用程序的现有用户活动。</span><span class="sxs-lookup"><span data-stu-id="fc35d-105">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc35d-106">权限</span><span class="sxs-lookup"><span data-stu-id="fc35d-106">Permissions</span></span>

<span data-ttu-id="fc35d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc35d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fc35d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc35d-109">Permission type</span></span>      | <span data-ttu-id="fc35d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc35d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc35d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc35d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fc35d-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="fc35d-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="fc35d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc35d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc35d-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="fc35d-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="fc35d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc35d-115">Application</span></span> | <span data-ttu-id="fc35d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc35d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc35d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc35d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fc35d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc35d-118">Request headers</span></span>

|<span data-ttu-id="fc35d-119">名称</span><span class="sxs-lookup"><span data-stu-id="fc35d-119">Name</span></span> | <span data-ttu-id="fc35d-120">类型</span><span class="sxs-lookup"><span data-stu-id="fc35d-120">Type</span></span> | <span data-ttu-id="fc35d-121">说明</span><span class="sxs-lookup"><span data-stu-id="fc35d-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="fc35d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc35d-122">Authorization</span></span> | <span data-ttu-id="fc35d-123">string</span><span class="sxs-lookup"><span data-stu-id="fc35d-123">string</span></span> | <span data-ttu-id="fc35d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fc35d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc35d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc35d-126">Request body</span></span>

<span data-ttu-id="fc35d-127">无请求正文。</span><span class="sxs-lookup"><span data-stu-id="fc35d-127">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="fc35d-128">响应</span><span class="sxs-lookup"><span data-stu-id="fc35d-128">Response</span></span>

<span data-ttu-id="fc35d-129">如果成功，此方法将返回 `204 No Content` 响应代码（如果活动已删除）。</span><span class="sxs-lookup"><span data-stu-id="fc35d-129">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="fc35d-130">示例</span><span class="sxs-lookup"><span data-stu-id="fc35d-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fc35d-131">请求</span><span class="sxs-lookup"><span data-stu-id="fc35d-131">Request</span></span>

<span data-ttu-id="fc35d-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc35d-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fc35d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc35d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```
# <a name="c"></a>[<span data-ttu-id="fc35d-134">C#</span><span class="sxs-lookup"><span data-stu-id="fc35d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc35d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc35d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc35d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc35d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fc35d-137">响应</span><span class="sxs-lookup"><span data-stu-id="fc35d-137">Response</span></span>

<span data-ttu-id="fc35d-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fc35d-138">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


