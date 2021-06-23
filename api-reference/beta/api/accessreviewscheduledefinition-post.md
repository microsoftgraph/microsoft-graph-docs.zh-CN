---
title: 创建 accessReviewScheduleDefinition
description: 创建新的 accessReviewScheduleDefinition 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b4fe8b50f52b67019569c7bded140837091e1ee7
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060008"
---
# <a name="create-accessreviewscheduledefinition"></a><span data-ttu-id="4a22d-103">创建 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="4a22d-103">Create accessReviewScheduleDefinition</span></span>

<span data-ttu-id="4a22d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a22d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a22d-105">创建新的 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4a22d-105">Create a new [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a22d-106">权限</span><span class="sxs-lookup"><span data-stu-id="4a22d-106">Permissions</span></span>

<span data-ttu-id="4a22d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a22d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a22d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a22d-109">Permission type</span></span>                        | <span data-ttu-id="4a22d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4a22d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a22d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a22d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a22d-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a22d-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="4a22d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a22d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a22d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a22d-114">Not supported.</span></span>|
|<span data-ttu-id="4a22d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a22d-115">Application</span></span>                            | <span data-ttu-id="4a22d-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a22d-116">AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="4a22d-117">登录用户还必须具有允许其创建访问评审的目录角色。</span><span class="sxs-lookup"><span data-stu-id="4a22d-117">The signed-in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="4a22d-118">有关详细信息，请参阅访问评审的角色和 [权限要求](../resources/accessreviewsv2-root.md)。</span><span class="sxs-lookup"><span data-stu-id="4a22d-118">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="4a22d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a22d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a><span data-ttu-id="4a22d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a22d-120">Request headers</span></span>
| <span data-ttu-id="4a22d-121">名称</span><span class="sxs-lookup"><span data-stu-id="4a22d-121">Name</span></span>         | <span data-ttu-id="4a22d-122">说明</span><span class="sxs-lookup"><span data-stu-id="4a22d-122">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="4a22d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a22d-123">Authorization</span></span>|<span data-ttu-id="4a22d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4a22d-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="4a22d-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="4a22d-126">Content-type</span></span> | <span data-ttu-id="4a22d-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4a22d-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a22d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a22d-129">Request body</span></span>
<span data-ttu-id="4a22d-130">在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a22d-130">In the request body, supply a JSON representation of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="4a22d-131">下表显示了创建 accessReview 时接受的属性。</span><span class="sxs-lookup"><span data-stu-id="4a22d-131">The following table shows the properties accepted to create an accessReview.</span></span>

| <span data-ttu-id="4a22d-132">属性</span><span class="sxs-lookup"><span data-stu-id="4a22d-132">Property</span></span> | <span data-ttu-id="4a22d-133">类型</span><span class="sxs-lookup"><span data-stu-id="4a22d-133">Type</span></span> | <span data-ttu-id="4a22d-134">说明</span><span class="sxs-lookup"><span data-stu-id="4a22d-134">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4a22d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4a22d-135">displayName</span></span> | <span data-ttu-id="4a22d-136">String</span><span class="sxs-lookup"><span data-stu-id="4a22d-136">String</span></span> | <span data-ttu-id="4a22d-137">访问评审系列的名称。</span><span class="sxs-lookup"><span data-stu-id="4a22d-137">Name of access review series.</span></span> <span data-ttu-id="4a22d-138">必填。</span><span class="sxs-lookup"><span data-stu-id="4a22d-138">Required.</span></span>|
| <span data-ttu-id="4a22d-139">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="4a22d-139">descriptionForAdmins</span></span> | <span data-ttu-id="4a22d-140">string</span><span class="sxs-lookup"><span data-stu-id="4a22d-140">string</span></span> | <span data-ttu-id="4a22d-141">提供给管理员评价的上下文。</span><span class="sxs-lookup"><span data-stu-id="4a22d-141">Context of the review provided to admins.</span></span> <span data-ttu-id="4a22d-142">必填。</span><span class="sxs-lookup"><span data-stu-id="4a22d-142">Required.</span></span> |
  <span data-ttu-id="4a22d-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="4a22d-143">descriptionForReviewers</span></span> | <span data-ttu-id="4a22d-144">string</span><span class="sxs-lookup"><span data-stu-id="4a22d-144">string</span></span> | <span data-ttu-id="4a22d-145">提供给审阅者的审阅上下文。</span><span class="sxs-lookup"><span data-stu-id="4a22d-145">Context of the review provided to reviewers.</span></span> <span data-ttu-id="4a22d-146">必填。</span><span class="sxs-lookup"><span data-stu-id="4a22d-146">Required.</span></span> |
