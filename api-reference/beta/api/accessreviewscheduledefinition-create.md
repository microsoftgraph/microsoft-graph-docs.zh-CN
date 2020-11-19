---
title: 创建 accessReviewScheduleDefinition
description: 创建新的 accessReviewScheduleDefinition 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1dc30208652af0989ab0b6bf0b35ebfdd50bc65d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221827"
---
# <a name="create-accessreviewscheduledefinition"></a><span data-ttu-id="83d91-103">创建 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="83d91-103">Create accessReviewScheduleDefinition</span></span>

<span data-ttu-id="83d91-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83d91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83d91-105">创建新的 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="83d91-105">Create a new [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="83d91-106">权限</span><span class="sxs-lookup"><span data-stu-id="83d91-106">Permissions</span></span>

<span data-ttu-id="83d91-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83d91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83d91-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="83d91-109">Permission type</span></span>                        | <span data-ttu-id="83d91-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="83d91-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="83d91-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83d91-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="83d91-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83d91-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="83d91-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83d91-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83d91-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="83d91-114">Not supported.</span></span>|
|<span data-ttu-id="83d91-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="83d91-115">Application</span></span>                            | <span data-ttu-id="83d91-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83d91-116">AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="83d91-117">登录用户还必须位于允许他们创建访问审阅的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="83d91-117">The signed-in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="83d91-118">有关更多详细信息，请参阅 [access 评审](../resources/accessreviewsv2-root.md)的角色和权限要求。</span><span class="sxs-lookup"><span data-stu-id="83d91-118">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="83d91-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83d91-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a><span data-ttu-id="83d91-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="83d91-120">Request headers</span></span>
| <span data-ttu-id="83d91-121">名称</span><span class="sxs-lookup"><span data-stu-id="83d91-121">Name</span></span>         | <span data-ttu-id="83d91-122">说明</span><span class="sxs-lookup"><span data-stu-id="83d91-122">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="83d91-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83d91-123">Authorization</span></span>|<span data-ttu-id="83d91-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="83d91-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="83d91-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="83d91-126">Content-type</span></span> | <span data-ttu-id="83d91-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="83d91-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83d91-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="83d91-129">Request body</span></span>
<span data-ttu-id="83d91-130">在请求正文中，提供 [accessReview](../resources/accessreview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83d91-130">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="83d91-131">下表显示了为创建 accessReview 而接受的属性。</span><span class="sxs-lookup"><span data-stu-id="83d91-131">The following table shows the properties accepted to create an accessReview.</span></span>

| <span data-ttu-id="83d91-132">属性</span><span class="sxs-lookup"><span data-stu-id="83d91-132">Property</span></span> | <span data-ttu-id="83d91-133">类型</span><span class="sxs-lookup"><span data-stu-id="83d91-133">Type</span></span> | <span data-ttu-id="83d91-134">说明</span><span class="sxs-lookup"><span data-stu-id="83d91-134">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="83d91-135">displayName</span><span class="sxs-lookup"><span data-stu-id="83d91-135">displayName</span></span> | <span data-ttu-id="83d91-136">String</span><span class="sxs-lookup"><span data-stu-id="83d91-136">String</span></span> | <span data-ttu-id="83d91-137">访问审阅系列的名称。</span><span class="sxs-lookup"><span data-stu-id="83d91-137">Name of access review series.</span></span> <span data-ttu-id="83d91-138">必需。</span><span class="sxs-lookup"><span data-stu-id="83d91-138">Required.</span></span>|
| <span data-ttu-id="83d91-139">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="83d91-139">descriptionForAdmins</span></span> | <span data-ttu-id="83d91-140">string</span><span class="sxs-lookup"><span data-stu-id="83d91-140">string</span></span> | <span data-ttu-id="83d91-141">向管理员提供的审阅的上下文。</span><span class="sxs-lookup"><span data-stu-id="83d91-141">Context of the review provided to admins.</span></span> <span data-ttu-id="83d91-142">必需。</span><span class="sxs-lookup"><span data-stu-id="83d91-142">Required.</span></span> |
  <span data-ttu-id="83d91-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="83d91-143">descriptionForReviewers</span></span> | <span data-ttu-id="83d91-144">string</span><span class="sxs-lookup"><span data-stu-id="83d91-144">string</span></span> | <span data-ttu-id="83d91-145">向审阅者提供的审阅的上下文。</span><span class="sxs-lookup"><span data-stu-id="83d91-145">Context of the review provided to reviewers.</span></span> <span data-ttu-id="83d91-146">必需。</span><span class="sxs-lookup"><span data-stu-id="83d91-146">Required.</span></span> |
| <span data-ttu-id="83d91-147">范围</span><span class="sxs-lookup"><span data-stu-id="83d91-147">scope</span></span> | [<span data-ttu-id="83d91-148">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="83d91-148">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="83d91-149">定义在组中审阅的用户的范围。</span><span class="sxs-lookup"><span data-stu-id="83d91-149">Defines the scope of users reviewed in a group.</span></span> <span data-ttu-id="83d91-150">请参阅  [accessReviewScope](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="83d91-150">See  [accessReviewScope](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="83d91-151">必需。</span><span class="sxs-lookup"><span data-stu-id="83d91-151">Required.</span></span>| 
| <span data-ttu-id="83d91-152">instanceEnumerationScope</span><span class="sxs-lookup"><span data-stu-id="83d91-152">instanceEnumerationScope</span></span> | [<span data-ttu-id="83d91-153">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="83d91-153">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="83d91-154">在所有组评审的情况下，这将确定将检查哪些组的范围。</span><span class="sxs-lookup"><span data-stu-id="83d91-154">In the case of an all groups review, this determines the scope of which groups will be reviewed.</span></span> <span data-ttu-id="83d91-155">请参阅 [accessReviewScope](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="83d91-155">See [accessReviewScope](../resources/accessreviewscheduledefinition.md).</span></span> | 
| <span data-ttu-id="83d91-156">settings</span><span class="sxs-lookup"><span data-stu-id="83d91-156">settings</span></span> | [<span data-ttu-id="83d91-157">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="83d91-157">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md)| <span data-ttu-id="83d91-158">Access 审阅系列的设置。</span><span class="sxs-lookup"><span data-stu-id="83d91-158">The settings for an access review series.</span></span> <span data-ttu-id="83d91-159">定期在此处确定。</span><span class="sxs-lookup"><span data-stu-id="83d91-159">Recurrence is determined here.</span></span> <span data-ttu-id="83d91-160">请参阅 [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="83d91-160">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="83d91-161">审批</span><span class="sxs-lookup"><span data-stu-id="83d91-161">reviewers</span></span> | <span data-ttu-id="83d91-162">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83d91-162">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span> | <span data-ttu-id="83d91-163">定义审阅人的身份。</span><span class="sxs-lookup"><span data-stu-id="83d91-163">Defines who the reviewers are.</span></span> <span data-ttu-id="83d91-164">如果未指定，则评审是一个自我审阅 (用户审阅他们自己的访问) 。</span><span class="sxs-lookup"><span data-stu-id="83d91-164">If none are specified, the review is a self-review (users reviewed review their own access).</span></span> <span data-ttu-id="83d91-165">请参阅 [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="83d91-165">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> |


## <a name="response"></a><span data-ttu-id="83d91-166">响应</span><span class="sxs-lookup"><span data-stu-id="83d91-166">Response</span></span>
<span data-ttu-id="83d91-167">如果成功，此方法 `201, Created` 在响应正文中返回响应代码和 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="83d91-167">If successful, this method returns a `201, Created` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83d91-168">示例</span><span class="sxs-lookup"><span data-stu-id="83d91-168">Examples</span></span>

<span data-ttu-id="83d91-169">下面的示例介绍了如何创建具有特定用户（其 user 对象 id 为7eae4444-d425-48b2-adf2-3c777f6256f3，作为审阅者）的 access 审阅系列。</span><span class="sxs-lookup"><span data-stu-id="83d91-169">This is an example of creating an access review series with a specific user, whose user object id is 7eae4444-d425-48b2-adf2-3c777f6256f3, as the reviewer.</span></span> <span data-ttu-id="83d91-170">评审将检查特定组的所有成员，其 group 对象 id 为 b7a059cb-038a-4802-8fc9-b9d1ed0c4444。</span><span class="sxs-lookup"><span data-stu-id="83d91-170">The review reviews all members of a specific group, whose group object id is b7a059cb-038a-4802-8fc9-b9d1ed0c4444.</span></span> <span data-ttu-id="83d91-171">它每周重复发生。</span><span class="sxs-lookup"><span data-stu-id="83d91-171">It recurs weekly.</span></span>

### <a name="request"></a><span data-ttu-id="83d91-172">请求</span><span class="sxs-lookup"><span data-stu-id="83d91-172">Request</span></span>
<span data-ttu-id="83d91-173">在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83d91-173">In the request body, supply a JSON representation of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="83d91-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="83d91-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews
Content-type: application/json

{
  "displayName": "Test create",
  "descriptionForAdmins": "New scheduled access review",
  "descriptionForReviewers": "If you have any questions, contact jerry@contoso.com",
  "scope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0c4444/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [
    {
      "query": "/users/7eae4444-d425-48b2-adf2-3c777f6256f3",
      "queryType": "MicrosoftGraph",
      "queryRoot": "decisions"
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 1,
    "autoApplyDecisionsEnabled": false,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-09-08T12:02:30.667Z"
      }
    }
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="83d91-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83d91-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="83d91-176">响应</span><span class="sxs-lookup"><span data-stu-id="83d91-176">Response</span></span>
><span data-ttu-id="83d91-p113">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="83d91-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "29f2d16e-9ca6-4052-bbfe-802c48944448",
    "displayName": "Test create",
    "createdDateTime": "0001-01-01T00:00:00Z",
    "lastModifiedDateTime": "0001-01-01T00:00:00Z",
    "status": "NotStarted",
    "descriptionForAdmins": "Test create",
    "descriptionForReviewers": "Test create",
    "instanceEnumerationScope": null,
    "createdBy": {
        "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@microsoft.com"
    },
    "scope": {
        "query": "/groups/b74444cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [
        {
            "query": "/users/7eae986b-d425-48b2-adf2-3c777f4444f3",
            "queryType": "MicrosoftGraph",
            "queryRoot": "decisions"
        }
    ],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "None",
        "instanceDurationInDays": 1,
        "autoApplyDecisionsEnabled": false,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": {
                "type": "weekly",
                "interval": 1,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "noEnd",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2020-09-08",
                "endDate": null
            }
        },
        "applyActions": []
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
