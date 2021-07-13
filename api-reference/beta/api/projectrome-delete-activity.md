---
title: 删除活动
description: 删除应用的现有用户活动。
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ailae
ms.openlocfilehash: d30fda3d79a7afe6f370a735f6ed6e331fba714b
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401517"
---
# <a name="delete-an-activity"></a><span data-ttu-id="6912a-103">删除活动</span><span class="sxs-lookup"><span data-stu-id="6912a-103">Delete an activity</span></span>

<span data-ttu-id="6912a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6912a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6912a-105">删除应用的现有用户活动。</span><span class="sxs-lookup"><span data-stu-id="6912a-105">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="6912a-106">权限</span><span class="sxs-lookup"><span data-stu-id="6912a-106">Permissions</span></span>

<span data-ttu-id="6912a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6912a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6912a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6912a-109">Permission type</span></span>      | <span data-ttu-id="6912a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6912a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6912a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6912a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6912a-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="6912a-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="6912a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6912a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6912a-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="6912a-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="6912a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6912a-115">Application</span></span> | <span data-ttu-id="6912a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6912a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6912a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6912a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6912a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6912a-118">Request headers</span></span>

|<span data-ttu-id="6912a-119">名称</span><span class="sxs-lookup"><span data-stu-id="6912a-119">Name</span></span> | <span data-ttu-id="6912a-120">类型</span><span class="sxs-lookup"><span data-stu-id="6912a-120">Type</span></span> | <span data-ttu-id="6912a-121">说明</span><span class="sxs-lookup"><span data-stu-id="6912a-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="6912a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6912a-122">Authorization</span></span> | <span data-ttu-id="6912a-123">string</span><span class="sxs-lookup"><span data-stu-id="6912a-123">string</span></span> | <span data-ttu-id="6912a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6912a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6912a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6912a-126">Request body</span></span>

<span data-ttu-id="6912a-127">无请求正文。</span><span class="sxs-lookup"><span data-stu-id="6912a-127">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="6912a-128">响应</span><span class="sxs-lookup"><span data-stu-id="6912a-128">Response</span></span>

<span data-ttu-id="6912a-129">如果成功，如果 `204 No Content` 活动被删除，此方法将返回 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6912a-129">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="6912a-130">示例</span><span class="sxs-lookup"><span data-stu-id="6912a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6912a-131">请求</span><span class="sxs-lookup"><span data-stu-id="6912a-131">Request</span></span>

<span data-ttu-id="6912a-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6912a-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6912a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6912a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```
# <a name="c"></a>[<span data-ttu-id="6912a-134">C#</span><span class="sxs-lookup"><span data-stu-id="6912a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6912a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6912a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6912a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6912a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6912a-137">Java</span><span class="sxs-lookup"><span data-stu-id="6912a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-activity-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6912a-138">响应</span><span class="sxs-lookup"><span data-stu-id="6912a-138">Response</span></span>

<span data-ttu-id="6912a-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6912a-139">The following is an example of the response.</span></span>

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