| <span data-ttu-id="4a22d-147">范围</span><span class="sxs-lookup"><span data-stu-id="4a22d-147">scope</span></span> | [<span data-ttu-id="4a22d-148">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="4a22d-148">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="4a22d-149">定义在组中查看的用户范围。</span><span class="sxs-lookup"><span data-stu-id="4a22d-149">Defines the scope of users reviewed in a group.</span></span> <span data-ttu-id="4a22d-150">请参阅  [accessReviewScope，](../resources/accessreviewscheduledefinition.md) 并了解如何 [配置访问评审定义的范围](/graph/accessreviews-scope-concept)。</span><span class="sxs-lookup"><span data-stu-id="4a22d-150">See  [accessReviewScope](../resources/accessreviewscheduledefinition.md) and also learn how to [configure the scope of your access review definition](/graph/accessreviews-scope-concept).</span></span> <span data-ttu-id="4a22d-151">必填。</span><span class="sxs-lookup"><span data-stu-id="4a22d-151">Required.</span></span>| 
| <span data-ttu-id="4a22d-152">instanceEnumerationScope</span><span class="sxs-lookup"><span data-stu-id="4a22d-152">instanceEnumerationScope</span></span> | [<span data-ttu-id="4a22d-153">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="4a22d-153">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="4a22d-154">对于所有组评审，这将确定将审核哪些组的范围。</span><span class="sxs-lookup"><span data-stu-id="4a22d-154">In the case of an all groups review, this determines the scope of which groups will be reviewed.</span></span> <span data-ttu-id="4a22d-155">请参阅 [accessReviewScope，](../resources/accessreviewscheduledefinition.md) 并了解如何 [配置访问评审定义的范围](/graph/accessreviews-scope-concept)。</span><span class="sxs-lookup"><span data-stu-id="4a22d-155">See [accessReviewScope](../resources/accessreviewscheduledefinition.md) and also learn how to [configure the scope of your access review definition](/graph/accessreviews-scope-concept).</span></span>| 
| <span data-ttu-id="4a22d-156">设置</span><span class="sxs-lookup"><span data-stu-id="4a22d-156">settings</span></span> | [<span data-ttu-id="4a22d-157">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="4a22d-157">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md)| <span data-ttu-id="4a22d-158">访问评审系列的设置。</span><span class="sxs-lookup"><span data-stu-id="4a22d-158">The settings for an access review series.</span></span> <span data-ttu-id="4a22d-159">定期在此处确定。</span><span class="sxs-lookup"><span data-stu-id="4a22d-159">Recurrence is determined here.</span></span> <span data-ttu-id="4a22d-160">请参阅 [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="4a22d-160">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="4a22d-161">reviewers</span><span class="sxs-lookup"><span data-stu-id="4a22d-161">reviewers</span></span> | <span data-ttu-id="4a22d-162">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4a22d-162">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span> | <span data-ttu-id="4a22d-163">定义审阅者是谁。</span><span class="sxs-lookup"><span data-stu-id="4a22d-163">Defines who the reviewers are.</span></span> <span data-ttu-id="4a22d-164">如果未指定任何内容，则评论是自 (审阅用户自己的访问权限或) 。</span><span class="sxs-lookup"><span data-stu-id="4a22d-164">If none are specified, the review is a self-review (users reviewed review their own access).</span></span>  <span data-ttu-id="4a22d-165">有关分配审阅者的选项示例，请参阅使用 Microsoft Graph API 将审阅者[分配给你的访问Graph定义](/graph/accessreviews-reviewers-concept)。</span><span class="sxs-lookup"><span data-stu-id="4a22d-165">For examples of options for assigning reviewers, see [Assign reviewers to your access review definition using the Microsoft Graph API](/graph/accessreviews-reviewers-concept).</span></span> |
|<span data-ttu-id="4a22d-166">fallbackReviewers</span><span class="sxs-lookup"><span data-stu-id="4a22d-166">fallbackReviewers</span></span>|<span data-ttu-id="4a22d-167">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4a22d-167">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="4a22d-168">如果提供，当主审阅者不存在时，会要求回退审阅者完成审阅。</span><span class="sxs-lookup"><span data-stu-id="4a22d-168">If provided, the fallback reviewers are asked to complete a review if the primary reviewers do not exist.</span></span> <span data-ttu-id="4a22d-169">例如，如果选择了经理作为，而审核中的主体在 Azure AD 中没有经理，则回退审阅者 `reviewers` 需要审阅该主体。</span><span class="sxs-lookup"><span data-stu-id="4a22d-169">For example, if managers are selected as `reviewers` and a principal under review does not have a manager in Azure AD, the fallback reviewers are asked to review that principal.</span></span>|
| <span data-ttu-id="4a22d-170">additionalNotificationRecipients</span><span class="sxs-lookup"><span data-stu-id="4a22d-170">additionalNotificationRecipients</span></span>   |<span data-ttu-id="4a22d-171">[accessReviewNotificationRecipientItem](../resources/accessReviewNotificationRecipientItem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4a22d-171">[accessReviewNotificationRecipientItem](../resources/accessReviewNotificationRecipientItem.md) collection</span></span>| <span data-ttu-id="4a22d-172">定义要接收访问评审进度通知的其他用户或组成员的列表。</span><span class="sxs-lookup"><span data-stu-id="4a22d-172">Defines the list of additional users or group members to be notified of the access review progress.</span></span> |
| <span data-ttu-id="4a22d-173">backupReviewers (弃用) </span><span class="sxs-lookup"><span data-stu-id="4a22d-173">backupReviewers (deprecated)</span></span> |<span data-ttu-id="4a22d-174">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4a22d-174">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>| <span data-ttu-id="4a22d-175">此属性已被 **fallbackReviewers 取代**。</span><span class="sxs-lookup"><span data-stu-id="4a22d-175">This property has been replaced by **fallbackReviewers**.</span></span> <span data-ttu-id="4a22d-176">但是，指定 **backupReviewers** 或 **fallbackReviewers** 会自动向另一个属性填充相同的值。</span><span class="sxs-lookup"><span data-stu-id="4a22d-176">However, specifying either **backupReviewers** or **fallbackReviewers** automatically populates the same values to the other property.</span></span> |

## <a name="response"></a><span data-ttu-id="4a22d-177">响应</span><span class="sxs-lookup"><span data-stu-id="4a22d-177">Response</span></span>
<span data-ttu-id="4a22d-178">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4a22d-178">If successful, this method returns a `201 Created` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4a22d-179">示例</span><span class="sxs-lookup"><span data-stu-id="4a22d-179">Examples</span></span>

### <a name="example-1-create-an-access-review-on-a-group"></a><span data-ttu-id="4a22d-180">示例 1：在组上创建访问评审</span><span class="sxs-lookup"><span data-stu-id="4a22d-180">Example 1: Create an access review on a group</span></span>

<span data-ttu-id="4a22d-181">这是一个创建具有以下设置的访问评审的示例：</span><span class="sxs-lookup"><span data-stu-id="4a22d-181">This is an example of creating an access review with the following settings:</span></span>
+ <span data-ttu-id="4a22d-182">评价将审阅组的所有成员，其组 **ID 为** `02f3bafb-448c-487c-88c2-5fd65ce49a41` 。</span><span class="sxs-lookup"><span data-stu-id="4a22d-182">The review reviews all members of a group, whose group **id** is `02f3bafb-448c-487c-88c2-5fd65ce49a41`.</span></span>
+ <span data-ttu-id="4a22d-183">用户 ID 为审阅 **者** `398164b1-5196-49dd-ada2-364b49f99b27` 的特定用户。</span><span class="sxs-lookup"><span data-stu-id="4a22d-183">A specific user, whose user **id** is `398164b1-5196-49dd-ada2-364b49f99b27` is the reviewer.</span></span>
+ <span data-ttu-id="4a22d-184">它每周重复一次，并无限期地继续。</span><span class="sxs-lookup"><span data-stu-id="4a22d-184">It recurs weekly and continues indefinitely.</span></span>

#### <a name="request"></a><span data-ttu-id="4a22d-185">请求</span><span class="sxs-lookup"><span data-stu-id="4a22d-185">Request</span></span>
<span data-ttu-id="4a22d-186">在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a22d-186">In the request body, supply a JSON representation of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="4a22d-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a22d-187">HTTP</span></span>](#tab/http)
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
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/02f3bafb-448c-487c-88c2-5fd65ce49a41/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [
    {
      "query": "/users/398164b1-5196-49dd-ada2-364b49f99b27",
      "queryType": "MicrosoftGraph"
    }
  ],  
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 1,
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
# <a name="javascript"></a>[<span data-ttu-id="4a22d-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a22d-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="4a22d-189">C#</span><span class="sxs-lookup"><span data-stu-id="4a22d-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a22d-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a22d-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a22d-191">Java</span><span class="sxs-lookup"><span data-stu-id="4a22d-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4a22d-192">响应</span><span class="sxs-lookup"><span data-stu-id="4a22d-192">Response</span></span>
><span data-ttu-id="4a22d-193">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4a22d-193">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
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

### <a name="example-2-create-an-access-review-on-all-teams-with-inactive-guest-users"></a><span data-ttu-id="4a22d-194">示例 2：在具有非活动来宾用户的所有团队上创建访问评审</span><span class="sxs-lookup"><span data-stu-id="4a22d-194">Example 2: Create an access review on all teams with inactive guest users</span></span>

<span data-ttu-id="4a22d-195">这是一个创建具有以下设置的访问评审的示例：</span><span class="sxs-lookup"><span data-stu-id="4a22d-195">This is an example of creating an access review with the following settings:</span></span>
+ <span data-ttu-id="4a22d-196">该评论将审核具有非活动来宾用户的所有团队。</span><span class="sxs-lookup"><span data-stu-id="4a22d-196">The review reviews all teams with inactive guest users.</span></span> <span data-ttu-id="4a22d-197">非活动期为自访问评审开始日期起 30 天。</span><span class="sxs-lookup"><span data-stu-id="4a22d-197">The period of inactivity is 30 days from the start date of the access review.</span></span>
+ <span data-ttu-id="4a22d-198">组所有者为审阅者，并分配回退审阅者。</span><span class="sxs-lookup"><span data-stu-id="4a22d-198">The group owners are the reviewers and fallback reviewers are assigned.</span></span>
+ <span data-ttu-id="4a22d-199">它每季度的第三天重复发生，并无限期地继续。</span><span class="sxs-lookup"><span data-stu-id="4a22d-199">It recurs on the third day of every quarter and continues indefinitely.</span></span>
+ <span data-ttu-id="4a22d-200">**autoApplyDecisionsEnabled** 设置为 ，将 `true` **defaultDecision 设置为** `Deny` 。</span><span class="sxs-lookup"><span data-stu-id="4a22d-200">**autoApplyDecisionsEnabled** is set to `true` with the **defaultDecision** set to `Deny`.</span></span>

#### <a name="request"></a><span data-ttu-id="4a22d-201">请求</span><span class="sxs-lookup"><span data-stu-id="4a22d-201">Request</span></span>
<span data-ttu-id="4a22d-202">在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a22d-202">In the request body, supply a JSON representation of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a22d-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a22d-203">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition_inactiveguests_M365"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
Content-type: application/json

{
  "displayName": "Review inactive guests on teams",
  "descriptionForAdmins": "Control guest user access to our teams.",
  "descriptionForReviewers": "Information security is everyone's responsibility. Review our access policy for more.",
  "instanceEnumerationScope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team')')",
    "queryType": "MicrosoftGraph"
  },
  "scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
    },
  "reviewers": [
    {
      "query": "./owners",
      "queryType": "MicrosoftGraph"
    }
  ],
  "fallbackReviewers": [
    {
      "query": "/users/fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
      "queryType": "MicrosoftGraph"
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "recommendationsEnabled": true,
    "instanceDurationInDays": 3,
    "recurrence": {
      "pattern": {
        "type": "absoluteMonthly",
        "dayOfMonth": 5,
        "interval": 3
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-05-04T00:00:00.000Z"
      }
    },
    "defaultDecisionEnabled": true,
    "defaultDecision": "Deny",
    "autoApplyDecisionsEnabled": true
  }
}
```
# <a name="c"></a>[<span data-ttu-id="4a22d-204">C#</span><span class="sxs-lookup"><span data-stu-id="4a22d-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewscheduledefinition-inactiveguests-m365-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a22d-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a22d-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-inactiveguests-m365-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a22d-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a22d-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewscheduledefinition-inactiveguests-m365-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a22d-207">Java</span><span class="sxs-lookup"><span data-stu-id="4a22d-207">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewscheduledefinition-inactiveguests-m365-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4a22d-208">响应</span><span class="sxs-lookup"><span data-stu-id="4a22d-208">Response</span></span>
><span data-ttu-id="4a22d-209">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4a22d-209">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions/$entity",
  "id": "b0966e21-a01e-43c9-8f8b-9ba30ed5710a",
  "displayName": "Review inactive guests on teams",
  "createdDateTime": "2021-05-04T18:27:02.6719849Z",
  "lastModifiedDateTime": "2021-05-04T18:27:24.0889623Z",
  "status": "InProgress",
  "descriptionForAdmins": "Control guest user access to our teams.",
  "descriptionForReviewers": "Information security is everyone's responsibility. Review our access policy for more.",
  "createdBy": {
    "id": "fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
    "displayName": "MOD Administrator",
    "userPrincipalName": "admin@contoso.com"
  },
  "scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "queryRoot": null,
    "inactiveDuration": "P30D"
  },
  "instanceEnumerationScope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team'))&$count=true",
    "queryType": "MicrosoftGraph",
    "queryRoot": null
  },
  "reviewers": [
    {
      "query": "./owners",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ],
  "backupReviewers": [],
  "fallbackReviewers": [
    {
      "query": "/users/fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": true,
    "defaultDecision": "Deny",
    "instanceDurationInDays": 3,
    "autoApplyDecisionsEnabled": true,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "absoluteMonthly",
        "interval": 3,
        "month": 0,
        "dayOfMonth": 5,
        "daysOfWeek": [],
        "firstDayOfWeek": "sunday",
        "index": "first"
      },
      "range": {
        "type": "noEnd",
        "numberOfOccurrences": 0,
        "recurrenceTimeZone": null,
        "startDate": "2021-05-05",
        "endDate": null
      }
    },
    "applyActions": []
  }
}
```

### <a name="example-3-create-an-access-review-of-all-users-to-an-application"></a><span data-ttu-id="4a22d-210">示例 3：创建对应用程序的所有用户的访问评审</span><span class="sxs-lookup"><span data-stu-id="4a22d-210">Example 3: Create an access review of all users to an application</span></span>

<span data-ttu-id="4a22d-211">这是一个创建具有以下设置的访问评审的示例：</span><span class="sxs-lookup"><span data-stu-id="4a22d-211">This is an example of creating an access review with the following settings:</span></span>
+ <span data-ttu-id="4a22d-212">该评论将审核用户对应用程序的访问权限。</span><span class="sxs-lookup"><span data-stu-id="4a22d-212">The review reviews user access to an application.</span></span>
+ <span data-ttu-id="4a22d-213">人员经理是审阅者，回退审阅者是组的成员。</span><span class="sxs-lookup"><span data-stu-id="4a22d-213">The people managers are the reviewers and fallback reviewers are the members of a group.</span></span>
+ <span data-ttu-id="4a22d-214">它每半年重复一次，自 startDate 起 1 年后结束。</span><span class="sxs-lookup"><span data-stu-id="4a22d-214">It recurs semi-annually and ends 1 year from the startDate.</span></span>

#### <a name="request"></a><span data-ttu-id="4a22d-215">请求</span><span class="sxs-lookup"><span data-stu-id="4a22d-215">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4a22d-216">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a22d-216">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition_allusers_M365_AADRole"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
Content-type: application/json

{
  "displayName": "Review employee access to LinkedIn",
  "descriptionForAdmins": "Review employee access to LinkedIn",
  "scope": {
    "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
    "principalScopes": [
      {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/users",
        "queryType": "MicrosoftGraph"
      }
    ],
    "resourceScopes": [
      {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/servicePrincipals/bae11f90-7d5d-46ba-9f55-8112b59d92ae",
        "queryType": "MicrosoftGraph"
      }
    ]
  },
  "reviewers": [
    {
      "query": "./manager",
      "queryType": "MicrosoftGraph",
      "queryRoot": "decisions"
    }
  ],
  "backupReviewers": [
    {
      "query": "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
      "queryType": "MicrosoftGraph"
    }
  ],
  "fallbackReviewers": [
    {
      "query": "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
      "queryType": "MicrosoftGraph"
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": true,
    "defaultDecision": "Recommendation",
    "instanceDurationInDays": 180,
    "autoApplyDecisionsEnabled": true,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "absoluteMonthly",
        "interval": 6,
        "dayOfMonth": 0
      },
      "range": {
        "type": "numbered",
        "startDate": "2021-05-05",
        "endDate": "2022-05-05"
      }
    }
  }
}
```
# <a name="c"></a>[<span data-ttu-id="4a22d-217">C#</span><span class="sxs-lookup"><span data-stu-id="4a22d-217">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewscheduledefinition-allusers-m365-aadrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a22d-218">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a22d-218">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-allusers-m365-aadrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a22d-219">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a22d-219">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewscheduledefinition-allusers-m365-aadrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a22d-220">Java</span><span class="sxs-lookup"><span data-stu-id="4a22d-220">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewscheduledefinition-allusers-m365-aadrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4a22d-221">响应</span><span class="sxs-lookup"><span data-stu-id="4a22d-221">Response</span></span>
><span data-ttu-id="4a22d-222">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4a22d-222">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions/$entity",
  "id": "1f79f34b-8667-40d9-875c-893b630b3dec",
  "scope": {
    "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
    "principalScopes": [
      {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/users",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
      }
    ],
    "resourceScopes": [
      {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/servicePrincipals/bae11f90-7d5d-46ba-9f55-8112b59d92ae",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
      }
    ]
  },
  "reviewers": [
    {
      "query": "./manager",
      "queryType": "MicrosoftGraph",
      "queryRoot": "decisions"
    }
  ],
  "backupReviewers": [
    {
      "query": "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ],
  "fallbackReviewers": [
    {
      "query": "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ],
  "settings": {
    "instanceDurationInDays": 180,
    "recurrence": {
      "pattern": {
        "type": "absoluteMonthly",
        "interval": 6,
        "month": 0,
        "dayOfMonth": 0,
        "daysOfWeek": [],
        "firstDayOfWeek": "sunday",
        "index": "first"
      },
      "range": {
        "type": "numbered",
        "numberOfOccurrences": 0,
        "recurrenceTimeZone": null,
        "startDate": "2021-05-05",
        "endDate": "2022-05-05"
      }
    }
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
