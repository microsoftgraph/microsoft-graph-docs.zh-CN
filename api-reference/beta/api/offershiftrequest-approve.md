---
title: offerShiftRequest：批准
description: 批准 offershiftrequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 323e18df4287b29531448ba168cbfc94c645fd06
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981306"
---
# <a name="offershiftrequest-approve"></a><span data-ttu-id="781eb-103">offerShiftRequest：批准</span><span class="sxs-lookup"><span data-stu-id="781eb-103">offerShiftRequest: approve</span></span>

<span data-ttu-id="781eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="781eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="781eb-105">批准 [offershiftrequest](../resources/offershiftrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="781eb-105">Approve an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="781eb-106">权限</span><span class="sxs-lookup"><span data-stu-id="781eb-106">Permissions</span></span>

<span data-ttu-id="781eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="781eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="781eb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="781eb-109">Permission type</span></span>                        | <span data-ttu-id="781eb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="781eb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="781eb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="781eb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="781eb-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="781eb-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="781eb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="781eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="781eb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="781eb-114">Not supported.</span></span> |
| <span data-ttu-id="781eb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="781eb-115">Application</span></span>                            | <span data-ttu-id="781eb-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="781eb-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="781eb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="781eb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="781eb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="781eb-118">Request headers</span></span>

| <span data-ttu-id="781eb-119">名称</span><span class="sxs-lookup"><span data-stu-id="781eb-119">Name</span></span>          | <span data-ttu-id="781eb-120">说明</span><span class="sxs-lookup"><span data-stu-id="781eb-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="781eb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="781eb-121">Authorization</span></span> | <span data-ttu-id="781eb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="781eb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="781eb-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="781eb-124">Content-type</span></span> | <span data-ttu-id="781eb-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="781eb-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="781eb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="781eb-127">Request body</span></span>

<span data-ttu-id="781eb-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="781eb-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="781eb-129">参数</span><span class="sxs-lookup"><span data-stu-id="781eb-129">Parameter</span></span>    | <span data-ttu-id="781eb-130">类型</span><span class="sxs-lookup"><span data-stu-id="781eb-130">Type</span></span>        | <span data-ttu-id="781eb-131">描述</span><span class="sxs-lookup"><span data-stu-id="781eb-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="781eb-132">message</span><span class="sxs-lookup"><span data-stu-id="781eb-132">message</span></span>|<span data-ttu-id="781eb-133">String</span><span class="sxs-lookup"><span data-stu-id="781eb-133">String</span></span>|<span data-ttu-id="781eb-134">在审批时发送的自定义邮件。</span><span class="sxs-lookup"><span data-stu-id="781eb-134">Custom message sent on approval.</span></span>|

## <a name="response"></a><span data-ttu-id="781eb-135">响应</span><span class="sxs-lookup"><span data-stu-id="781eb-135">Response</span></span>

<span data-ttu-id="781eb-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="781eb-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="781eb-138">示例</span><span class="sxs-lookup"><span data-stu-id="781eb-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="781eb-139">请求</span><span class="sxs-lookup"><span data-stu-id="781eb-139">Request</span></span>

<span data-ttu-id="781eb-140">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="781eb-140">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="781eb-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="781eb-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve
Content-type: application/json

{
  "message": "Approved!"
}
```
# <a name="javascript"></a>[<span data-ttu-id="781eb-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="781eb-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="781eb-143">C#</span><span class="sxs-lookup"><span data-stu-id="781eb-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/offershiftrequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="781eb-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="781eb-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/offershiftrequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="781eb-145">Java</span><span class="sxs-lookup"><span data-stu-id="781eb-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/offershiftrequest-approve-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="781eb-146">响应</span><span class="sxs-lookup"><span data-stu-id="781eb-146">Response</span></span>

<span data-ttu-id="781eb-147">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="781eb-147">The following example shows the response.</span></span>
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
  "description": "offerShiftRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


