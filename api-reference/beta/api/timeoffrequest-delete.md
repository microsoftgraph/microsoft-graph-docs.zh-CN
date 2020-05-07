---
title: 删除 timeOffRequest
description: 删除 timeOffRequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: baa7ed94a438c1b40a5f70c7bc12e166450b023d
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154351"
---
# <a name="delete-timeoffrequest"></a><span data-ttu-id="cf06e-103">删除 timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="cf06e-103">Delete timeOffRequest</span></span>

<span data-ttu-id="cf06e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf06e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf06e-105">删除[timeOffRequest](../resources/timeoffrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cf06e-105">Delete a [timeOffRequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf06e-106">权限</span><span class="sxs-lookup"><span data-stu-id="cf06e-106">Permissions</span></span>

<span data-ttu-id="cf06e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf06e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf06e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf06e-109">Permission type</span></span>                        | <span data-ttu-id="cf06e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf06e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cf06e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf06e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf06e-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf06e-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="cf06e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf06e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf06e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf06e-114">Not supported.</span></span> |
|<span data-ttu-id="cf06e-115">Application</span><span class="sxs-lookup"><span data-stu-id="cf06e-115">Application</span></span> | <span data-ttu-id="cf06e-116">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="cf06e-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="cf06e-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="cf06e-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="cf06e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf06e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="cf06e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf06e-119">Request headers</span></span>

| <span data-ttu-id="cf06e-120">名称</span><span class="sxs-lookup"><span data-stu-id="cf06e-120">Name</span></span>          | <span data-ttu-id="cf06e-121">说明</span><span class="sxs-lookup"><span data-stu-id="cf06e-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cf06e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf06e-122">Authorization</span></span> | <span data-ttu-id="cf06e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cf06e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf06e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf06e-125">Request body</span></span>

<span data-ttu-id="cf06e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf06e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf06e-127">响应</span><span class="sxs-lookup"><span data-stu-id="cf06e-127">Response</span></span>

<span data-ttu-id="cf06e-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cf06e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cf06e-130">示例</span><span class="sxs-lookup"><span data-stu-id="cf06e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cf06e-131">请求</span><span class="sxs-lookup"><span data-stu-id="cf06e-131">Request</span></span>

<span data-ttu-id="cf06e-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cf06e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf06e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf06e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_timeoffrequest"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="cf06e-134">C#</span><span class="sxs-lookup"><span data-stu-id="cf06e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf06e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf06e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf06e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf06e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cf06e-137">响应</span><span class="sxs-lookup"><span data-stu-id="cf06e-137">Response</span></span>

<span data-ttu-id="cf06e-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cf06e-138">The following is an example of the response.</span></span>

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
