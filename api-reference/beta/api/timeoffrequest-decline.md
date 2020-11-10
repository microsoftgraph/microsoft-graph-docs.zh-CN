---
title: timeOffRequest：拒绝
description: 拒绝 timeoffrequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9fb4432cc9cf05689ec26a6b8ebe8b0447f33ca6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981352"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="b99b1-103">timeOffRequest：拒绝</span><span class="sxs-lookup"><span data-stu-id="b99b1-103">timeOffRequest: decline</span></span>

<span data-ttu-id="b99b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b99b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b99b1-105">拒绝 [timeoffrequest](../resources/timeoffrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b99b1-105">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b99b1-106">权限</span><span class="sxs-lookup"><span data-stu-id="b99b1-106">Permissions</span></span>

<span data-ttu-id="b99b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b99b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b99b1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b99b1-109">Permission type</span></span>                        | <span data-ttu-id="b99b1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b99b1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b99b1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b99b1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b99b1-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b99b1-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="b99b1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b99b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b99b1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b99b1-114">Not supported.</span></span> |
|<span data-ttu-id="b99b1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b99b1-115">Application</span></span> | <span data-ttu-id="b99b1-116">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="b99b1-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="b99b1-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="b99b1-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="b99b1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b99b1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="b99b1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b99b1-119">Request headers</span></span>

| <span data-ttu-id="b99b1-120">名称</span><span class="sxs-lookup"><span data-stu-id="b99b1-120">Name</span></span>          | <span data-ttu-id="b99b1-121">说明</span><span class="sxs-lookup"><span data-stu-id="b99b1-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b99b1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b99b1-122">Authorization</span></span> | <span data-ttu-id="b99b1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b99b1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b99b1-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="b99b1-125">Content-type</span></span> | <span data-ttu-id="b99b1-126">application-json。</span><span class="sxs-lookup"><span data-stu-id="b99b1-126">application-json.</span></span> <span data-ttu-id="b99b1-127">必填。</span><span class="sxs-lookup"><span data-stu-id="b99b1-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b99b1-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b99b1-128">Request body</span></span>

<span data-ttu-id="b99b1-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b99b1-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b99b1-130">参数</span><span class="sxs-lookup"><span data-stu-id="b99b1-130">Parameter</span></span>    | <span data-ttu-id="b99b1-131">类型</span><span class="sxs-lookup"><span data-stu-id="b99b1-131">Type</span></span>        | <span data-ttu-id="b99b1-132">描述</span><span class="sxs-lookup"><span data-stu-id="b99b1-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b99b1-133">message</span><span class="sxs-lookup"><span data-stu-id="b99b1-133">message</span></span>|<span data-ttu-id="b99b1-134">String</span><span class="sxs-lookup"><span data-stu-id="b99b1-134">String</span></span>|<span data-ttu-id="b99b1-135">自定义拒绝邮件。</span><span class="sxs-lookup"><span data-stu-id="b99b1-135">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="b99b1-136">响应</span><span class="sxs-lookup"><span data-stu-id="b99b1-136">Response</span></span>

<span data-ttu-id="b99b1-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b99b1-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b99b1-139">示例</span><span class="sxs-lookup"><span data-stu-id="b99b1-139">Examples</span></span>

<span data-ttu-id="b99b1-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b99b1-140">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="b99b1-141">请求</span><span class="sxs-lookup"><span data-stu-id="b99b1-141">Request</span></span>

<span data-ttu-id="b99b1-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b99b1-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b99b1-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="b99b1-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="javascript"></a>[<span data-ttu-id="b99b1-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b99b1-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b99b1-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b99b1-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="b99b1-146">C#</span><span class="sxs-lookup"><span data-stu-id="b99b1-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b99b1-147">Java</span><span class="sxs-lookup"><span data-stu-id="b99b1-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffrequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b99b1-148">响应</span><span class="sxs-lookup"><span data-stu-id="b99b1-148">Response</span></span>

<span data-ttu-id="b99b1-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b99b1-149">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeOffRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


