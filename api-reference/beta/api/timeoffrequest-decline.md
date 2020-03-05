---
title: timeOffRequest：拒绝
description: 拒绝 timeoffrequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9b99949d8ae30d208e1d1939c6473c8767d6cbd6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452258"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="e2a5d-103">timeOffRequest：拒绝</span><span class="sxs-lookup"><span data-stu-id="e2a5d-103">timeOffRequest: decline</span></span>

<span data-ttu-id="e2a5d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e2a5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2a5d-105">拒绝[timeoffrequest](../resources/timeoffrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e2a5d-105">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2a5d-106">权限</span><span class="sxs-lookup"><span data-stu-id="e2a5d-106">Permissions</span></span>

<span data-ttu-id="e2a5d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2a5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e2a5d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2a5d-109">Permission type</span></span>                        | <span data-ttu-id="e2a5d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2a5d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e2a5d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2a5d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e2a5d-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2a5d-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="e2a5d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2a5d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2a5d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2a5d-114">Not supported.</span></span> |
|<span data-ttu-id="e2a5d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2a5d-115">Application</span></span> | <span data-ttu-id="e2a5d-116">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="e2a5d-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="e2a5d-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="e2a5d-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="e2a5d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2a5d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/timeOffRequests/decline
```

## <a name="request-headers"></a><span data-ttu-id="e2a5d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2a5d-119">Request headers</span></span>

| <span data-ttu-id="e2a5d-120">名称</span><span class="sxs-lookup"><span data-stu-id="e2a5d-120">Name</span></span>          | <span data-ttu-id="e2a5d-121">说明</span><span class="sxs-lookup"><span data-stu-id="e2a5d-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e2a5d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2a5d-122">Authorization</span></span> | <span data-ttu-id="e2a5d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2a5d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e2a5d-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="e2a5d-125">Content-type</span></span> | <span data-ttu-id="e2a5d-126">application-json。</span><span class="sxs-lookup"><span data-stu-id="e2a5d-126">application-json.</span></span> <span data-ttu-id="e2a5d-127">必填。</span><span class="sxs-lookup"><span data-stu-id="e2a5d-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2a5d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2a5d-128">Request body</span></span>

<span data-ttu-id="e2a5d-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e2a5d-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e2a5d-130">参数</span><span class="sxs-lookup"><span data-stu-id="e2a5d-130">Parameter</span></span>    | <span data-ttu-id="e2a5d-131">类型</span><span class="sxs-lookup"><span data-stu-id="e2a5d-131">Type</span></span>        | <span data-ttu-id="e2a5d-132">描述</span><span class="sxs-lookup"><span data-stu-id="e2a5d-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e2a5d-133">message</span><span class="sxs-lookup"><span data-stu-id="e2a5d-133">message</span></span>|<span data-ttu-id="e2a5d-134">String</span><span class="sxs-lookup"><span data-stu-id="e2a5d-134">String</span></span>|<span data-ttu-id="e2a5d-135">自定义拒绝邮件。</span><span class="sxs-lookup"><span data-stu-id="e2a5d-135">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="e2a5d-136">响应</span><span class="sxs-lookup"><span data-stu-id="e2a5d-136">Response</span></span>

<span data-ttu-id="e2a5d-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e2a5d-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e2a5d-139">示例</span><span class="sxs-lookup"><span data-stu-id="e2a5d-139">Examples</span></span>

<span data-ttu-id="e2a5d-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e2a5d-140">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="e2a5d-141">请求</span><span class="sxs-lookup"><span data-stu-id="e2a5d-141">Request</span></span>

<span data-ttu-id="e2a5d-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e2a5d-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e2a5d-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2a5d-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="javascript"></a>[<span data-ttu-id="e2a5d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2a5d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2a5d-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2a5d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e2a5d-146">响应</span><span class="sxs-lookup"><span data-stu-id="e2a5d-146">Response</span></span>

<span data-ttu-id="e2a5d-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e2a5d-147">The following is an example of the response.</span></span>
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
