---
title: timeOffRequest： decline
description: 拒绝 timeoffrequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0f745bea1f16680861c92fa8b4a5c18025c425da
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787315"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="73d40-103">timeOffRequest： decline</span><span class="sxs-lookup"><span data-stu-id="73d40-103">timeOffRequest: decline</span></span>

<span data-ttu-id="73d40-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73d40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73d40-105">拒绝 [timeoffrequest](../resources/timeoffrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73d40-105">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="73d40-106">权限</span><span class="sxs-lookup"><span data-stu-id="73d40-106">Permissions</span></span>

<span data-ttu-id="73d40-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73d40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73d40-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="73d40-109">Permission type</span></span>                        | <span data-ttu-id="73d40-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73d40-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="73d40-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73d40-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="73d40-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73d40-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="73d40-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73d40-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73d40-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73d40-114">Not supported.</span></span> |
|<span data-ttu-id="73d40-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="73d40-115">Application</span></span> | <span data-ttu-id="73d40-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="73d40-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="73d40-117">\***重要提示：** 应用程序权限目前仅为个人预览版，不可公开使用。</span><span class="sxs-lookup"><span data-stu-id="73d40-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="73d40-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73d40-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="73d40-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="73d40-119">Request headers</span></span>

| <span data-ttu-id="73d40-120">名称</span><span class="sxs-lookup"><span data-stu-id="73d40-120">Name</span></span>          | <span data-ttu-id="73d40-121">说明</span><span class="sxs-lookup"><span data-stu-id="73d40-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="73d40-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="73d40-122">Authorization</span></span> | <span data-ttu-id="73d40-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73d40-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73d40-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="73d40-125">Content-type</span></span> | <span data-ttu-id="73d40-126">application-json。</span><span class="sxs-lookup"><span data-stu-id="73d40-126">application-json.</span></span> <span data-ttu-id="73d40-127">必填。</span><span class="sxs-lookup"><span data-stu-id="73d40-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73d40-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="73d40-128">Request body</span></span>

<span data-ttu-id="73d40-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="73d40-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="73d40-130">参数</span><span class="sxs-lookup"><span data-stu-id="73d40-130">Parameter</span></span>    | <span data-ttu-id="73d40-131">类型</span><span class="sxs-lookup"><span data-stu-id="73d40-131">Type</span></span>        | <span data-ttu-id="73d40-132">描述</span><span class="sxs-lookup"><span data-stu-id="73d40-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="73d40-133">message</span><span class="sxs-lookup"><span data-stu-id="73d40-133">message</span></span>|<span data-ttu-id="73d40-134">String</span><span class="sxs-lookup"><span data-stu-id="73d40-134">String</span></span>|<span data-ttu-id="73d40-135">自定义拒绝邮件。</span><span class="sxs-lookup"><span data-stu-id="73d40-135">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="73d40-136">响应</span><span class="sxs-lookup"><span data-stu-id="73d40-136">Response</span></span>

<span data-ttu-id="73d40-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="73d40-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73d40-139">示例</span><span class="sxs-lookup"><span data-stu-id="73d40-139">Examples</span></span>

<span data-ttu-id="73d40-140">下面是如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="73d40-140">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="73d40-141">请求</span><span class="sxs-lookup"><span data-stu-id="73d40-141">Request</span></span>

<span data-ttu-id="73d40-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="73d40-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="73d40-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="73d40-143">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="73d40-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73d40-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73d40-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73d40-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="73d40-146">C#</span><span class="sxs-lookup"><span data-stu-id="73d40-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73d40-147">Java</span><span class="sxs-lookup"><span data-stu-id="73d40-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffrequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="73d40-148">响应</span><span class="sxs-lookup"><span data-stu-id="73d40-148">Response</span></span>

<span data-ttu-id="73d40-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="73d40-149">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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


