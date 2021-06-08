---
title: timeOffRequest： decline
description: 拒绝 timeoffrequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7f9e5f6151e30dbbfcfc74db51a9a8e2afacab1c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787420"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="8f654-103">timeOffRequest： decline</span><span class="sxs-lookup"><span data-stu-id="8f654-103">timeOffRequest: decline</span></span>

<span data-ttu-id="8f654-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f654-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8f654-105">拒绝 [timeoffrequest](../resources/timeoffrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8f654-105">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f654-106">权限</span><span class="sxs-lookup"><span data-stu-id="8f654-106">Permissions</span></span>

<span data-ttu-id="8f654-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f654-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f654-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f654-109">Permission type</span></span>                        | <span data-ttu-id="8f654-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f654-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="8f654-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f654-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8f654-112">Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f654-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8f654-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f654-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f654-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f654-114">Not supported.</span></span>    |
|<span data-ttu-id="8f654-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f654-115">Application</span></span> | <span data-ttu-id="8f654-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f654-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="8f654-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="8f654-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8f654-118">全局管理员可以访问他们不是其成员组。</span><span class="sxs-lookup"><span data-stu-id="8f654-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8f654-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f654-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="8f654-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f654-120">Request headers</span></span>

| <span data-ttu-id="8f654-121">名称</span><span class="sxs-lookup"><span data-stu-id="8f654-121">Name</span></span>          | <span data-ttu-id="8f654-122">说明</span><span class="sxs-lookup"><span data-stu-id="8f654-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8f654-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f654-123">Authorization</span></span> | <span data-ttu-id="8f654-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f654-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f654-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="8f654-126">Content-type</span></span> | <span data-ttu-id="8f654-127">application-json。</span><span class="sxs-lookup"><span data-stu-id="8f654-127">application-json.</span></span> <span data-ttu-id="8f654-128">必填。</span><span class="sxs-lookup"><span data-stu-id="8f654-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f654-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f654-129">Request body</span></span>

<span data-ttu-id="8f654-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8f654-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8f654-131">参数</span><span class="sxs-lookup"><span data-stu-id="8f654-131">Parameter</span></span>    | <span data-ttu-id="8f654-132">类型</span><span class="sxs-lookup"><span data-stu-id="8f654-132">Type</span></span>        | <span data-ttu-id="8f654-133">描述</span><span class="sxs-lookup"><span data-stu-id="8f654-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8f654-134">message</span><span class="sxs-lookup"><span data-stu-id="8f654-134">message</span></span>|<span data-ttu-id="8f654-135">String</span><span class="sxs-lookup"><span data-stu-id="8f654-135">String</span></span>|<span data-ttu-id="8f654-136">自定义拒绝邮件。</span><span class="sxs-lookup"><span data-stu-id="8f654-136">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="8f654-137">响应</span><span class="sxs-lookup"><span data-stu-id="8f654-137">Response</span></span>

<span data-ttu-id="8f654-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8f654-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f654-140">示例</span><span class="sxs-lookup"><span data-stu-id="8f654-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f654-141">请求</span><span class="sxs-lookup"><span data-stu-id="8f654-141">Request</span></span>

<span data-ttu-id="8f654-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8f654-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8f654-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f654-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8f654-144">C#</span><span class="sxs-lookup"><span data-stu-id="8f654-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f654-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f654-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f654-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f654-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f654-147">Java</span><span class="sxs-lookup"><span data-stu-id="8f654-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffrequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="8f654-148">响应</span><span class="sxs-lookup"><span data-stu-id="8f654-148">Response</span></span>

<span data-ttu-id="8f654-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8f654-149">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
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

