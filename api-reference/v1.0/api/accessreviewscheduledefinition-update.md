---
title: 更新 accessReviewScheduleDefinition
description: 更新 accessReviewScheduleDefinition 对象的属性。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6f3c39f6111ad910d2551da7e03cdf6e03597b3d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208385"
---
# <a name="update-accessreviewscheduledefinition"></a><span data-ttu-id="32b71-103">更新 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="32b71-103">Update accessReviewScheduleDefinition</span></span>
<span data-ttu-id="32b71-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32b71-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="32b71-105">更新 [accessReviewScheduleDefinition 对象](../resources/accessreviewscheduledefinition.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="32b71-105">Update the properties of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="32b71-106">对 accessReviewScheduleDefinition 的任何更新都仅适用于将来的实例。</span><span class="sxs-lookup"><span data-stu-id="32b71-106">Any updates to an accessReviewScheduleDefinition only apply to future instances.</span></span> <span data-ttu-id="32b71-107">当前运行的实例无法更新。</span><span class="sxs-lookup"><span data-stu-id="32b71-107">Currently running instances cannot be updated.</span></span> <span data-ttu-id="32b71-108">此外，此 API 不用于更新 accessReviewInstance 级别的属性（包括决策）。</span><span class="sxs-lookup"><span data-stu-id="32b71-108">Additionally, this API is not intended to update properties, including decisions, on the accessReviewInstance level.</span></span> <span data-ttu-id="32b71-109">有关[实例详细信息，请参阅 accessReviewInstance。](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="32b71-109">See [accessReviewInstance](../resources/accessreviewinstance.md) for more information on instances.</span></span>

## <a name="permissions"></a><span data-ttu-id="32b71-110">权限</span><span class="sxs-lookup"><span data-stu-id="32b71-110">Permissions</span></span>
<span data-ttu-id="32b71-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32b71-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32b71-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="32b71-113">Permission type</span></span>|<span data-ttu-id="32b71-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32b71-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32b71-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32b71-115">Delegated (work or school account)</span></span>|<span data-ttu-id="32b71-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32b71-116">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="32b71-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32b71-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32b71-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="32b71-118">Not supported.</span></span>|
|<span data-ttu-id="32b71-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="32b71-119">Application</span></span>|<span data-ttu-id="32b71-120">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32b71-120">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32b71-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32b71-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="32b71-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="32b71-122">Request headers</span></span>
|<span data-ttu-id="32b71-123">名称</span><span class="sxs-lookup"><span data-stu-id="32b71-123">Name</span></span>|<span data-ttu-id="32b71-124">说明</span><span class="sxs-lookup"><span data-stu-id="32b71-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="32b71-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="32b71-125">Authorization</span></span>|<span data-ttu-id="32b71-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="32b71-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="32b71-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32b71-128">Content-Type</span></span>|<span data-ttu-id="32b71-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="32b71-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32b71-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="32b71-131">Request body</span></span>
<span data-ttu-id="32b71-132">在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32b71-132">In the request body, supply a JSON representation of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="32b71-133">下表显示接受用于更新 accessReviewScheduleDefinition 的属性。</span><span class="sxs-lookup"><span data-stu-id="32b71-133">The following table shows the properties accepted to update an accessReviewScheduleDefinition.</span></span>

