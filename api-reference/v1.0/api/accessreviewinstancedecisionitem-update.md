---
title: 更新 accessReviewInstanceDecisionItem
description: 更新 accessReviewInstanceDecisionItem 对象的属性。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ca2f5c24f10bd287b73502ec3d8ba5b6c399da18
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209613"
---
# <a name="update-accessreviewinstancedecisionitem"></a><span data-ttu-id="d8941-103">更新 accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="d8941-103">Update accessReviewInstanceDecisionItem</span></span>
<span data-ttu-id="d8941-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8941-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d8941-105">更新 [accessReviewInstanceDecisionItem 对象](../resources/accessreviewinstancedecisionitem.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="d8941-105">Update the properties of an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="d8941-106">权限</span><span class="sxs-lookup"><span data-stu-id="d8941-106">Permissions</span></span>
<span data-ttu-id="d8941-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8941-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8941-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8941-109">Permission type</span></span>|<span data-ttu-id="d8941-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d8941-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8941-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8941-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d8941-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8941-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="d8941-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8941-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8941-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8941-114">Not supported.</span></span>|
|<span data-ttu-id="d8941-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8941-115">Application</span></span>|<span data-ttu-id="d8941-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8941-116">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="d8941-117">只有列为父 [accessReviewInstance](../resources/accessreviewinstance.md) 审阅者的调用用户才能更新 **accessReviewInstanceDecisionItem**。</span><span class="sxs-lookup"><span data-stu-id="d8941-117">Only a calling user who is listed as reviewer for the parent [accessReviewInstance](../resources/accessreviewinstance.md) can update the **accessReviewInstanceDecisionItem**.</span></span>

## <a name="http-request"></a><span data-ttu-id="d8941-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8941-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="d8941-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8941-119">Request headers</span></span>
|<span data-ttu-id="d8941-120">名称</span><span class="sxs-lookup"><span data-stu-id="d8941-120">Name</span></span>|<span data-ttu-id="d8941-121">说明</span><span class="sxs-lookup"><span data-stu-id="d8941-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d8941-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8941-122">Authorization</span></span>|<span data-ttu-id="d8941-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d8941-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d8941-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8941-125">Content-Type</span></span>|<span data-ttu-id="d8941-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d8941-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8941-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8941-128">Request body</span></span>
<span data-ttu-id="d8941-129">在请求正文中，提供 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8941-129">In the request body, supply a JSON representation of the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object.</span></span>

<span data-ttu-id="d8941-130">下表显示更新 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)时接受的属性。</span><span class="sxs-lookup"><span data-stu-id="d8941-130">The following table shows the properties that are accepted when you update the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).</span></span>

|<span data-ttu-id="d8941-131">属性</span><span class="sxs-lookup"><span data-stu-id="d8941-131">Property</span></span>|<span data-ttu-id="d8941-132">类型</span><span class="sxs-lookup"><span data-stu-id="d8941-132">Type</span></span>|<span data-ttu-id="d8941-133">说明</span><span class="sxs-lookup"><span data-stu-id="d8941-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8941-134">decision</span><span class="sxs-lookup"><span data-stu-id="d8941-134">decision</span></span>|<span data-ttu-id="d8941-135">String</span><span class="sxs-lookup"><span data-stu-id="d8941-135">String</span></span>|<span data-ttu-id="d8941-136">审阅者对主体是否应有权访问所审阅的资源的投票。</span><span class="sxs-lookup"><span data-stu-id="d8941-136">The reviewer's vote on whether the principal should have access to the resource under review.</span></span> <span data-ttu-id="d8941-137">可能的值 `Approve` ：、 `Deny` 或 `DontKnow` 。</span><span class="sxs-lookup"><span data-stu-id="d8941-137">Possible values: `Approve`, `Deny`, or `DontKnow`.</span></span> <span data-ttu-id="d8941-138">必填。</span><span class="sxs-lookup"><span data-stu-id="d8941-138">Required.</span></span>|
|<span data-ttu-id="d8941-139">justification</span><span class="sxs-lookup"><span data-stu-id="d8941-139">justification</span></span>|<span data-ttu-id="d8941-140">String</span><span class="sxs-lookup"><span data-stu-id="d8941-140">String</span></span>|<span data-ttu-id="d8941-141">审阅者的决策原因。</span><span class="sxs-lookup"><span data-stu-id="d8941-141">The reviewer's reason for decision.</span></span> <span data-ttu-id="d8941-142">如果 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)的 settings 属性的 **justificationRequiredOnApproval** 为 ，则必需 `true` 。</span><span class="sxs-lookup"><span data-stu-id="d8941-142">Required if the **justificationRequiredOnApproval** of the settings property of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="d8941-143">响应</span><span class="sxs-lookup"><span data-stu-id="d8941-143">Response</span></span>

<span data-ttu-id="d8941-144">如果成功，此方法返回 `204 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d8941-144">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d8941-145">示例</span><span class="sxs-lookup"><span data-stu-id="d8941-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d8941-146">请求</span><span class="sxs-lookup"><span data-stu-id="d8941-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d8941-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8941-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d8941-148">C#</span><span class="sxs-lookup"><span data-stu-id="d8941-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8941-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8941-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8941-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8941-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8941-151">Java</span><span class="sxs-lookup"><span data-stu-id="d8941-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d8941-152">响应</span><span class="sxs-lookup"><span data-stu-id="d8941-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
