---
title: 更新 accessReviewScheduleDefinition
description: 更新现有 accessReviewScheduleDefinition 对象以更改其一个或多个属性。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0fe437806ee9fdb71535c16dab8c7ff07f631f39
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579632"
---
# <a name="update-accessreviewscheduledefinition"></a><span data-ttu-id="e381c-103">更新 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="e381c-103">Update accessReviewScheduleDefinition</span></span>

<span data-ttu-id="e381c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e381c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e381c-105">更新现有 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象以更改其一个或多个属性。</span><span class="sxs-lookup"><span data-stu-id="e381c-105">Update an existing [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object to change one or more of its properties.</span></span>

>[!NOTE]
><span data-ttu-id="e381c-106">对 accessReviewScheduleDefinition 进行的任何更新都仅适用于将来实例。</span><span class="sxs-lookup"><span data-stu-id="e381c-106">Any updates made to an accessReviewScheduleDefinition only apply to future instances.</span></span> <span data-ttu-id="e381c-107">当前运行的实例无法更新。</span><span class="sxs-lookup"><span data-stu-id="e381c-107">Currently running instances cannot be updated.</span></span>
><span data-ttu-id="e381c-108">此外，此 API 不用于更新 accessReviewInstance 级别的属性（包括决策）。</span><span class="sxs-lookup"><span data-stu-id="e381c-108">Additionally, this API is not intended to update properties, including decisions, on the accessReviewInstance level.</span></span> <span data-ttu-id="e381c-109">有关[实例详细信息，请参阅 accessReviewInstance。](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="e381c-109">See [accessReviewInstance](../resources/accessreviewinstance.md) for more information on instances.</span></span>

## <a name="permissions"></a><span data-ttu-id="e381c-110">权限</span><span class="sxs-lookup"><span data-stu-id="e381c-110">Permissions</span></span>
<span data-ttu-id="e381c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e381c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e381c-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="e381c-113">Permission type</span></span>                        | <span data-ttu-id="e381c-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e381c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e381c-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e381c-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="e381c-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e381c-116">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="e381c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e381c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e381c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e381c-118">Not supported.</span></span>|
|<span data-ttu-id="e381c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="e381c-119">Application</span></span>                            | <span data-ttu-id="e381c-120">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e381c-120">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e381c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e381c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="e381c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e381c-122">Request headers</span></span>
| <span data-ttu-id="e381c-123">名称</span><span class="sxs-lookup"><span data-stu-id="e381c-123">Name</span></span>         | <span data-ttu-id="e381c-124">说明</span><span class="sxs-lookup"><span data-stu-id="e381c-124">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="e381c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e381c-125">Authorization</span></span>|<span data-ttu-id="e381c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e381c-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="e381c-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="e381c-128">Content-type</span></span> | <span data-ttu-id="e381c-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e381c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e381c-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="e381c-131">Request body</span></span>
<span data-ttu-id="e381c-132">在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e381c-132">In the request body, supply a JSON representation of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="e381c-133">下表显示接受用于更新 accessReviewScheduleDefinition 的属性。</span><span class="sxs-lookup"><span data-stu-id="e381c-133">The following table shows the properties accepted to update an accessReviewScheduleDefinition.</span></span>

| <span data-ttu-id="e381c-134">属性</span><span class="sxs-lookup"><span data-stu-id="e381c-134">Property</span></span> | <span data-ttu-id="e381c-135">类型</span><span class="sxs-lookup"><span data-stu-id="e381c-135">Type</span></span> | <span data-ttu-id="e381c-136">说明</span><span class="sxs-lookup"><span data-stu-id="e381c-136">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e381c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e381c-137">displayName</span></span> | <span data-ttu-id="e381c-138">String</span><span class="sxs-lookup"><span data-stu-id="e381c-138">String</span></span> | <span data-ttu-id="e381c-139">访问评审系列的名称。</span><span class="sxs-lookup"><span data-stu-id="e381c-139">Name of access review series.</span></span> |
| <span data-ttu-id="e381c-140">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="e381c-140">descriptionForAdmins</span></span> | <span data-ttu-id="e381c-141">String</span><span class="sxs-lookup"><span data-stu-id="e381c-141">String</span></span> | <span data-ttu-id="e381c-142">提供给管理员评价的上下文。</span><span class="sxs-lookup"><span data-stu-id="e381c-142">Context of the review provided to admins.</span></span> |
| <span data-ttu-id="e381c-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="e381c-143">descriptionForReviewers</span></span> | <span data-ttu-id="e381c-144">String</span><span class="sxs-lookup"><span data-stu-id="e381c-144">String</span></span> | <span data-ttu-id="e381c-145">提供给审阅者的审阅上下文。</span><span class="sxs-lookup"><span data-stu-id="e381c-145">Context of the review provided to reviewers.</span></span> |
| <span data-ttu-id="e381c-146">settings</span><span class="sxs-lookup"><span data-stu-id="e381c-146">settings</span></span> | [<span data-ttu-id="e381c-147">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="e381c-147">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md) | <span data-ttu-id="e381c-148">访问评审系列的设置。</span><span class="sxs-lookup"><span data-stu-id="e381c-148">The settings for an access review series.</span></span> <span data-ttu-id="e381c-149">请参阅 [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="e381c-149">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="e381c-150">reviewers</span><span class="sxs-lookup"><span data-stu-id="e381c-150">reviewers</span></span> | <span data-ttu-id="e381c-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e381c-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|  <span data-ttu-id="e381c-152">定义审阅者是谁。</span><span class="sxs-lookup"><span data-stu-id="e381c-152">Defines who the reviewers are.</span></span> <span data-ttu-id="e381c-153">如果未指定任何内容，则评论是自 (审阅用户自己的访问权限或) 。</span><span class="sxs-lookup"><span data-stu-id="e381c-153">If none are specified, the review is a self-review (users reviewed review their own access).</span></span> <span data-ttu-id="e381c-154">Reviewers 属性仅在分配了单个用户为审阅者时可更新。</span><span class="sxs-lookup"><span data-stu-id="e381c-154">The Reviewers property is only updatable if individual users assigned are as reviewers.</span></span> <span data-ttu-id="e381c-155">请参阅 [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="e381c-155">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> | 

<span data-ttu-id="e381c-156">**PUT** 请求希望传入完整的对象，其中包括所有可写属性，而不只是要更新的属性。</span><span class="sxs-lookup"><span data-stu-id="e381c-156">A **PUT** request expects the full object to be passed in, which includes all writable properties, not just the properties being updated.</span></span>

## <a name="response"></a><span data-ttu-id="e381c-157">响应</span><span class="sxs-lookup"><span data-stu-id="e381c-157">Response</span></span>
<span data-ttu-id="e381c-158">如果成功，此方法返回 响应 `204 No Content` 代码，无响应正文。</span><span class="sxs-lookup"><span data-stu-id="e381c-158">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e381c-159">示例</span><span class="sxs-lookup"><span data-stu-id="e381c-159">Examples</span></span>

<span data-ttu-id="e381c-160">这是更新现有访问评审系列的 displayName 的示例。</span><span class="sxs-lookup"><span data-stu-id="e381c-160">This is an example of updating the displayName of an existing access review series.</span></span>

### <a name="request"></a><span data-ttu-id="e381c-161">请求</span><span class="sxs-lookup"><span data-stu-id="e381c-161">Request</span></span>
<span data-ttu-id="e381c-162">在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的新属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e381c-162">In the request body, supply a JSON representation of the new properties of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>



# <a name="http"></a>[<span data-ttu-id="e381c-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="e381c-163">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="e381c-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e381c-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e381c-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e381c-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="e381c-166">C#</span><span class="sxs-lookup"><span data-stu-id="e381c-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e381c-167">Java</span><span class="sxs-lookup"><span data-stu-id="e381c-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="e381c-168">响应</span><span class="sxs-lookup"><span data-stu-id="e381c-168">Response</span></span>
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
