---
title: timeOffRequest：拒绝
description: 拒绝 timeoffrequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9d893dcf8f5557fa650b5eb1eefd8b00704874ee
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44215925"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="b0e8e-103">timeOffRequest：拒绝</span><span class="sxs-lookup"><span data-stu-id="b0e8e-103">timeOffRequest: decline</span></span>

<span data-ttu-id="b0e8e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0e8e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b0e8e-105">拒绝[timeoffrequest](../resources/timeoffrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b0e8e-105">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0e8e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b0e8e-106">Permissions</span></span>

<span data-ttu-id="b0e8e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0e8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0e8e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0e8e-109">Permission type</span></span>                        | <span data-ttu-id="b0e8e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0e8e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="b0e8e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0e8e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b0e8e-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="b0e8e-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b0e8e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0e8e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0e8e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0e8e-114">Not supported.</span></span>    |
|<span data-ttu-id="b0e8e-115">Application</span><span class="sxs-lookup"><span data-stu-id="b0e8e-115">Application</span></span> | <span data-ttu-id="b0e8e-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0e8e-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="b0e8e-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="b0e8e-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b0e8e-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="b0e8e-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b0e8e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0e8e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="b0e8e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0e8e-120">Request headers</span></span>

| <span data-ttu-id="b0e8e-121">名称</span><span class="sxs-lookup"><span data-stu-id="b0e8e-121">Name</span></span>          | <span data-ttu-id="b0e8e-122">说明</span><span class="sxs-lookup"><span data-stu-id="b0e8e-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b0e8e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0e8e-123">Authorization</span></span> | <span data-ttu-id="b0e8e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b0e8e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b0e8e-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="b0e8e-126">Content-type</span></span> | <span data-ttu-id="b0e8e-127">application-json。</span><span class="sxs-lookup"><span data-stu-id="b0e8e-127">application-json.</span></span> <span data-ttu-id="b0e8e-128">必填。</span><span class="sxs-lookup"><span data-stu-id="b0e8e-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0e8e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0e8e-129">Request body</span></span>

<span data-ttu-id="b0e8e-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b0e8e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b0e8e-131">参数</span><span class="sxs-lookup"><span data-stu-id="b0e8e-131">Parameter</span></span>    | <span data-ttu-id="b0e8e-132">类型</span><span class="sxs-lookup"><span data-stu-id="b0e8e-132">Type</span></span>        | <span data-ttu-id="b0e8e-133">描述</span><span class="sxs-lookup"><span data-stu-id="b0e8e-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b0e8e-134">message</span><span class="sxs-lookup"><span data-stu-id="b0e8e-134">message</span></span>|<span data-ttu-id="b0e8e-135">String</span><span class="sxs-lookup"><span data-stu-id="b0e8e-135">String</span></span>|<span data-ttu-id="b0e8e-136">自定义拒绝邮件。</span><span class="sxs-lookup"><span data-stu-id="b0e8e-136">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="b0e8e-137">响应</span><span class="sxs-lookup"><span data-stu-id="b0e8e-137">Response</span></span>

<span data-ttu-id="b0e8e-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b0e8e-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b0e8e-140">示例</span><span class="sxs-lookup"><span data-stu-id="b0e8e-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b0e8e-141">请求</span><span class="sxs-lookup"><span data-stu-id="b0e8e-141">Request</span></span>

<span data-ttu-id="b0e8e-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b0e8e-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b0e8e-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0e8e-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="b0e8e-144">C#</span><span class="sxs-lookup"><span data-stu-id="b0e8e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0e8e-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0e8e-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0e8e-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0e8e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b0e8e-147">Java</span><span class="sxs-lookup"><span data-stu-id="b0e8e-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffrequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="b0e8e-148">响应</span><span class="sxs-lookup"><span data-stu-id="b0e8e-148">Response</span></span>

<span data-ttu-id="b0e8e-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b0e8e-149">The following is an example of the response.</span></span>
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
