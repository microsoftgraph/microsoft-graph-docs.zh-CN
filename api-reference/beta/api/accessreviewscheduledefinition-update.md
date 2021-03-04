---
title: 更新 accessReviewScheduleDefinition
description: 更新现有 accessReviewScheduleDefinition 对象以更改其一个或多个属性。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6d03271d78dea64edf1c410a4bf30886c3e13603
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439014"
---
# <a name="update-accessreviewscheduledefinition"></a><span data-ttu-id="1ec1e-103">更新 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="1ec1e-103">Update accessReviewScheduleDefinition</span></span>

<span data-ttu-id="1ec1e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ec1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ec1e-105">更新现有 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象以更改其一个或多个属性。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-105">Update an existing [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object to change one or more of its properties.</span></span>

>[!NOTE]
><span data-ttu-id="1ec1e-106">对 accessReviewScheduleDefinition 进行的任何更新都仅适用于将来的实例。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-106">Any updates made to an accessReviewScheduleDefinition only apply to future instances.</span></span> <span data-ttu-id="1ec1e-107">当前运行的实例无法更新。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-107">Currently running instances cannot be updated.</span></span>
><span data-ttu-id="1ec1e-108">此外，此 API 不用于更新 accessReviewInstance 级别的属性（包括决策）。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-108">Additionally, this API is not intended to update properties, including decisions, on the accessReviewInstance level.</span></span> <span data-ttu-id="1ec1e-109">有关[实例详细信息，请参阅 accessReviewInstance。](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="1ec1e-109">See [accessReviewInstance](../resources/accessreviewinstance.md) for more information on instances.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ec1e-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="1ec1e-110">Permissions</span></span>
<span data-ttu-id="1ec1e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ec1e-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ec1e-113">Permission type</span></span>                        | <span data-ttu-id="1ec1e-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ec1e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ec1e-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ec1e-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ec1e-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ec1e-116">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="1ec1e-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ec1e-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ec1e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-118">Not supported.</span></span>|
|<span data-ttu-id="1ec1e-119">Application</span><span class="sxs-lookup"><span data-stu-id="1ec1e-119">Application</span></span>                            | <span data-ttu-id="1ec1e-120">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ec1e-120">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ec1e-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ec1e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="1ec1e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ec1e-122">Request headers</span></span>
| <span data-ttu-id="1ec1e-123">名称</span><span class="sxs-lookup"><span data-stu-id="1ec1e-123">Name</span></span>         | <span data-ttu-id="1ec1e-124">说明</span><span class="sxs-lookup"><span data-stu-id="1ec1e-124">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="1ec1e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ec1e-125">Authorization</span></span>|<span data-ttu-id="1ec1e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="1ec1e-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="1ec1e-128">Content-type</span></span> | <span data-ttu-id="1ec1e-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1ec1e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ec1e-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ec1e-131">Request body</span></span>
<span data-ttu-id="1ec1e-132">在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-132">In the request body, supply a JSON representation of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="1ec1e-133">下表显示了接受用于更新 accessReviewScheduleDefinition 的属性。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-133">The following table shows the properties accepted to update an accessReviewScheduleDefinition.</span></span>

| <span data-ttu-id="1ec1e-134">属性</span><span class="sxs-lookup"><span data-stu-id="1ec1e-134">Property</span></span> | <span data-ttu-id="1ec1e-135">类型</span><span class="sxs-lookup"><span data-stu-id="1ec1e-135">Type</span></span> | <span data-ttu-id="1ec1e-136">说明</span><span class="sxs-lookup"><span data-stu-id="1ec1e-136">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1ec1e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1ec1e-137">displayName</span></span> | <span data-ttu-id="1ec1e-138">String</span><span class="sxs-lookup"><span data-stu-id="1ec1e-138">String</span></span> | <span data-ttu-id="1ec1e-139">访问评审系列的名称。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-139">Name of access review series.</span></span> |
| <span data-ttu-id="1ec1e-140">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="1ec1e-140">descriptionForAdmins</span></span> | <span data-ttu-id="1ec1e-141">String</span><span class="sxs-lookup"><span data-stu-id="1ec1e-141">String</span></span> | <span data-ttu-id="1ec1e-142">提供给管理员的审阅上下文。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-142">Context of the review provided to admins.</span></span> |
| <span data-ttu-id="1ec1e-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="1ec1e-143">descriptionForReviewers</span></span> | <span data-ttu-id="1ec1e-144">String</span><span class="sxs-lookup"><span data-stu-id="1ec1e-144">String</span></span> | <span data-ttu-id="1ec1e-145">提供给审阅者的审阅上下文。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-145">Context of the review provided to reviewers.</span></span> |
| <span data-ttu-id="1ec1e-146">settings</span><span class="sxs-lookup"><span data-stu-id="1ec1e-146">settings</span></span> | [<span data-ttu-id="1ec1e-147">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="1ec1e-147">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md) | <span data-ttu-id="1ec1e-148">访问评审系列的设置。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-148">The settings for an access review series.</span></span> <span data-ttu-id="1ec1e-149">请参阅 [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-149">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="1ec1e-150">审阅者</span><span class="sxs-lookup"><span data-stu-id="1ec1e-150">reviewers</span></span> | <span data-ttu-id="1ec1e-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ec1e-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|  <span data-ttu-id="1ec1e-152">定义审阅者是谁。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-152">Defines who the reviewers are.</span></span> <span data-ttu-id="1ec1e-153">如果未指定任何内容，则评价是自 (审阅用户自己的访问权限) 。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-153">If none are specified, the review is a self-review (users reviewed review their own access).</span></span> <span data-ttu-id="1ec1e-154">只有在分配了单个用户为审阅者时，Reviewers 属性才可更新。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-154">The Reviewers property is only updatable if individual users assigned are as reviewers.</span></span> <span data-ttu-id="1ec1e-155">请参阅 [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-155">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> | 

<span data-ttu-id="1ec1e-156">请注意，PUT 请求需要传入整个对象，其中包括所有可写属性，而不只是要更新的属性。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-156">Note that a PUT request expects the full object to be passed in, in which all writable properties are included, not just the properties being updated.</span></span>

## <a name="response"></a><span data-ttu-id="1ec1e-157">响应</span><span class="sxs-lookup"><span data-stu-id="1ec1e-157">Response</span></span>
<span data-ttu-id="1ec1e-158">如果成功，此方法将返回 `204, Accepted` 响应代码，并且不会返回响应正文。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-158">If successful, this method returns a `204, Accepted` response code and no response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ec1e-159">示例</span><span class="sxs-lookup"><span data-stu-id="1ec1e-159">Examples</span></span>

<span data-ttu-id="1ec1e-160">这是更新现有访问评审系列的 displayName 的示例。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-160">This is an example of updating the displayName of an existing access review series.</span></span>

### <a name="request"></a><span data-ttu-id="1ec1e-161">请求</span><span class="sxs-lookup"><span data-stu-id="1ec1e-161">Request</span></span>
<span data-ttu-id="1ec1e-162">在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的新属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-162">In the request body, supply a JSON representation of the new properties of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>



# <a name="http"></a>[<span data-ttu-id="1ec1e-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ec1e-163">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="1ec1e-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ec1e-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ec1e-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ec1e-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="1ec1e-166">C#</span><span class="sxs-lookup"><span data-stu-id="1ec1e-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1ec1e-167">Java</span><span class="sxs-lookup"><span data-stu-id="1ec1e-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="1ec1e-168">响应</span><span class="sxs-lookup"><span data-stu-id="1ec1e-168">Response</span></span>
><span data-ttu-id="1ec1e-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1ec1e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 Accepted
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
