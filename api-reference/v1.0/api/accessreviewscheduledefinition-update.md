---
title: 更新 accessReviewScheduleDefinition
description: 更新 accessReviewScheduleDefinition 对象的属性。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0e5569c4d4bee977528883be06003d486e72df72
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031090"
---
# <a name="update-accessreviewscheduledefinition"></a><span data-ttu-id="f121c-103">更新 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="f121c-103">Update accessReviewScheduleDefinition</span></span>
<span data-ttu-id="f121c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f121c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f121c-105">更新 [accessReviewScheduleDefinition 对象](../resources/accessreviewscheduledefinition.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="f121c-105">Update the properties of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="f121c-106">对 accessReviewScheduleDefinition 的任何更新都仅适用于将来的实例。</span><span class="sxs-lookup"><span data-stu-id="f121c-106">Any updates to an accessReviewScheduleDefinition only apply to future instances.</span></span> <span data-ttu-id="f121c-107">当前运行的实例无法更新。</span><span class="sxs-lookup"><span data-stu-id="f121c-107">Currently running instances cannot be updated.</span></span> <span data-ttu-id="f121c-108">此外，此 API 不用于更新 accessReviewInstance 级别的属性（包括决策）。</span><span class="sxs-lookup"><span data-stu-id="f121c-108">Additionally, this API is not intended to update properties, including decisions, on the accessReviewInstance level.</span></span> <span data-ttu-id="f121c-109">有关[实例详细信息，请参阅 accessReviewInstance。](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="f121c-109">See [accessReviewInstance](../resources/accessreviewinstance.md) for more information on instances.</span></span>

## <a name="permissions"></a><span data-ttu-id="f121c-110">权限</span><span class="sxs-lookup"><span data-stu-id="f121c-110">Permissions</span></span>
<span data-ttu-id="f121c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f121c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f121c-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="f121c-113">Permission type</span></span>|<span data-ttu-id="f121c-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f121c-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f121c-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f121c-115">Delegated (work or school account)</span></span>|<span data-ttu-id="f121c-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f121c-116">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="f121c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f121c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f121c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f121c-118">Not supported.</span></span>|
|<span data-ttu-id="f121c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="f121c-119">Application</span></span>|<span data-ttu-id="f121c-120">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f121c-120">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f121c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f121c-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="f121c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f121c-122">Request headers</span></span>
|<span data-ttu-id="f121c-123">名称</span><span class="sxs-lookup"><span data-stu-id="f121c-123">Name</span></span>|<span data-ttu-id="f121c-124">说明</span><span class="sxs-lookup"><span data-stu-id="f121c-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f121c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f121c-125">Authorization</span></span>|<span data-ttu-id="f121c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f121c-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f121c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f121c-128">Content-Type</span></span>|<span data-ttu-id="f121c-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f121c-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f121c-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="f121c-131">Request body</span></span>
<span data-ttu-id="f121c-132">在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f121c-132">In the request body, supply a JSON representation of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="f121c-133">下表显示接受用于更新 accessReviewScheduleDefinition 的属性。</span><span class="sxs-lookup"><span data-stu-id="f121c-133">The following table shows the properties accepted to update an accessReviewScheduleDefinition.</span></span>

| <span data-ttu-id="f121c-134">属性</span><span class="sxs-lookup"><span data-stu-id="f121c-134">Property</span></span> | <span data-ttu-id="f121c-135">类型</span><span class="sxs-lookup"><span data-stu-id="f121c-135">Type</span></span> | <span data-ttu-id="f121c-136">说明</span><span class="sxs-lookup"><span data-stu-id="f121c-136">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f121c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f121c-137">displayName</span></span> | <span data-ttu-id="f121c-138">String</span><span class="sxs-lookup"><span data-stu-id="f121c-138">String</span></span> | <span data-ttu-id="f121c-139">访问评审系列的名称。</span><span class="sxs-lookup"><span data-stu-id="f121c-139">Name of access review series.</span></span> |
| <span data-ttu-id="f121c-140">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="f121c-140">descriptionForAdmins</span></span> | <span data-ttu-id="f121c-141">String</span><span class="sxs-lookup"><span data-stu-id="f121c-141">String</span></span> | <span data-ttu-id="f121c-142">提供给管理员评价的上下文。</span><span class="sxs-lookup"><span data-stu-id="f121c-142">Context of the review provided to admins.</span></span> |
| <span data-ttu-id="f121c-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="f121c-143">descriptionForReviewers</span></span> | <span data-ttu-id="f121c-144">String</span><span class="sxs-lookup"><span data-stu-id="f121c-144">String</span></span> | <span data-ttu-id="f121c-145">提供给审阅者的审阅上下文。</span><span class="sxs-lookup"><span data-stu-id="f121c-145">Context of the review provided to reviewers.</span></span> |
| <span data-ttu-id="f121c-146">settings</span><span class="sxs-lookup"><span data-stu-id="f121c-146">settings</span></span> | [<span data-ttu-id="f121c-147">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="f121c-147">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md) | <span data-ttu-id="f121c-148">访问评审系列的设置。</span><span class="sxs-lookup"><span data-stu-id="f121c-148">The settings for an access review series.</span></span> <span data-ttu-id="f121c-149">请参阅 [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="f121c-149">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="f121c-150">reviewers</span><span class="sxs-lookup"><span data-stu-id="f121c-150">reviewers</span></span> | <span data-ttu-id="f121c-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f121c-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|  <span data-ttu-id="f121c-152">定义审阅者是谁。</span><span class="sxs-lookup"><span data-stu-id="f121c-152">Defines who the reviewers are.</span></span> <span data-ttu-id="f121c-153">如果未指定任何内容，则评论是自 (用户查看自己的访问权限) 。</span><span class="sxs-lookup"><span data-stu-id="f121c-153">If none are specified, the review is a self-review (users review their own access).</span></span> <span data-ttu-id="f121c-154">只有在 **将** 单个用户分配为审阅者时，审阅者属性才可更新。</span><span class="sxs-lookup"><span data-stu-id="f121c-154">The **reviewers** property is only updatable if individual users are assigned as reviewers.</span></span> <span data-ttu-id="f121c-155">请参阅 [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="f121c-155">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> |
|<span data-ttu-id="f121c-156">fallbackReviewers</span><span class="sxs-lookup"><span data-stu-id="f121c-156">fallbackReviewers</span></span>|<span data-ttu-id="f121c-157">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f121c-157">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="f121c-158">用于定义回退审阅者列表的审阅者范围的集合，如果从指定的审阅者列表中找不到用户，将通知这些审阅者采取措施。</span><span class="sxs-lookup"><span data-stu-id="f121c-158">A collection of reviewer scopes used to define the list of fallback reviewers who are notified to take action if no users are found from the list of reviewers specified.</span></span> <span data-ttu-id="f121c-159">当组所有者指定为审阅者，但组所有者不存在时，或者将经理指定为审阅者但用户的经理不存在时，可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="f121c-159">This could occur when either the group owner is specified as the reviewer but the group owner does not exist, or manager is specified as reviewer but a user's manager does not exist.</span></span>|

<span data-ttu-id="f121c-160">**PUT** 请求希望传入完整的对象，其中包括所有可写属性，而不只是要更新的属性。</span><span class="sxs-lookup"><span data-stu-id="f121c-160">A **PUT** request expects the full object to be passed in, which includes all writable properties, not just the properties being updated.</span></span>

## <a name="response"></a><span data-ttu-id="f121c-161">响应</span><span class="sxs-lookup"><span data-stu-id="f121c-161">Response</span></span>
<span data-ttu-id="f121c-162">如果成功，此方法返回 响应 `204 No Content` 代码，无响应正文。</span><span class="sxs-lookup"><span data-stu-id="f121c-162">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f121c-163">示例</span><span class="sxs-lookup"><span data-stu-id="f121c-163">Examples</span></span>
<span data-ttu-id="f121c-164">这是更新现有访问评审系列的 displayName 的示例。</span><span class="sxs-lookup"><span data-stu-id="f121c-164">This is an example of updating the displayName of an existing access review series.</span></span>

### <a name="request"></a><span data-ttu-id="f121c-165">请求</span><span class="sxs-lookup"><span data-stu-id="f121c-165">Request</span></span>
<span data-ttu-id="f121c-166">在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的新属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f121c-166">In the request body, supply a JSON representation of the new properties of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

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


### <a name="response"></a><span data-ttu-id="f121c-167">响应</span><span class="sxs-lookup"><span data-stu-id="f121c-167">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
