---
title: 删除 timeOffRequest
description: 删除 timeOffRequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6f5af597174d6146c50d88a3038af1af0158c931
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044065"
---
# <a name="delete-timeoffrequest"></a><span data-ttu-id="cb2ad-103">删除 timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="cb2ad-103">Delete timeOffRequest</span></span>

<span data-ttu-id="cb2ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb2ad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb2ad-105">删除 [timeOffRequest](../resources/timeoffrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-105">Delete a [timeOffRequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb2ad-106">权限</span><span class="sxs-lookup"><span data-stu-id="cb2ad-106">Permissions</span></span>

<span data-ttu-id="cb2ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb2ad-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb2ad-109">Permission type</span></span>                        | <span data-ttu-id="cb2ad-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb2ad-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="cb2ad-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb2ad-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cb2ad-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="cb2ad-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cb2ad-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb2ad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb2ad-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-114">Not supported.</span></span>    |
|<span data-ttu-id="cb2ad-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb2ad-115">Application</span></span> | <span data-ttu-id="cb2ad-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb2ad-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="cb2ad-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="cb2ad-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="cb2ad-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb2ad-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="cb2ad-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb2ad-120">Request headers</span></span>

| <span data-ttu-id="cb2ad-121">名称</span><span class="sxs-lookup"><span data-stu-id="cb2ad-121">Name</span></span>          | <span data-ttu-id="cb2ad-122">说明</span><span class="sxs-lookup"><span data-stu-id="cb2ad-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cb2ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb2ad-123">Authorization</span></span> | <span data-ttu-id="cb2ad-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb2ad-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb2ad-126">Request body</span></span>

<span data-ttu-id="cb2ad-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb2ad-128">响应</span><span class="sxs-lookup"><span data-stu-id="cb2ad-128">Response</span></span>

<span data-ttu-id="cb2ad-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb2ad-131">示例</span><span class="sxs-lookup"><span data-stu-id="cb2ad-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb2ad-132">请求</span><span class="sxs-lookup"><span data-stu-id="cb2ad-132">Request</span></span>

<span data-ttu-id="cb2ad-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cb2ad-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb2ad-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_timeoffrequest"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="cb2ad-135">C#</span><span class="sxs-lookup"><span data-stu-id="cb2ad-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb2ad-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb2ad-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb2ad-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb2ad-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb2ad-138">Java</span><span class="sxs-lookup"><span data-stu-id="cb2ad-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-timeoffrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="cb2ad-139">响应</span><span class="sxs-lookup"><span data-stu-id="cb2ad-139">Response</span></span>

<span data-ttu-id="cb2ad-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

