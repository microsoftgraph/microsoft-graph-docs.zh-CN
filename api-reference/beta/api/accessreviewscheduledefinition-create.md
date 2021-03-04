---
title: 创建 accessReviewScheduleDefinition
description: 创建新的 accessReviewScheduleDefinition 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b82980e053a50b7562cf94d0a5224badfd1d2a8a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439098"
---
# <a name="create-accessreviewscheduledefinition"></a><span data-ttu-id="a57c2-103">创建 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="a57c2-103">Create accessReviewScheduleDefinition</span></span>

<span data-ttu-id="a57c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a57c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a57c2-105">创建新的 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a57c2-105">Create a new [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a57c2-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a57c2-106">Permissions</span></span>

<span data-ttu-id="a57c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a57c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a57c2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a57c2-109">Permission type</span></span>                        | <span data-ttu-id="a57c2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a57c2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a57c2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a57c2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a57c2-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a57c2-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="a57c2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a57c2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a57c2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a57c2-114">Not supported.</span></span>|
|<span data-ttu-id="a57c2-115">Application</span><span class="sxs-lookup"><span data-stu-id="a57c2-115">Application</span></span>                            | <span data-ttu-id="a57c2-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a57c2-116">AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="a57c2-117">登录用户还必须具有允许其创建访问评审的目录角色。</span><span class="sxs-lookup"><span data-stu-id="a57c2-117">The signed-in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="a57c2-118">有关详细信息，请参阅访问评审的角色 [和权限要求](../resources/accessreviewsv2-root.md)。</span><span class="sxs-lookup"><span data-stu-id="a57c2-118">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="a57c2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a57c2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a><span data-ttu-id="a57c2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a57c2-120">Request headers</span></span>
| <span data-ttu-id="a57c2-121">名称</span><span class="sxs-lookup"><span data-stu-id="a57c2-121">Name</span></span>         | <span data-ttu-id="a57c2-122">说明</span><span class="sxs-lookup"><span data-stu-id="a57c2-122">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="a57c2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a57c2-123">Authorization</span></span>|<span data-ttu-id="a57c2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a57c2-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="a57c2-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="a57c2-126">Content-type</span></span> | <span data-ttu-id="a57c2-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a57c2-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a57c2-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a57c2-129">Request body</span></span>
<span data-ttu-id="a57c2-130">在请求正文中，提供 [accessReview](../resources/accessreview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a57c2-130">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="a57c2-131">下表显示了创建 accessReview 时接受的属性。</span><span class="sxs-lookup"><span data-stu-id="a57c2-131">The following table shows the properties accepted to create an accessReview.</span></span>

| <span data-ttu-id="a57c2-132">属性</span><span class="sxs-lookup"><span data-stu-id="a57c2-132">Property</span></span> | <span data-ttu-id="a57c2-133">类型</span><span class="sxs-lookup"><span data-stu-id="a57c2-133">Type</span></span> | <span data-ttu-id="a57c2-134">说明</span><span class="sxs-lookup"><span data-stu-id="a57c2-134">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a57c2-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a57c2-135">displayName</span></span> | <span data-ttu-id="a57c2-136">String</span><span class="sxs-lookup"><span data-stu-id="a57c2-136">String</span></span> | <span data-ttu-id="a57c2-137">访问评审系列的名称。</span><span class="sxs-lookup"><span data-stu-id="a57c2-137">Name of access review series.</span></span> <span data-ttu-id="a57c2-138">必需。</span><span class="sxs-lookup"><span data-stu-id="a57c2-138">Required.</span></span>|
| <span data-ttu-id="a57c2-139">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="a57c2-139">descriptionForAdmins</span></span> | <span data-ttu-id="a57c2-140">string</span><span class="sxs-lookup"><span data-stu-id="a57c2-140">string</span></span> | <span data-ttu-id="a57c2-141">提供给管理员的审阅上下文。</span><span class="sxs-lookup"><span data-stu-id="a57c2-141">Context of the review provided to admins.</span></span> <span data-ttu-id="a57c2-142">必需。</span><span class="sxs-lookup"><span data-stu-id="a57c2-142">Required.</span></span> |
  <span data-ttu-id="a57c2-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="a57c2-143">descriptionForReviewers</span></span> | <span data-ttu-id="a57c2-144">string</span><span class="sxs-lookup"><span data-stu-id="a57c2-144">string</span></span> | <span data-ttu-id="a57c2-145">提供给审阅者的审阅上下文。</span><span class="sxs-lookup"><span data-stu-id="a57c2-145">Context of the review provided to reviewers.</span></span> <span data-ttu-id="a57c2-146">必需。</span><span class="sxs-lookup"><span data-stu-id="a57c2-146">Required.</span></span> |
| <span data-ttu-id="a57c2-147">范围</span><span class="sxs-lookup"><span data-stu-id="a57c2-147">scope</span></span> | [<span data-ttu-id="a57c2-148">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="a57c2-148">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="a57c2-149">定义在组中审阅的用户范围。</span><span class="sxs-lookup"><span data-stu-id="a57c2-149">Defines the scope of users reviewed in a group.</span></span> <span data-ttu-id="a57c2-150">请参阅  [accessReviewScope](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="a57c2-150">See  [accessReviewScope](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="a57c2-151">必需。</span><span class="sxs-lookup"><span data-stu-id="a57c2-151">Required.</span></span>| 
| <span data-ttu-id="a57c2-152">instanceEnumerationScope</span><span class="sxs-lookup"><span data-stu-id="a57c2-152">instanceEnumerationScope</span></span> | [<span data-ttu-id="a57c2-153">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="a57c2-153">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="a57c2-154">对于所有组审阅，这将确定将审阅哪些组的范围。</span><span class="sxs-lookup"><span data-stu-id="a57c2-154">In the case of an all groups review, this determines the scope of which groups will be reviewed.</span></span> <span data-ttu-id="a57c2-155">请参阅 [accessReviewScope](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="a57c2-155">See [accessReviewScope](../resources/accessreviewscheduledefinition.md).</span></span> | 
| <span data-ttu-id="a57c2-156">settings</span><span class="sxs-lookup"><span data-stu-id="a57c2-156">settings</span></span> | [<span data-ttu-id="a57c2-157">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="a57c2-157">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md)| <span data-ttu-id="a57c2-158">访问评审系列的设置。</span><span class="sxs-lookup"><span data-stu-id="a57c2-158">The settings for an access review series.</span></span> <span data-ttu-id="a57c2-159">定期在此处确定。</span><span class="sxs-lookup"><span data-stu-id="a57c2-159">Recurrence is determined here.</span></span> <span data-ttu-id="a57c2-160">请参阅 [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="a57c2-160">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="a57c2-161">审阅者</span><span class="sxs-lookup"><span data-stu-id="a57c2-161">reviewers</span></span> | <span data-ttu-id="a57c2-162">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a57c2-162">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span> | <span data-ttu-id="a57c2-163">定义审阅者是谁。</span><span class="sxs-lookup"><span data-stu-id="a57c2-163">Defines who the reviewers are.</span></span> <span data-ttu-id="a57c2-164">如果未指定任何内容，则评价是自 (审阅用户自己的访问权限) 。</span><span class="sxs-lookup"><span data-stu-id="a57c2-164">If none are specified, the review is a self-review (users reviewed review their own access).</span></span> <span data-ttu-id="a57c2-165">请参阅 [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="a57c2-165">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> |


## <a name="response"></a><span data-ttu-id="a57c2-166">响应</span><span class="sxs-lookup"><span data-stu-id="a57c2-166">Response</span></span>
<span data-ttu-id="a57c2-167">如果成功，此方法在响应正文中返回响应代码和 `201, Created` [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a57c2-167">If successful, this method returns a `201, Created` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a57c2-168">示例</span><span class="sxs-lookup"><span data-stu-id="a57c2-168">Examples</span></span>

<span data-ttu-id="a57c2-169">这是一个使用特定用户创建访问评审系列的示例，该用户的用户对象 ID 为 7eae4444-d425-48b2-adf2-3c777f6256f3，作为审阅者。</span><span class="sxs-lookup"><span data-stu-id="a57c2-169">This is an example of creating an access review series with a specific user, whose user object id is 7eae4444-d425-48b2-adf2-3c777f6256f3, as the reviewer.</span></span> <span data-ttu-id="a57c2-170">审阅将审阅特定组的所有成员，其组对象 ID 为 b7a059cb-038a-4802-8fc9-b9d1ed0c4444。</span><span class="sxs-lookup"><span data-stu-id="a57c2-170">The review reviews all members of a specific group, whose group object id is b7a059cb-038a-4802-8fc9-b9d1ed0c4444.</span></span> <span data-ttu-id="a57c2-171">每周重复一次。</span><span class="sxs-lookup"><span data-stu-id="a57c2-171">It recurs weekly.</span></span>

### <a name="request"></a><span data-ttu-id="a57c2-172">请求</span><span class="sxs-lookup"><span data-stu-id="a57c2-172">Request</span></span>
<span data-ttu-id="a57c2-173">在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a57c2-173">In the request body, supply a JSON representation of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="a57c2-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="a57c2-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
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
# <a name="javascript"></a>[<span data-ttu-id="a57c2-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a57c2-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="a57c2-176">C#</span><span class="sxs-lookup"><span data-stu-id="a57c2-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a57c2-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a57c2-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a57c2-178">Java</span><span class="sxs-lookup"><span data-stu-id="a57c2-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a57c2-179">响应</span><span class="sxs-lookup"><span data-stu-id="a57c2-179">Response</span></span>
><span data-ttu-id="a57c2-p113">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a57c2-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
        "userPrincipalName": "admin@contoso.com"
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
