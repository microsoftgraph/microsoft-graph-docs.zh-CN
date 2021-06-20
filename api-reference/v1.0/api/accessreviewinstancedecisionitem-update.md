---
title: 更新 accessReviewInstanceDecisionItem
description: 更新 accessReviewInstanceDecisionItem 对象的属性。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 54b66ade8eb217ce740d3d721fc7433c9d86f505
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031059"
---
# <a name="update-accessreviewinstancedecisionitem"></a><span data-ttu-id="b6e50-103">更新 accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="b6e50-103">Update accessReviewInstanceDecisionItem</span></span>
<span data-ttu-id="b6e50-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6e50-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6e50-105">更新 [accessReviewInstanceDecisionItem 对象](../resources/accessreviewinstancedecisionitem.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="b6e50-105">Update the properties of an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="b6e50-106">权限</span><span class="sxs-lookup"><span data-stu-id="b6e50-106">Permissions</span></span>
<span data-ttu-id="b6e50-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b6e50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6e50-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6e50-109">Permission type</span></span>|<span data-ttu-id="b6e50-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b6e50-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6e50-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6e50-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b6e50-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6e50-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="b6e50-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6e50-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6e50-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6e50-114">Not supported.</span></span>|
|<span data-ttu-id="b6e50-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6e50-115">Application</span></span>|<span data-ttu-id="b6e50-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6e50-116">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="b6e50-117">只有列为父 [accessReviewInstance](../resources/accessreviewinstance.md) 审阅者的调用用户才能更新 **accessReviewInstanceDecisionItem**。</span><span class="sxs-lookup"><span data-stu-id="b6e50-117">Only a calling user who is listed as reviewer for the parent [accessReviewInstance](../resources/accessreviewinstance.md) can update the **accessReviewInstanceDecisionItem**.</span></span>

## <a name="http-request"></a><span data-ttu-id="b6e50-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6e50-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="b6e50-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6e50-119">Request headers</span></span>
|<span data-ttu-id="b6e50-120">名称</span><span class="sxs-lookup"><span data-stu-id="b6e50-120">Name</span></span>|<span data-ttu-id="b6e50-121">说明</span><span class="sxs-lookup"><span data-stu-id="b6e50-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b6e50-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6e50-122">Authorization</span></span>|<span data-ttu-id="b6e50-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b6e50-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b6e50-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b6e50-125">Content-Type</span></span>|<span data-ttu-id="b6e50-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b6e50-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6e50-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6e50-128">Request body</span></span>
<span data-ttu-id="b6e50-129">在请求正文中，提供 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6e50-129">In the request body, supply a JSON representation of the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object.</span></span>

<span data-ttu-id="b6e50-130">下表显示更新 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)时接受的属性。</span><span class="sxs-lookup"><span data-stu-id="b6e50-130">The following table shows the properties that are accepted when you update the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).</span></span>

|<span data-ttu-id="b6e50-131">属性</span><span class="sxs-lookup"><span data-stu-id="b6e50-131">Property</span></span>|<span data-ttu-id="b6e50-132">类型</span><span class="sxs-lookup"><span data-stu-id="b6e50-132">Type</span></span>|<span data-ttu-id="b6e50-133">说明</span><span class="sxs-lookup"><span data-stu-id="b6e50-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6e50-134">decision</span><span class="sxs-lookup"><span data-stu-id="b6e50-134">decision</span></span>|<span data-ttu-id="b6e50-135">String</span><span class="sxs-lookup"><span data-stu-id="b6e50-135">String</span></span>|<span data-ttu-id="b6e50-136">审阅者对主体是否应有权访问所审阅的资源的投票。</span><span class="sxs-lookup"><span data-stu-id="b6e50-136">The reviewer's vote on whether the principal should have access to the resource under review.</span></span> <span data-ttu-id="b6e50-137">可能的值 `Approve` ：、 `Deny` 或 `DontKnow` 。</span><span class="sxs-lookup"><span data-stu-id="b6e50-137">Possible values: `Approve`, `Deny`, or `DontKnow`.</span></span> <span data-ttu-id="b6e50-138">必填。</span><span class="sxs-lookup"><span data-stu-id="b6e50-138">Required.</span></span>|
|<span data-ttu-id="b6e50-139">justification</span><span class="sxs-lookup"><span data-stu-id="b6e50-139">justification</span></span>|<span data-ttu-id="b6e50-140">String</span><span class="sxs-lookup"><span data-stu-id="b6e50-140">String</span></span>|<span data-ttu-id="b6e50-141">审阅者的决策原因。</span><span class="sxs-lookup"><span data-stu-id="b6e50-141">The reviewer's reason for decision.</span></span> <span data-ttu-id="b6e50-142">如果 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)的 settings 属性的 **justificationRequiredOnApproval** 为 ，则必需 `true` 。</span><span class="sxs-lookup"><span data-stu-id="b6e50-142">Required if the **justificationRequiredOnApproval** of the settings property of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="b6e50-143">响应</span><span class="sxs-lookup"><span data-stu-id="b6e50-143">Response</span></span>

<span data-ttu-id="b6e50-144">如果成功，此方法返回 `204 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b6e50-144">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b6e50-145">示例</span><span class="sxs-lookup"><span data-stu-id="b6e50-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b6e50-146">请求</span><span class="sxs-lookup"><span data-stu-id="b6e50-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_accessreviewinstancedecisionitem"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/instances/4444f3b6-8ea4-4dea-90a5-9eac8fe95678/decisions/5555f3b6-8ea4-4dea-90a5-9eac8fe95555
Content-Type: application/json
Content-length: 691

{
  "decision": "Approve",
  "justification": "Kathleen still needs access to the Marketing group as she works in the Marketing organization."
}
```


### <a name="response"></a><span data-ttu-id="b6e50-147">响应</span><span class="sxs-lookup"><span data-stu-id="b6e50-147">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
