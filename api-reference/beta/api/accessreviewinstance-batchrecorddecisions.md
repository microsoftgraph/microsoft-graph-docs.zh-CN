---
title: accessReviewInstance：batchRecordDecisions
description: 可模拟审阅者分批审阅所有 accessReviewInstanceDecisionItems。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e9573dabd24b414b55fc4ec961999c43896fc687
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469727"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a><span data-ttu-id="69f43-103">accessReviewInstance：batchRecordDecisions</span><span class="sxs-lookup"><span data-stu-id="69f43-103">accessReviewInstance: batchRecordDecisions</span></span>
<span data-ttu-id="69f43-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69f43-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69f43-105">允许审阅者使用 、或两者成批查看所有 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) `principalId` `resourceId` 对象。</span><span class="sxs-lookup"><span data-stu-id="69f43-105">Enable reviewers to review all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects in batches by using `principalId`, `resourceId`, or neither.</span></span>

## <a name="permissions"></a><span data-ttu-id="69f43-106">权限</span><span class="sxs-lookup"><span data-stu-id="69f43-106">Permissions</span></span>
<span data-ttu-id="69f43-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69f43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69f43-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="69f43-109">Permission type</span></span>|<span data-ttu-id="69f43-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69f43-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69f43-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69f43-111">Delegated (work or school account)</span></span>|<span data-ttu-id="69f43-112">AccessReviews.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f43-112">AccessReviews.ReadWrite.All</span></span>|
|<span data-ttu-id="69f43-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69f43-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69f43-114">不支持</span><span class="sxs-lookup"><span data-stu-id="69f43-114">Not supported</span></span>|
|<span data-ttu-id="69f43-115">Application</span><span class="sxs-lookup"><span data-stu-id="69f43-115">Application</span></span>|<span data-ttu-id="69f43-116">AccessReviews.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f43-116">AccessReviews.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69f43-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69f43-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
```

## <a name="request-headers"></a><span data-ttu-id="69f43-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="69f43-118">Request headers</span></span>
|<span data-ttu-id="69f43-119">名称</span><span class="sxs-lookup"><span data-stu-id="69f43-119">Name</span></span>|<span data-ttu-id="69f43-120">说明</span><span class="sxs-lookup"><span data-stu-id="69f43-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="69f43-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="69f43-121">Authorization</span></span>|<span data-ttu-id="69f43-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="69f43-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="69f43-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69f43-124">Content-Type</span></span>|<span data-ttu-id="69f43-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="69f43-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69f43-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="69f43-127">Request body</span></span>
<span data-ttu-id="69f43-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69f43-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="69f43-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="69f43-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="69f43-130">参数</span><span class="sxs-lookup"><span data-stu-id="69f43-130">Parameter</span></span>|<span data-ttu-id="69f43-131">类型</span><span class="sxs-lookup"><span data-stu-id="69f43-131">Type</span></span>|<span data-ttu-id="69f43-132">说明</span><span class="sxs-lookup"><span data-stu-id="69f43-132">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="69f43-133">decision</span><span class="sxs-lookup"><span data-stu-id="69f43-133">decision</span></span>  | <span data-ttu-id="69f43-134">String</span><span class="sxs-lookup"><span data-stu-id="69f43-134">String</span></span> | <span data-ttu-id="69f43-135">被审阅实体的访问决策。</span><span class="sxs-lookup"><span data-stu-id="69f43-135">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="69f43-136">可取值为：`Approve`、`Deny`、`NotReviewed`、`DontKnow`。</span><span class="sxs-lookup"><span data-stu-id="69f43-136">Possible values are: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span></span> <span data-ttu-id="69f43-137">必需。</span><span class="sxs-lookup"><span data-stu-id="69f43-137">Required.</span></span>  |
|  <span data-ttu-id="69f43-138">justification</span><span class="sxs-lookup"><span data-stu-id="69f43-138">justification</span></span> | <span data-ttu-id="69f43-139">String</span><span class="sxs-lookup"><span data-stu-id="69f43-139">String</span></span> | <span data-ttu-id="69f43-140">提供给管理员评价的上下文。</span><span class="sxs-lookup"><span data-stu-id="69f43-140">Context of the review provided to admins.</span></span> <span data-ttu-id="69f43-141">如果 **justificationRequiredOnApproval** `True` 位于 **accessReviewScheduleDefinition 上，则是必需的**。</span><span class="sxs-lookup"><span data-stu-id="69f43-141">Required if **justificationRequiredOnApproval** is `True` on the **accessReviewScheduleDefinition**.</span></span>  |
|<span data-ttu-id="69f43-142">principalId</span><span class="sxs-lookup"><span data-stu-id="69f43-142">principalId</span></span>|<span data-ttu-id="69f43-143">String</span><span class="sxs-lookup"><span data-stu-id="69f43-143">String</span></span>|<span data-ttu-id="69f43-144">如果提供，将在此批处理中检查具有匹配 **principalId** 的所有 **accessReviewInstanceDecisionItems。**</span><span class="sxs-lookup"><span data-stu-id="69f43-144">If supplied, all the **accessReviewInstanceDecisionItems** with matching **principalId** will be reviewed in this batch.</span></span> <span data-ttu-id="69f43-145">如果未提供，将 **检查所有 principalId。**</span><span class="sxs-lookup"><span data-stu-id="69f43-145">If not supplied, all **principalIds** will be reviewed.</span></span>|
|<span data-ttu-id="69f43-146">resourceId</span><span class="sxs-lookup"><span data-stu-id="69f43-146">resourceId</span></span>|<span data-ttu-id="69f43-147">String</span><span class="sxs-lookup"><span data-stu-id="69f43-147">String</span></span>|<span data-ttu-id="69f43-148">如果提供，将在此批处理中检查具有匹配 **resourceId** 的所有 **accessReviewInstanceDecisionItems。**</span><span class="sxs-lookup"><span data-stu-id="69f43-148">If supplied, all the **accessReviewInstanceDecisionItems** with matching **resourceId** will be reviewed in this batch.</span></span> <span data-ttu-id="69f43-149">如果未提供，将 **检查所有 resourceId。**</span><span class="sxs-lookup"><span data-stu-id="69f43-149">If not supplied, all **resourceIds** will be reviewed.</span></span>|



## <a name="response"></a><span data-ttu-id="69f43-150">响应</span><span class="sxs-lookup"><span data-stu-id="69f43-150">Response</span></span>

<span data-ttu-id="69f43-151">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="69f43-151">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="69f43-152">示例</span><span class="sxs-lookup"><span data-stu-id="69f43-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="69f43-153">请求</span><span class="sxs-lookup"><span data-stu-id="69f43-153">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_batchrecorddecisions"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
Content-Type: application/json
Content-length: 113

{
  "decision": "Approve",
  "justification": "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team",
  "resourceId": "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
}
```


### <a name="response"></a><span data-ttu-id="69f43-154">响应</span><span class="sxs-lookup"><span data-stu-id="69f43-154">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