| <span data-ttu-id="32b71-134">属性</span><span class="sxs-lookup"><span data-stu-id="32b71-134">Property</span></span> | <span data-ttu-id="32b71-135">类型</span><span class="sxs-lookup"><span data-stu-id="32b71-135">Type</span></span> | <span data-ttu-id="32b71-136">说明</span><span class="sxs-lookup"><span data-stu-id="32b71-136">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="32b71-137">displayName</span><span class="sxs-lookup"><span data-stu-id="32b71-137">displayName</span></span> | <span data-ttu-id="32b71-138">String</span><span class="sxs-lookup"><span data-stu-id="32b71-138">String</span></span> | <span data-ttu-id="32b71-139">访问评审系列的名称。</span><span class="sxs-lookup"><span data-stu-id="32b71-139">Name of access review series.</span></span> |
| <span data-ttu-id="32b71-140">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="32b71-140">descriptionForAdmins</span></span> | <span data-ttu-id="32b71-141">String</span><span class="sxs-lookup"><span data-stu-id="32b71-141">String</span></span> | <span data-ttu-id="32b71-142">提供给管理员评价的上下文。</span><span class="sxs-lookup"><span data-stu-id="32b71-142">Context of the review provided to admins.</span></span> |
| <span data-ttu-id="32b71-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="32b71-143">descriptionForReviewers</span></span> | <span data-ttu-id="32b71-144">String</span><span class="sxs-lookup"><span data-stu-id="32b71-144">String</span></span> | <span data-ttu-id="32b71-145">提供给审阅者的审阅上下文。</span><span class="sxs-lookup"><span data-stu-id="32b71-145">Context of the review provided to reviewers.</span></span> |
| <span data-ttu-id="32b71-146">settings</span><span class="sxs-lookup"><span data-stu-id="32b71-146">settings</span></span> | [<span data-ttu-id="32b71-147">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="32b71-147">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md) | <span data-ttu-id="32b71-148">访问评审系列的设置。</span><span class="sxs-lookup"><span data-stu-id="32b71-148">The settings for an access review series.</span></span> <span data-ttu-id="32b71-149">请参阅 [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="32b71-149">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="32b71-150">reviewers</span><span class="sxs-lookup"><span data-stu-id="32b71-150">reviewers</span></span> | <span data-ttu-id="32b71-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="32b71-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|  <span data-ttu-id="32b71-152">定义审阅者是谁。</span><span class="sxs-lookup"><span data-stu-id="32b71-152">Defines who the reviewers are.</span></span> <span data-ttu-id="32b71-153">如果未指定任何内容，则评论是自 (用户查看自己的访问权限) 。</span><span class="sxs-lookup"><span data-stu-id="32b71-153">If none are specified, the review is a self-review (users review their own access).</span></span> <span data-ttu-id="32b71-154">只有在 **将** 单个用户分配为审阅者时，审阅者属性才可更新。</span><span class="sxs-lookup"><span data-stu-id="32b71-154">The **reviewers** property is only updatable if individual users are assigned as reviewers.</span></span> <span data-ttu-id="32b71-155">请参阅 [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="32b71-155">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> |
|<span data-ttu-id="32b71-156">fallbackReviewers</span><span class="sxs-lookup"><span data-stu-id="32b71-156">fallbackReviewers</span></span>|<span data-ttu-id="32b71-157">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="32b71-157">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="32b71-158">用于定义回退审阅者列表的审阅者范围的集合，如果从指定的审阅者列表中找不到用户，将通知这些审阅者采取措施。</span><span class="sxs-lookup"><span data-stu-id="32b71-158">A collection of reviewer scopes used to define the list of fallback reviewers who are notified to take action if no users are found from the list of reviewers specified.</span></span> <span data-ttu-id="32b71-159">当组所有者指定为审阅者，但组所有者不存在时，或者将经理指定为审阅者但用户的经理不存在时，可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="32b71-159">This could occur when either the group owner is specified as the reviewer but the group owner does not exist, or manager is specified as reviewer but a user's manager does not exist.</span></span>|

<span data-ttu-id="32b71-160">**PUT** 请求希望传入完整的对象，其中包括所有可写属性，而不只是要更新的属性。</span><span class="sxs-lookup"><span data-stu-id="32b71-160">A **PUT** request expects the full object to be passed in, which includes all writable properties, not just the properties being updated.</span></span>

## <a name="response"></a><span data-ttu-id="32b71-161">响应</span><span class="sxs-lookup"><span data-stu-id="32b71-161">Response</span></span>
<span data-ttu-id="32b71-162">如果成功，此方法返回 响应 `204 No Content` 代码，无响应正文。</span><span class="sxs-lookup"><span data-stu-id="32b71-162">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="examples"></a><span data-ttu-id="32b71-163">示例</span><span class="sxs-lookup"><span data-stu-id="32b71-163">Examples</span></span>
<span data-ttu-id="32b71-164">这是更新现有访问评审系列的 displayName 的示例。</span><span class="sxs-lookup"><span data-stu-id="32b71-164">This is an example of updating the displayName of an existing access review series.</span></span>

### <a name="request"></a><span data-ttu-id="32b71-165">请求</span><span class="sxs-lookup"><span data-stu-id="32b71-165">Request</span></span>
<span data-ttu-id="32b71-166">在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的新属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32b71-166">In the request body, supply a JSON representation of the new properties of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="32b71-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="32b71-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessreviewscheduledefinition"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6

{
  "id": "60860cdd-fb4d-4054-91ba-f75e04444aa6",
  "displayName": "Test world UPDATED NAME!",
  "descriptionForAdmins": "Test world",
  "descriptionForReviewers": "Test world",
  "scope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "instanceEnumerationScope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 3,
    "autoApplyDecisionsEnabled": false,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-09-15"
      }
    }
  }
}
```
# <a name="c"></a>[<span data-ttu-id="32b71-168">C#</span><span class="sxs-lookup"><span data-stu-id="32b71-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32b71-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32b71-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32b71-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32b71-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32b71-171">Java</span><span class="sxs-lookup"><span data-stu-id="32b71-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="32b71-172">响应</span><span class="sxs-lookup"><span data-stu-id="32b71-172">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
