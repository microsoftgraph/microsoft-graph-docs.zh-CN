---
title: 'accessReviewInstance: applyDecisions'
description: 对 accessReviewInstance 应用决策。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0af1ae1291a95145041a3e92bedf948c766bd1c0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214725"
---
# <a name="accessreviewinstance-applydecisions"></a><span data-ttu-id="b9d12-103">accessReviewInstance: applyDecisions</span><span class="sxs-lookup"><span data-stu-id="b9d12-103">accessReviewInstance: applyDecisions</span></span>

<span data-ttu-id="b9d12-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9d12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9d12-105">在 [accessReviewInstance](../resources/accessreviewinstance.md)上应用评审决策。</span><span class="sxs-lookup"><span data-stu-id="b9d12-105">Apply review decisions on an [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

<span data-ttu-id="b9d12-106">请注意，如果审阅的 [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)中的 autoApplyDecisionsEnabled 参数为 True，则将自动应用决策。</span><span class="sxs-lookup"><span data-stu-id="b9d12-106">Note that decisions will be applied automatically if the autoApplyDecisionsEnabled parameter is True in the review's [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b9d12-107">权限</span><span class="sxs-lookup"><span data-stu-id="b9d12-107">Permissions</span></span>
<span data-ttu-id="b9d12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9d12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9d12-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9d12-110">Permission type</span></span>                        | <span data-ttu-id="b9d12-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9d12-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9d12-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9d12-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9d12-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9d12-113">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="b9d12-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9d12-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9d12-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9d12-115">Not supported.</span></span>|
|<span data-ttu-id="b9d12-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9d12-116">Application</span></span>                            | <span data-ttu-id="b9d12-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9d12-117">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9d12-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9d12-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/applyDecisions
```

## <a name="request-headers"></a><span data-ttu-id="b9d12-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9d12-119">Request headers</span></span>
|<span data-ttu-id="b9d12-120">名称</span><span class="sxs-lookup"><span data-stu-id="b9d12-120">Name</span></span>|<span data-ttu-id="b9d12-121">说明</span><span class="sxs-lookup"><span data-stu-id="b9d12-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b9d12-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9d12-122">Authorization</span></span>|<span data-ttu-id="b9d12-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9d12-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b9d12-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9d12-125">Content-Type</span></span>|<span data-ttu-id="b9d12-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b9d12-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9d12-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9d12-128">Request body</span></span>
<span data-ttu-id="b9d12-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b9d12-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9d12-130">响应</span><span class="sxs-lookup"><span data-stu-id="b9d12-130">Response</span></span>
<span data-ttu-id="b9d12-131">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b9d12-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b9d12-132">示例</span><span class="sxs-lookup"><span data-stu-id="b9d12-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b9d12-133">请求</span><span class="sxs-lookup"><span data-stu-id="b9d12-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b9d12-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9d12-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_applydecisions"
}
-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/04e5c3b2-9db2-40d3-a204-128f4956ae8e/instances/70463350-742e-4909-bfa5-bc23447bd002/applyDecisions
```
# <a name="c"></a>[<span data-ttu-id="b9d12-135">C#</span><span class="sxs-lookup"><span data-stu-id="b9d12-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-applydecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9d12-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9d12-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-applydecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9d12-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9d12-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-applydecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9d12-138">Java</span><span class="sxs-lookup"><span data-stu-id="b9d12-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-applydecisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="b9d12-139">响应</span><span class="sxs-lookup"><span data-stu-id="b9d12-139">Response</span></span>
<span data-ttu-id="b9d12-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b9d12-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
