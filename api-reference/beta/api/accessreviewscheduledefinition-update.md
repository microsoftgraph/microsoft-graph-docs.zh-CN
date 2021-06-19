---
title: 更新 accessReviewScheduleDefinition
description: 更新现有 accessReviewScheduleDefinition 对象以更改其一个或多个属性。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: be3b7603419d616ef9ea9e4da94fdb8942dc36f3
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030444"
---
# <a name="update-accessreviewscheduledefinition"></a><span data-ttu-id="32c5b-103">更新 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="32c5b-103">Update accessReviewScheduleDefinition</span></span>

<span data-ttu-id="32c5b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32c5b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32c5b-105">更新现有 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象以更改其一个或多个属性。</span><span class="sxs-lookup"><span data-stu-id="32c5b-105">Update an existing [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object to change one or more of its properties.</span></span>

>[!NOTE]
><span data-ttu-id="32c5b-106">对 accessReviewScheduleDefinition 进行的任何更新都仅适用于将来实例。</span><span class="sxs-lookup"><span data-stu-id="32c5b-106">Any updates made to an accessReviewScheduleDefinition only apply to future instances.</span></span> <span data-ttu-id="32c5b-107">当前运行的实例无法更新。</span><span class="sxs-lookup"><span data-stu-id="32c5b-107">Currently running instances cannot be updated.</span></span>
><span data-ttu-id="32c5b-108">此外，此 API 不用于更新 accessReviewInstance 级别的属性（包括决策）。</span><span class="sxs-lookup"><span data-stu-id="32c5b-108">Additionally, this API is not intended to update properties, including decisions, on the accessReviewInstance level.</span></span> <span data-ttu-id="32c5b-109">有关[实例详细信息，请参阅 accessReviewInstance。](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="32c5b-109">See [accessReviewInstance](../resources/accessreviewinstance.md) for more information on instances.</span></span>

## <a name="permissions"></a><span data-ttu-id="32c5b-110">权限</span><span class="sxs-lookup"><span data-stu-id="32c5b-110">Permissions</span></span>
<span data-ttu-id="32c5b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32c5b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32c5b-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="32c5b-113">Permission type</span></span>                        | <span data-ttu-id="32c5b-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32c5b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="32c5b-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32c5b-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="32c5b-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32c5b-116">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="32c5b-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32c5b-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32c5b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="32c5b-118">Not supported.</span></span>|
|<span data-ttu-id="32c5b-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="32c5b-119">Application</span></span>                            | <span data-ttu-id="32c5b-120">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32c5b-120">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="32c5b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32c5b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="32c5b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="32c5b-122">Request headers</span></span>
| <span data-ttu-id="32c5b-123">名称</span><span class="sxs-lookup"><span data-stu-id="32c5b-123">Name</span></span>         | <span data-ttu-id="32c5b-124">说明</span><span class="sxs-lookup"><span data-stu-id="32c5b-124">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="32c5b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="32c5b-125">Authorization</span></span>|<span data-ttu-id="32c5b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="32c5b-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="32c5b-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="32c5b-128">Content-type</span></span> | <span data-ttu-id="32c5b-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="32c5b-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32c5b-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="32c5b-131">Request body</span></span>
<span data-ttu-id="32c5b-132">在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32c5b-132">In the request body, supply a JSON representation of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="32c5b-133">下表显示接受用于更新 accessReviewScheduleDefinition 的属性。</span><span class="sxs-lookup"><span data-stu-id="32c5b-133">The following table shows the properties accepted to update an accessReviewScheduleDefinition.</span></span>

| <span data-ttu-id="32c5b-134">属性</span><span class="sxs-lookup"><span data-stu-id="32c5b-134">Property</span></span> | <span data-ttu-id="32c5b-135">类型</span><span class="sxs-lookup"><span data-stu-id="32c5b-135">Type</span></span> | <span data-ttu-id="32c5b-136">说明</span><span class="sxs-lookup"><span data-stu-id="32c5b-136">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="32c5b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="32c5b-137">displayName</span></span> | <span data-ttu-id="32c5b-138">String</span><span class="sxs-lookup"><span data-stu-id="32c5b-138">String</span></span> | <span data-ttu-id="32c5b-139">访问评审系列的名称。</span><span class="sxs-lookup"><span data-stu-id="32c5b-139">Name of access review series.</span></span> |
| <span data-ttu-id="32c5b-140">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="32c5b-140">descriptionForAdmins</span></span> | <span data-ttu-id="32c5b-141">String</span><span class="sxs-lookup"><span data-stu-id="32c5b-141">String</span></span> | <span data-ttu-id="32c5b-142">提供给管理员评价的上下文。</span><span class="sxs-lookup"><span data-stu-id="32c5b-142">Context of the review provided to admins.</span></span> |
| <span data-ttu-id="32c5b-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="32c5b-143">descriptionForReviewers</span></span> | <span data-ttu-id="32c5b-144">String</span><span class="sxs-lookup"><span data-stu-id="32c5b-144">String</span></span> | <span data-ttu-id="32c5b-145">提供给审阅者的审阅上下文。</span><span class="sxs-lookup"><span data-stu-id="32c5b-145">Context of the review provided to reviewers.</span></span> |
| <span data-ttu-id="32c5b-146">settings</span><span class="sxs-lookup"><span data-stu-id="32c5b-146">settings</span></span> | [<span data-ttu-id="32c5b-147">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="32c5b-147">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md) | <span data-ttu-id="32c5b-148">访问评审系列的设置。</span><span class="sxs-lookup"><span data-stu-id="32c5b-148">The settings for an access review series.</span></span> <span data-ttu-id="32c5b-149">请参阅 [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="32c5b-149">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="32c5b-150">reviewers</span><span class="sxs-lookup"><span data-stu-id="32c5b-150">reviewers</span></span> | <span data-ttu-id="32c5b-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="32c5b-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|  <span data-ttu-id="32c5b-152">定义审阅者是谁。</span><span class="sxs-lookup"><span data-stu-id="32c5b-152">Defines who the reviewers are.</span></span> <span data-ttu-id="32c5b-153">如果未指定任何内容，则评论是自 (用户查看自己的访问权限) 。</span><span class="sxs-lookup"><span data-stu-id="32c5b-153">If none are specified, the review is a self-review (users review their own access).</span></span> <span data-ttu-id="32c5b-154">只有在 **将** 单个用户分配为审阅者时，审阅者属性才可更新。</span><span class="sxs-lookup"><span data-stu-id="32c5b-154">The **reviewers** property is only updatable if individual users are assigned as reviewers.</span></span> <span data-ttu-id="32c5b-155">请参阅 [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="32c5b-155">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> |
|<span data-ttu-id="32c5b-156">fallbackReviewers</span><span class="sxs-lookup"><span data-stu-id="32c5b-156">fallbackReviewers</span></span>|<span data-ttu-id="32c5b-157">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="32c5b-157">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="32c5b-158">用于定义回退审阅者列表的审阅者范围的集合，如果从指定的审阅者列表中找不到用户，将通知这些审阅者采取措施。</span><span class="sxs-lookup"><span data-stu-id="32c5b-158">A collection of reviewer scopes used to define the list of fallback reviewers who are notified to take action if no users are found from the list of reviewers specified.</span></span> <span data-ttu-id="32c5b-159">当组所有者指定为审阅者，但组所有者不存在时，或者将经理指定为审阅者但用户的经理不存在时，可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="32c5b-159">This could occur when either the group owner is specified as the reviewer but the group owner does not exist, or manager is specified as reviewer but a user's manager does not exist.</span></span>|
| <span data-ttu-id="32c5b-160">backupReviewers (弃用) </span><span class="sxs-lookup"><span data-stu-id="32c5b-160">backupReviewers (deprecated)</span></span>|<span data-ttu-id="32c5b-161">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="32c5b-161">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>| <span data-ttu-id="32c5b-162">此属性已被 **fallbackReviewers 取代**。</span><span class="sxs-lookup"><span data-stu-id="32c5b-162">This property has been replaced by **fallbackReviewers**.</span></span> <span data-ttu-id="32c5b-163">但是，指定 **backupReviewers** 或 **fallbackReviewers** 会自动向另一个属性填充相同的值。</span><span class="sxs-lookup"><span data-stu-id="32c5b-163">However, specifying either **backupReviewers** or **fallbackReviewers** automatically populates the same values to the other property.</span></span> |

<span data-ttu-id="32c5b-164">**PUT** 请求希望传入完整的对象，其中包括所有可写属性，而不只是要更新的属性。</span><span class="sxs-lookup"><span data-stu-id="32c5b-164">A **PUT** request expects the full object to be passed in, which includes all writable properties, not just the properties being updated.</span></span>

## <a name="response"></a><span data-ttu-id="32c5b-165">响应</span><span class="sxs-lookup"><span data-stu-id="32c5b-165">Response</span></span>
<span data-ttu-id="32c5b-166">如果成功，此方法返回 响应 `204 No Content` 代码，无响应正文。</span><span class="sxs-lookup"><span data-stu-id="32c5b-166">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="examples"></a><span data-ttu-id="32c5b-167">示例</span><span class="sxs-lookup"><span data-stu-id="32c5b-167">Examples</span></span>

<span data-ttu-id="32c5b-168">这是更新现有访问评审系列的 displayName 的示例。</span><span class="sxs-lookup"><span data-stu-id="32c5b-168">This is an example of updating the displayName of an existing access review series.</span></span>

### <a name="request"></a><span data-ttu-id="32c5b-169">请求</span><span class="sxs-lookup"><span data-stu-id="32c5b-169">Request</span></span>
<span data-ttu-id="32c5b-170">在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的新属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32c5b-170">In the request body, supply a JSON representation of the new properties of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>



# <a name="http"></a>[<span data-ttu-id="32c5b-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="32c5b-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewScheduleDefinition"
}-->
```http
PUT https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6

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
# <a name="javascript"></a>[<span data-ttu-id="32c5b-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32c5b-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32c5b-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32c5b-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="32c5b-174">C#</span><span class="sxs-lookup"><span data-stu-id="32c5b-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32c5b-175">Java</span><span class="sxs-lookup"><span data-stu-id="32c5b-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="32c5b-176">响应</span><span class="sxs-lookup"><span data-stu-id="32c5b-176">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
