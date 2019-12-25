---
title: 删除 timeOffRequest
description: 删除 timeOffRequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 97587997d771fee433b72d54347dc05aa73acb72
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863592"
---
# <a name="delete-timeoffrequest"></a><span data-ttu-id="54725-103">删除 timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="54725-103">Delete timeOffRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54725-104">删除[timeOffRequest](../resources/timeoffrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="54725-104">Delete a [timeOffRequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="54725-105">权限</span><span class="sxs-lookup"><span data-stu-id="54725-105">Permissions</span></span>

<span data-ttu-id="54725-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54725-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54725-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="54725-108">Permission type</span></span>                        | <span data-ttu-id="54725-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="54725-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="54725-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54725-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="54725-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54725-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="54725-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54725-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54725-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="54725-113">Not supported.</span></span> |
|<span data-ttu-id="54725-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="54725-114">Application</span></span> | <span data-ttu-id="54725-115">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="54725-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="54725-116">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="54725-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="54725-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54725-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/timeOffRequests
```

## <a name="request-headers"></a><span data-ttu-id="54725-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="54725-118">Request headers</span></span>

| <span data-ttu-id="54725-119">名称</span><span class="sxs-lookup"><span data-stu-id="54725-119">Name</span></span>          | <span data-ttu-id="54725-120">说明</span><span class="sxs-lookup"><span data-stu-id="54725-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="54725-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="54725-121">Authorization</span></span> | <span data-ttu-id="54725-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="54725-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54725-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="54725-124">Request body</span></span>

<span data-ttu-id="54725-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="54725-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54725-126">响应</span><span class="sxs-lookup"><span data-stu-id="54725-126">Response</span></span>

<span data-ttu-id="54725-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="54725-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54725-129">示例</span><span class="sxs-lookup"><span data-stu-id="54725-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54725-130">请求</span><span class="sxs-lookup"><span data-stu-id="54725-130">Request</span></span>

<span data-ttu-id="54725-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="54725-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="54725-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="54725-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_timeoffrequest"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="54725-133">C#</span><span class="sxs-lookup"><span data-stu-id="54725-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="54725-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54725-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="54725-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54725-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="54725-136">响应</span><span class="sxs-lookup"><span data-stu-id="54725-136">Response</span></span>

<span data-ttu-id="54725-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="54725-137">The following is an example of the response.</span></span>

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
