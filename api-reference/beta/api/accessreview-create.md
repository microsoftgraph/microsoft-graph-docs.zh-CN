---
title: 创建 accessReview
description: 在 "Azure AD access 评论" 功能中, 创建一个新的 accessReview 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0fe636c531ba4a9b82c44427002937876c8e4178
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172773"
---
# <a name="create-accessreview"></a><span data-ttu-id="c5996-103">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="c5996-103">Create accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5996-104">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 创建一个新的[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c5996-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="c5996-105">在发出此请求之前, 呼叫者必须先[检索业务流模板列表](businessflowtemplate-list.md), 才能将值`businessFlowTemplateId`包含在请求中。</span><span class="sxs-lookup"><span data-stu-id="c5996-105">Before making this request, the caller must have previously [retrieved the list of business flow templates](businessflowtemplate-list.md), to have the value of `businessFlowTemplateId` to include in the request.</span></span>

<span data-ttu-id="c5996-106">发出此请求后, 调用方应[创建一个 programControl](programcontrol-create.md), 以将访问审核链接到某个程序。</span><span class="sxs-lookup"><span data-stu-id="c5996-106">After making this request, the caller should [create a programControl](programcontrol-create.md), to link the access review to a program.</span></span>  

## <a name="permissions"></a><span data-ttu-id="c5996-107">权限</span><span class="sxs-lookup"><span data-stu-id="c5996-107">Permissions</span></span>
<span data-ttu-id="c5996-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5996-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5996-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5996-110">Permission type</span></span>                        | <span data-ttu-id="c5996-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5996-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5996-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5996-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5996-113">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="c5996-113">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="c5996-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5996-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5996-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5996-115">Not supported.</span></span> |
|<span data-ttu-id="c5996-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5996-116">Application</span></span>                            | <span data-ttu-id="c5996-117">AccessReview 的成员资格</span><span class="sxs-lookup"><span data-stu-id="c5996-117">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="c5996-118">调用方还应具有 ProgramControl 权限, 以便在创建访问审核之后, 调用方可以创建[ProgramControl](../resources/programcontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="c5996-118">The caller should also have ProgramControl.ReadWrite.All permission, so that after creating an access review, the caller can create a [programControl](../resources/programcontrol.md).</span></span>
<span data-ttu-id="c5996-119">此外, 登录用户还必须位于允许他们创建访问审阅的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="c5996-119">In addition, the signed in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="c5996-120">有关更多详细信息, 请参阅[access 评审](../resources/accessreviews-root.md)的角色和权限要求。</span><span class="sxs-lookup"><span data-stu-id="c5996-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="c5996-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5996-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a><span data-ttu-id="c5996-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5996-122">Request headers</span></span>
| <span data-ttu-id="c5996-123">名称</span><span class="sxs-lookup"><span data-stu-id="c5996-123">Name</span></span>         | <span data-ttu-id="c5996-124">类型</span><span class="sxs-lookup"><span data-stu-id="c5996-124">Type</span></span>        | <span data-ttu-id="c5996-125">说明</span><span class="sxs-lookup"><span data-stu-id="c5996-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c5996-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5996-126">Authorization</span></span> | <span data-ttu-id="c5996-127">string</span><span class="sxs-lookup"><span data-stu-id="c5996-127">string</span></span> | <span data-ttu-id="c5996-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5996-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5996-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5996-130">Request body</span></span>
<span data-ttu-id="c5996-131">在请求正文中, 提供[accessReview](../resources/accessreview.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5996-131">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="c5996-132">下表显示创建 accessReview 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c5996-132">The following table shows the properties that are required when you create an accessReview.</span></span>

| <span data-ttu-id="c5996-133">属性</span><span class="sxs-lookup"><span data-stu-id="c5996-133">Property</span></span>     | <span data-ttu-id="c5996-134">类型</span><span class="sxs-lookup"><span data-stu-id="c5996-134">Type</span></span>        | <span data-ttu-id="c5996-135">说明</span><span class="sxs-lookup"><span data-stu-id="c5996-135">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="c5996-136">访问审阅名称。</span><span class="sxs-lookup"><span data-stu-id="c5996-136">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="c5996-137">计划开始评审时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="c5996-137">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="c5996-138">这必须是将来的日期。</span><span class="sxs-lookup"><span data-stu-id="c5996-138">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="c5996-139">计划结束评审时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c5996-139">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="c5996-140">此时间必须至少为一个晚于开始日期的一天。</span><span class="sxs-lookup"><span data-stu-id="c5996-140">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="c5996-141">要向审阅者显示的说明。</span><span class="sxs-lookup"><span data-stu-id="c5996-141">The description, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="c5996-142">从[businessFlowTemplate](../resources/businessflowtemplate.md)获取的业务流模板标识符。</span><span class="sxs-lookup"><span data-stu-id="c5996-142">The business flow template identifier, obtained from a [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span>  |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="c5996-143">审阅者的关系类型: 审阅的对象的访问权限、 `self` `delegated`、或。 `entityOwners`</span><span class="sxs-lookup"><span data-stu-id="c5996-143">The relationship type of reviewer to the access rights of the reviewed object, one of `self`, `delegated`, or `entityOwners`.</span></span> | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="c5996-144">为其创建访问审核的对象, 例如组的成员身份或向应用程序分配的用户。</span><span class="sxs-lookup"><span data-stu-id="c5996-144">The object for which an access review is created, such as the membership of a group or the assignments of users to an application.</span></span> | 


<span data-ttu-id="c5996-145">如果要提供的 reviewerType 具有值`delegated`, 则调用方还必须包括该`reviewers`属性, 其中包含审阅人的[userIdentity](../resources/useridentity.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="c5996-145">If the reviewerType being supplied has the value `delegated`, then the caller must also include the `reviewers` property, with a collection of [userIdentity](../resources/useridentity.md) of the reviewers.</span></span>

<span data-ttu-id="c5996-146">如果您的应用程序在没有登录用户的情况下调用此 API, 则呼叫者还必须包含**createdBy**属性, 其值是将被标识为审阅的创建者的用户的[userIdentity](../resources/useridentity.md) 。</span><span class="sxs-lookup"><span data-stu-id="c5996-146">If your app is calling this API without a signed-in user, then the caller must also include the **createdBy** property, the value for which is a [userIdentity](../resources/useridentity.md) of the user who will be identified as the creator of the review.</span></span>

<span data-ttu-id="c5996-147">此外, 呼叫者还可以包括设置、创建定期审阅系列或从默认的审阅行为更改。</span><span class="sxs-lookup"><span data-stu-id="c5996-147">In addition, the caller can include settings, to create a recurring review series or to change from the default review behavior.</span></span> <span data-ttu-id="c5996-148">特别是, 若要创建定期检查, 呼叫者必须在 " `accessReviewRecurrenceSettings`访问审核设置" 中包含 "",</span><span class="sxs-lookup"><span data-stu-id="c5996-148">In particular, to create a recurring review, the caller must include the `accessReviewRecurrenceSettings` within the access review settings,</span></span>


## <a name="response"></a><span data-ttu-id="c5996-149">响应</span><span class="sxs-lookup"><span data-stu-id="c5996-149">Response</span></span>
<span data-ttu-id="c5996-150">如果成功, 此方法在响应`201, Created`正文中返回响应代码和[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c5996-150">If successful, this method returns a `201, Created` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5996-151">示例</span><span class="sxs-lookup"><span data-stu-id="c5996-151">Example</span></span>

<span data-ttu-id="c5996-152">下面的示例演示了如何创建一次性 (非定期) 访问审核, 并将两个用户显式指定为审阅者。</span><span class="sxs-lookup"><span data-stu-id="c5996-152">This is an example of creating a one-time (not recurring) access review, explicitly specifying two users as the reviewers.</span></span>

##### <a name="request"></a><span data-ttu-id="c5996-153">请求</span><span class="sxs-lookup"><span data-stu-id="c5996-153">Request</span></span>
<span data-ttu-id="c5996-154">在请求正文中, 提供[accessReview](../resources/accessreview.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5996-154">In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c5996-155">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c5996-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReview_from_accessReviews"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews
Content-type: application/json

{
    "displayName":"TestReview",
    "startDateTime":"2017-02-10T00:35:53.214Z",
    "endDateTime":"2017-03-12T00:35:53.214Z",
    "reviewedEntity": {
        "id": "99025615-a0b1-47ec-9117-35377b10998b",
    },
    "reviewerType" : "delegated",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "description":"Sample description",
    "reviewers":
    [
        {
            "id":"f260246a-09b1-4fd5-8d18-daed736071ec"
        },
        {
            "id":"5a4e184c-4ee5-4883-96e9-b371f8da88e3"
        }
    ],
    "settings":
    {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval":true,
        "autoReviewEnabled":false,
        "activityDurationInDays":30,
        "autoApplyReviewResultsEnabled":false,
        "accessRecommendationsEnabled":false,
        "recurrenceSettings":{
            "recurrenceType":"onetime",
            "recurrenceEndType":"endBy",
            "durationInDays":0,
            "recurrenceCount":0
        },
        "autoReviewSettings":{
            "notReviewedResult":"Deny"
        }
    }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c5996-156">C#</span><span class="sxs-lookup"><span data-stu-id="c5996-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreview-from-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c5996-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="c5996-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreview-from-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c5996-158">目标-C</span><span class="sxs-lookup"><span data-stu-id="c5996-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreview-from-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c5996-159">Java</span><span class="sxs-lookup"><span data-stu-id="c5996-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreview-from-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c5996-160">响应</span><span class="sxs-lookup"><span data-stu-id="c5996-160">Response</span></span>
><span data-ttu-id="c5996-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c5996-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
