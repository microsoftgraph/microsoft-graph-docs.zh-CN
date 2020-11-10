---
title: 删除 timeOffRequest
description: 删除 timeOffRequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f185c8a9e4c3d0b3bb4f8286e0c4f7252e13692e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981342"
---
# <a name="delete-timeoffrequest"></a><span data-ttu-id="3dbf9-103">删除 timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="3dbf9-103">Delete timeOffRequest</span></span>

<span data-ttu-id="3dbf9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3dbf9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dbf9-105">删除 [timeOffRequest](../resources/timeoffrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3dbf9-105">Delete a [timeOffRequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3dbf9-106">权限</span><span class="sxs-lookup"><span data-stu-id="3dbf9-106">Permissions</span></span>

<span data-ttu-id="3dbf9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3dbf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3dbf9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3dbf9-109">Permission type</span></span>                        | <span data-ttu-id="3dbf9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3dbf9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3dbf9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3dbf9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3dbf9-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dbf9-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="3dbf9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3dbf9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dbf9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3dbf9-114">Not supported.</span></span> |
|<span data-ttu-id="3dbf9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3dbf9-115">Application</span></span> | <span data-ttu-id="3dbf9-116">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="3dbf9-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="3dbf9-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="3dbf9-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="3dbf9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3dbf9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="3dbf9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3dbf9-119">Request headers</span></span>

| <span data-ttu-id="3dbf9-120">名称</span><span class="sxs-lookup"><span data-stu-id="3dbf9-120">Name</span></span>          | <span data-ttu-id="3dbf9-121">说明</span><span class="sxs-lookup"><span data-stu-id="3dbf9-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3dbf9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3dbf9-122">Authorization</span></span> | <span data-ttu-id="3dbf9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3dbf9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3dbf9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3dbf9-125">Request body</span></span>

<span data-ttu-id="3dbf9-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3dbf9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3dbf9-127">响应</span><span class="sxs-lookup"><span data-stu-id="3dbf9-127">Response</span></span>

<span data-ttu-id="3dbf9-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3dbf9-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3dbf9-130">示例</span><span class="sxs-lookup"><span data-stu-id="3dbf9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3dbf9-131">请求</span><span class="sxs-lookup"><span data-stu-id="3dbf9-131">Request</span></span>

<span data-ttu-id="3dbf9-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3dbf9-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3dbf9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dbf9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_timeoffrequest"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="3dbf9-134">C#</span><span class="sxs-lookup"><span data-stu-id="3dbf9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dbf9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dbf9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dbf9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dbf9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3dbf9-137">Java</span><span class="sxs-lookup"><span data-stu-id="3dbf9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-timeoffrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3dbf9-138">响应</span><span class="sxs-lookup"><span data-stu-id="3dbf9-138">Response</span></span>

<span data-ttu-id="3dbf9-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3dbf9-139">The following is an example of the response.</span></span>

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


