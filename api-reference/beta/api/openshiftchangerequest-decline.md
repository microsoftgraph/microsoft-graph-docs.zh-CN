---
title: openShiftChangeRequest： decline
description: 拒绝开放临时请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 64a54cba75b1f71e4bce43ca8bced4e2bb5841e8
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785940"
---
# <a name="openshiftchangerequest-decline"></a><span data-ttu-id="80c75-103">openShiftChangeRequest： decline</span><span class="sxs-lookup"><span data-stu-id="80c75-103">openShiftChangeRequest: decline</span></span>

<span data-ttu-id="80c75-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80c75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80c75-105">拒绝 [openshiftchangerequest](../resources/openshiftchangerequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80c75-105">Decline an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="80c75-106">权限</span><span class="sxs-lookup"><span data-stu-id="80c75-106">Permissions</span></span>

<span data-ttu-id="80c75-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80c75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="80c75-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="80c75-109">Permission type</span></span>                        | <span data-ttu-id="80c75-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80c75-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="80c75-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80c75-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="80c75-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80c75-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="80c75-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80c75-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80c75-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="80c75-114">Not supported.</span></span> |
| <span data-ttu-id="80c75-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="80c75-115">Application</span></span>                            | <span data-ttu-id="80c75-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="80c75-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="80c75-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80c75-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="80c75-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="80c75-118">Request headers</span></span>

| <span data-ttu-id="80c75-119">名称</span><span class="sxs-lookup"><span data-stu-id="80c75-119">Name</span></span>          | <span data-ttu-id="80c75-120">说明</span><span class="sxs-lookup"><span data-stu-id="80c75-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="80c75-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="80c75-121">Authorization</span></span> | <span data-ttu-id="80c75-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80c75-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80c75-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="80c75-124">Request body</span></span>

<span data-ttu-id="80c75-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="80c75-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="80c75-126">参数</span><span class="sxs-lookup"><span data-stu-id="80c75-126">Parameter</span></span>    | <span data-ttu-id="80c75-127">类型</span><span class="sxs-lookup"><span data-stu-id="80c75-127">Type</span></span>        | <span data-ttu-id="80c75-128">描述</span><span class="sxs-lookup"><span data-stu-id="80c75-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="80c75-129">message</span><span class="sxs-lookup"><span data-stu-id="80c75-129">message</span></span>|<span data-ttu-id="80c75-130">String</span><span class="sxs-lookup"><span data-stu-id="80c75-130">String</span></span>|<span data-ttu-id="80c75-131">自定义拒绝邮件。</span><span class="sxs-lookup"><span data-stu-id="80c75-131">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="80c75-132">响应</span><span class="sxs-lookup"><span data-stu-id="80c75-132">Response</span></span>

<span data-ttu-id="80c75-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="80c75-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="80c75-135">示例</span><span class="sxs-lookup"><span data-stu-id="80c75-135">Examples</span></span>

<span data-ttu-id="80c75-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="80c75-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="80c75-137">请求</span><span class="sxs-lookup"><span data-stu-id="80c75-137">Request</span></span>

<span data-ttu-id="80c75-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="80c75-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="80c75-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="80c75-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="80c75-140">C#</span><span class="sxs-lookup"><span data-stu-id="80c75-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/openshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80c75-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80c75-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/openshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80c75-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80c75-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/openshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80c75-143">Java</span><span class="sxs-lookup"><span data-stu-id="80c75-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/openshiftchangerequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="80c75-144">响应</span><span class="sxs-lookup"><span data-stu-id="80c75-144">Response</span></span>

<span data-ttu-id="80c75-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="80c75-145">The following is an example of the response.</span></span>
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
  "description": "openShiftChangeRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


