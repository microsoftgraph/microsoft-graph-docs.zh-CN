---
title: 删除 timeOffRequest
description: 删除 timeOffRequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c860c1948d798ec949b9ed611882d65a22b7ad93
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452270"
---
# <a name="delete-timeoffrequest"></a><span data-ttu-id="26b3c-103">删除 timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="26b3c-103">Delete timeOffRequest</span></span>

<span data-ttu-id="26b3c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="26b3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26b3c-105">删除[timeOffRequest](../resources/timeoffrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="26b3c-105">Delete a [timeOffRequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="26b3c-106">权限</span><span class="sxs-lookup"><span data-stu-id="26b3c-106">Permissions</span></span>

<span data-ttu-id="26b3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26b3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26b3c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="26b3c-109">Permission type</span></span>                        | <span data-ttu-id="26b3c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26b3c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="26b3c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26b3c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="26b3c-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b3c-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="26b3c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26b3c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26b3c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="26b3c-114">Not supported.</span></span> |
|<span data-ttu-id="26b3c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="26b3c-115">Application</span></span> | <span data-ttu-id="26b3c-116">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="26b3c-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="26b3c-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="26b3c-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="26b3c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26b3c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/timeOffRequests
```

## <a name="request-headers"></a><span data-ttu-id="26b3c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="26b3c-119">Request headers</span></span>

| <span data-ttu-id="26b3c-120">名称</span><span class="sxs-lookup"><span data-stu-id="26b3c-120">Name</span></span>          | <span data-ttu-id="26b3c-121">说明</span><span class="sxs-lookup"><span data-stu-id="26b3c-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="26b3c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26b3c-122">Authorization</span></span> | <span data-ttu-id="26b3c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="26b3c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26b3c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="26b3c-125">Request body</span></span>

<span data-ttu-id="26b3c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="26b3c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26b3c-127">响应</span><span class="sxs-lookup"><span data-stu-id="26b3c-127">Response</span></span>

<span data-ttu-id="26b3c-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="26b3c-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26b3c-130">示例</span><span class="sxs-lookup"><span data-stu-id="26b3c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26b3c-131">请求</span><span class="sxs-lookup"><span data-stu-id="26b3c-131">Request</span></span>

<span data-ttu-id="26b3c-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26b3c-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26b3c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="26b3c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_timeoffrequest"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests
```
# <a name="c"></a>[<span data-ttu-id="26b3c-134">C#</span><span class="sxs-lookup"><span data-stu-id="26b3c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26b3c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26b3c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26b3c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26b3c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="26b3c-137">响应</span><span class="sxs-lookup"><span data-stu-id="26b3c-137">Response</span></span>

<span data-ttu-id="26b3c-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="26b3c-138">The following is an example of the response.</span></span>

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
