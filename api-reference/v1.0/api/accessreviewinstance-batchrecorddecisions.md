---
title: accessReviewInstance：batchRecordDecisions
description: 使审阅者可以分批审阅所有 accessReviewInstanceDecisionItems。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ea22d510bb70ab8d7047f952f7b4c0e265d57197
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031075"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a><span data-ttu-id="fa143-103">accessReviewInstance：batchRecordDecisions</span><span class="sxs-lookup"><span data-stu-id="fa143-103">accessReviewInstance: batchRecordDecisions</span></span>
<span data-ttu-id="fa143-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa143-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fa143-105">允许审阅者使用 **principalId** **、resourceId** 或两者成批查看所有 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fa143-105">Enables reviewers to review all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects in batches by using **principalId**, **resourceId**, or neither.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa143-106">权限</span><span class="sxs-lookup"><span data-stu-id="fa143-106">Permissions</span></span>
<span data-ttu-id="fa143-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa143-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa143-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa143-109">Permission type</span></span>|<span data-ttu-id="fa143-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa143-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa143-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa143-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa143-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa143-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="fa143-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa143-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa143-114">不支持</span><span class="sxs-lookup"><span data-stu-id="fa143-114">Not supported</span></span>|
|<span data-ttu-id="fa143-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa143-115">Application</span></span>|<span data-ttu-id="fa143-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa143-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa143-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa143-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/batchRecordDecisions
```

## <a name="request-headers"></a><span data-ttu-id="fa143-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa143-118">Request headers</span></span>
|<span data-ttu-id="fa143-119">名称</span><span class="sxs-lookup"><span data-stu-id="fa143-119">Name</span></span>|<span data-ttu-id="fa143-120">说明</span><span class="sxs-lookup"><span data-stu-id="fa143-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fa143-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa143-121">Authorization</span></span>|<span data-ttu-id="fa143-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa143-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fa143-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa143-124">Content-Type</span></span>|<span data-ttu-id="fa143-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="fa143-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa143-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa143-127">Request body</span></span>
<span data-ttu-id="fa143-128">在请求正文中，提供 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa143-128">In the request body, supply a JSON representation of an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).</span></span>

<span data-ttu-id="fa143-129">下表列出了可用于查看 [accessReviewInstanceDecisionItem 对象](../resources/accessreviewinstancedecisionitem.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="fa143-129">The following table lists the properties that you can use to review [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects.</span></span>

|<span data-ttu-id="fa143-130">参数</span><span class="sxs-lookup"><span data-stu-id="fa143-130">Parameter</span></span>|<span data-ttu-id="fa143-131">类型</span><span class="sxs-lookup"><span data-stu-id="fa143-131">Type</span></span>|<span data-ttu-id="fa143-132">说明</span><span class="sxs-lookup"><span data-stu-id="fa143-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa143-133">decision</span><span class="sxs-lookup"><span data-stu-id="fa143-133">decision</span></span>|<span data-ttu-id="fa143-134">String</span><span class="sxs-lookup"><span data-stu-id="fa143-134">String</span></span>|<span data-ttu-id="fa143-135">被审阅实体的访问决策。</span><span class="sxs-lookup"><span data-stu-id="fa143-135">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="fa143-136">可取值为：`Approve`、`Deny`、`NotReviewed`、`DontKnow`。</span><span class="sxs-lookup"><span data-stu-id="fa143-136">Possible values are: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span></span> <span data-ttu-id="fa143-137">必填。</span><span class="sxs-lookup"><span data-stu-id="fa143-137">Required.</span></span>|
|<span data-ttu-id="fa143-138">justification</span><span class="sxs-lookup"><span data-stu-id="fa143-138">justification</span></span>|<span data-ttu-id="fa143-139">String</span><span class="sxs-lookup"><span data-stu-id="fa143-139">String</span></span>|<span data-ttu-id="fa143-140">提供给管理员评价的上下文。</span><span class="sxs-lookup"><span data-stu-id="fa143-140">Context of the review provided to admins.</span></span> <span data-ttu-id="fa143-141">如果 **accessReviewScheduleDefinition** 的 settings 属性的 **justificationRequiredOnApproval** 为 ，则必需 `true` 。</span><span class="sxs-lookup"><span data-stu-id="fa143-141">Required if **justificationRequiredOnApproval** of the settings property of the **accessReviewScheduleDefinition** is `true` .</span></span>|
|<span data-ttu-id="fa143-142">principalId</span><span class="sxs-lookup"><span data-stu-id="fa143-142">principalId</span></span>|<span data-ttu-id="fa143-143">String</span><span class="sxs-lookup"><span data-stu-id="fa143-143">String</span></span>|<span data-ttu-id="fa143-144">如果提供，将在此批处理中检查具有匹配 **principalId** 值的所有 **accessReviewInstanceDecisionItems。**</span><span class="sxs-lookup"><span data-stu-id="fa143-144">If supplied, all the **accessReviewInstanceDecisionItems** with matching **principalId** values will be reviewed in this batch.</span></span> <span data-ttu-id="fa143-145">如果未提供，将检查 **所有 accessReviewInstanceDecisionItems。**</span><span class="sxs-lookup"><span data-stu-id="fa143-145">If not supplied, all **accessReviewInstanceDecisionItems** will be reviewed.</span></span>|
|<span data-ttu-id="fa143-146">resourceId</span><span class="sxs-lookup"><span data-stu-id="fa143-146">resourceId</span></span>|<span data-ttu-id="fa143-147">String</span><span class="sxs-lookup"><span data-stu-id="fa143-147">String</span></span>|<span data-ttu-id="fa143-148">如果提供，将在此批处理中检查具有匹配 **resourceId** 的所有 **accessReviewInstanceDecisionItems。**</span><span class="sxs-lookup"><span data-stu-id="fa143-148">If supplied, all the **accessReviewInstanceDecisionItems** with matching **resourceId** will be reviewed in this batch.</span></span> <span data-ttu-id="fa143-149">如果未提供，将检查 **所有 accessReviewInstanceDecisionItems。**</span><span class="sxs-lookup"><span data-stu-id="fa143-149">If not supplied, all **accessReviewInstanceDecisionItems** will be reviewed.</span></span>|

## <a name="response"></a><span data-ttu-id="fa143-150">响应</span><span class="sxs-lookup"><span data-stu-id="fa143-150">Response</span></span>

<span data-ttu-id="fa143-151">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="fa143-151">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="fa143-152">示例</span><span class="sxs-lookup"><span data-stu-id="fa143-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fa143-153">请求</span><span class="sxs-lookup"><span data-stu-id="fa143-153">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_batchrecorddecisions"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-6778-8868-9999c7f4cc06/batchRecordDecisions
Content-type: application/json

{
  "decision": "Approve",
  "justification": "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team",
  "resourceId": "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
}
```

### <a name="response"></a><span data-ttu-id="fa143-154">响应</span><span class="sxs-lookup"><span data-stu-id="fa143-154">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
