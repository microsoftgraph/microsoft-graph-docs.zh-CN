---
title: accessReviewInstance：batchRecordDecisions
description: 使审阅者可以分批查看所有 accessReviewInstanceDecisionItem 对象。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ab7e7e3580275aa127bbb01e34484a823d4b01bf
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030745"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a><span data-ttu-id="86d37-103">accessReviewInstance：batchRecordDecisions</span><span class="sxs-lookup"><span data-stu-id="86d37-103">accessReviewInstance: batchRecordDecisions</span></span>
<span data-ttu-id="86d37-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86d37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86d37-105">允许审阅者使用 **principalId** **、resourceId** 或两者成批查看所有 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="86d37-105">Enables reviewers to review all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects in batches by using **principalId**, **resourceId**, or neither.</span></span>

## <a name="permissions"></a><span data-ttu-id="86d37-106">权限</span><span class="sxs-lookup"><span data-stu-id="86d37-106">Permissions</span></span>
<span data-ttu-id="86d37-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86d37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86d37-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="86d37-109">Permission type</span></span>|<span data-ttu-id="86d37-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86d37-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86d37-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86d37-111">Delegated (work or school account)</span></span>|<span data-ttu-id="86d37-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86d37-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="86d37-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86d37-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86d37-114">不支持</span><span class="sxs-lookup"><span data-stu-id="86d37-114">Not supported</span></span>|
|<span data-ttu-id="86d37-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="86d37-115">Application</span></span>|<span data-ttu-id="86d37-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86d37-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86d37-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86d37-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
```

## <a name="request-headers"></a><span data-ttu-id="86d37-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="86d37-118">Request headers</span></span>
|<span data-ttu-id="86d37-119">名称</span><span class="sxs-lookup"><span data-stu-id="86d37-119">Name</span></span>|<span data-ttu-id="86d37-120">说明</span><span class="sxs-lookup"><span data-stu-id="86d37-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="86d37-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="86d37-121">Authorization</span></span>|<span data-ttu-id="86d37-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="86d37-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="86d37-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="86d37-124">Content-Type</span></span>|<span data-ttu-id="86d37-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="86d37-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86d37-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="86d37-127">Request body</span></span>
<span data-ttu-id="86d37-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86d37-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="86d37-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="86d37-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="86d37-130">参数</span><span class="sxs-lookup"><span data-stu-id="86d37-130">Parameter</span></span>|<span data-ttu-id="86d37-131">类型</span><span class="sxs-lookup"><span data-stu-id="86d37-131">Type</span></span>|<span data-ttu-id="86d37-132">说明</span><span class="sxs-lookup"><span data-stu-id="86d37-132">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="86d37-133">decision</span><span class="sxs-lookup"><span data-stu-id="86d37-133">decision</span></span>  | <span data-ttu-id="86d37-134">String</span><span class="sxs-lookup"><span data-stu-id="86d37-134">String</span></span> | <span data-ttu-id="86d37-135">被审阅实体的访问决策。</span><span class="sxs-lookup"><span data-stu-id="86d37-135">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="86d37-136">可取值为：`Approve`、`Deny`、`NotReviewed`、`DontKnow`。</span><span class="sxs-lookup"><span data-stu-id="86d37-136">Possible values are: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span></span> <span data-ttu-id="86d37-137">必填。</span><span class="sxs-lookup"><span data-stu-id="86d37-137">Required.</span></span>  |
|  <span data-ttu-id="86d37-138">justification</span><span class="sxs-lookup"><span data-stu-id="86d37-138">justification</span></span> | <span data-ttu-id="86d37-139">String</span><span class="sxs-lookup"><span data-stu-id="86d37-139">String</span></span> | <span data-ttu-id="86d37-140">提供给管理员评价的上下文。</span><span class="sxs-lookup"><span data-stu-id="86d37-140">Context of the review provided to admins.</span></span> <span data-ttu-id="86d37-141">如果 **justificationRequiredOnApproval** `True` 位于 **accessReviewScheduleDefinition 上，则是必需的**。</span><span class="sxs-lookup"><span data-stu-id="86d37-141">Required if **justificationRequiredOnApproval** is `True` on the **accessReviewScheduleDefinition**.</span></span>  |
|<span data-ttu-id="86d37-142">principalId</span><span class="sxs-lookup"><span data-stu-id="86d37-142">principalId</span></span>|<span data-ttu-id="86d37-143">String</span><span class="sxs-lookup"><span data-stu-id="86d37-143">String</span></span>|<span data-ttu-id="86d37-144">如果提供，将在此批处理中检查具有匹配 **principalId** 的所有 **accessReviewInstanceDecisionItems。**</span><span class="sxs-lookup"><span data-stu-id="86d37-144">If supplied, all the **accessReviewInstanceDecisionItems** with matching **principalId** will be reviewed in this batch.</span></span> <span data-ttu-id="86d37-145">如果未提供，将 **检查所有 principalId。**</span><span class="sxs-lookup"><span data-stu-id="86d37-145">If not supplied, all **principalIds** will be reviewed.</span></span>|
|<span data-ttu-id="86d37-146">resourceId</span><span class="sxs-lookup"><span data-stu-id="86d37-146">resourceId</span></span>|<span data-ttu-id="86d37-147">String</span><span class="sxs-lookup"><span data-stu-id="86d37-147">String</span></span>|<span data-ttu-id="86d37-148">如果提供，将在此批处理中检查具有匹配 **resourceId** 的所有 **accessReviewInstanceDecisionItems。**</span><span class="sxs-lookup"><span data-stu-id="86d37-148">If supplied, all the **accessReviewInstanceDecisionItems** with matching **resourceId** will be reviewed in this batch.</span></span> <span data-ttu-id="86d37-149">如果未提供，将 **检查所有 resourceId。**</span><span class="sxs-lookup"><span data-stu-id="86d37-149">If not supplied, all **resourceIds** will be reviewed.</span></span>|



## <a name="response"></a><span data-ttu-id="86d37-150">响应</span><span class="sxs-lookup"><span data-stu-id="86d37-150">Response</span></span>

<span data-ttu-id="86d37-151">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="86d37-151">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="86d37-152">示例</span><span class="sxs-lookup"><span data-stu-id="86d37-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86d37-153">请求</span><span class="sxs-lookup"><span data-stu-id="86d37-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="86d37-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="86d37-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_batchrecorddecisions"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
Content-Type: application/json

{
  "decision": "Approve",
  "justification": "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team",
  "resourceId": "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
}
```
# <a name="c"></a>[<span data-ttu-id="86d37-155">C#</span><span class="sxs-lookup"><span data-stu-id="86d37-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-batchrecorddecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86d37-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86d37-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-batchrecorddecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86d37-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86d37-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-batchrecorddecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86d37-158">Java</span><span class="sxs-lookup"><span data-stu-id="86d37-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-batchrecorddecisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="86d37-159">响应</span><span class="sxs-lookup"><span data-stu-id="86d37-159">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
