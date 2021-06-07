---
title: 创建 accessReview
description: 在 Azure AD 访问评审功能中，创建新的 accessReview 对象。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: fd1f6c25dcc4013c1abc3d39dafa63723a1e3ea0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751116"
---
# <a name="create-accessreview"></a><span data-ttu-id="797ef-103">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="797ef-103">Create accessReview</span></span>

<span data-ttu-id="797ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="797ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="797ef-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，创建新的 [accessReview](../resources/accessreview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="797ef-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="797ef-106">进行此请求之前，调用方之前必须已检索 [](businessflowtemplate-list.md)到业务流模板的列表，才能将 **businessFlowTemplateId** 的值包括在请求中。</span><span class="sxs-lookup"><span data-stu-id="797ef-106">Before making this request, the caller must have previously [retrieved the list of business flow templates](businessflowtemplate-list.md), to have the value of **businessFlowTemplateId** to include in the request.</span></span>

<span data-ttu-id="797ef-107">提出此请求后，调用方应 [创建 programControl，](programcontrol-create.md)以将访问评审链接到程序。</span><span class="sxs-lookup"><span data-stu-id="797ef-107">After making this request, the caller should [create a programControl](programcontrol-create.md), to link the access review to a program.</span></span>  

## <a name="permissions"></a><span data-ttu-id="797ef-108">权限</span><span class="sxs-lookup"><span data-stu-id="797ef-108">Permissions</span></span>

<span data-ttu-id="797ef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="797ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="797ef-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="797ef-111">Permission type</span></span>                        | <span data-ttu-id="797ef-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="797ef-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="797ef-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="797ef-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="797ef-114">AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="797ef-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="797ef-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="797ef-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="797ef-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="797ef-116">Not supported.</span></span> |
|<span data-ttu-id="797ef-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="797ef-117">Application</span></span>                            | <span data-ttu-id="797ef-118">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="797ef-118">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="797ef-119">调用方还应具有 ProgramControl.ReadWrite.All 权限，以便创建访问评审后，调用方可以创建 [programControl](../resources/programcontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="797ef-119">The caller should also have ProgramControl.ReadWrite.All permission, so that after creating an access review, the caller can create a [programControl](../resources/programcontrol.md).</span></span>
<span data-ttu-id="797ef-120">此外，登录用户还必须具有允许其创建访问评审的目录角色。</span><span class="sxs-lookup"><span data-stu-id="797ef-120">In addition, the signed in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="797ef-121">有关详细信息，请参阅访问评审的角色和 [权限要求](../resources/accessreviews-root.md)。</span><span class="sxs-lookup"><span data-stu-id="797ef-121">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="797ef-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="797ef-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a><span data-ttu-id="797ef-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="797ef-123">Request headers</span></span>
| <span data-ttu-id="797ef-124">名称</span><span class="sxs-lookup"><span data-stu-id="797ef-124">Name</span></span>         | <span data-ttu-id="797ef-125">说明</span><span class="sxs-lookup"><span data-stu-id="797ef-125">Description</span></span> |
|:-------------|:------------|
| <span data-ttu-id="797ef-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="797ef-126">Authorization</span></span> | <span data-ttu-id="797ef-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="797ef-p103">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="797ef-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="797ef-129">Content-type</span></span> | <span data-ttu-id="797ef-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="797ef-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="797ef-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="797ef-132">Request body</span></span>
<span data-ttu-id="797ef-133">在请求正文中，提供 [accessReview](../resources/accessreview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="797ef-133">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="797ef-134">下表显示创建 accessReview 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="797ef-134">The following table shows the properties that are required when you create an accessReview.</span></span>

| <span data-ttu-id="797ef-135">属性</span><span class="sxs-lookup"><span data-stu-id="797ef-135">Property</span></span>     | <span data-ttu-id="797ef-136">类型</span><span class="sxs-lookup"><span data-stu-id="797ef-136">Type</span></span>        | <span data-ttu-id="797ef-137">说明</span><span class="sxs-lookup"><span data-stu-id="797ef-137">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="797ef-138">displayName</span><span class="sxs-lookup"><span data-stu-id="797ef-138">displayName</span></span>             |<span data-ttu-id="797ef-139">String</span><span class="sxs-lookup"><span data-stu-id="797ef-139">String</span></span>                                                        | <span data-ttu-id="797ef-140">访问评审名称。</span><span class="sxs-lookup"><span data-stu-id="797ef-140">The access review name.</span></span>  |
| <span data-ttu-id="797ef-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="797ef-141">startDateTime</span></span>           |<span data-ttu-id="797ef-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="797ef-142">DateTimeOffset</span></span>                                                | <span data-ttu-id="797ef-143">计划开始审阅的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="797ef-143">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="797ef-144">这必须是将来的日期。</span><span class="sxs-lookup"><span data-stu-id="797ef-144">This must be a date in the future.</span></span>   |
| <span data-ttu-id="797ef-145">endDateTime</span><span class="sxs-lookup"><span data-stu-id="797ef-145">endDateTime</span></span>             |<span data-ttu-id="797ef-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="797ef-146">DateTimeOffset</span></span>                                                | <span data-ttu-id="797ef-147">计划结束审阅的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="797ef-147">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="797ef-148">这必须至少比开始日期晚一天。</span><span class="sxs-lookup"><span data-stu-id="797ef-148">This must be at least one day later than the start date.</span></span>   |
| <span data-ttu-id="797ef-149">说明</span><span class="sxs-lookup"><span data-stu-id="797ef-149">description</span></span>             |<span data-ttu-id="797ef-150">String</span><span class="sxs-lookup"><span data-stu-id="797ef-150">String</span></span>                                                        | <span data-ttu-id="797ef-151">向审阅者显示的说明。</span><span class="sxs-lookup"><span data-stu-id="797ef-151">The description, to show to the reviewers.</span></span> |
| <span data-ttu-id="797ef-152">businessFlowTemplateId</span><span class="sxs-lookup"><span data-stu-id="797ef-152">businessFlowTemplateId</span></span>  |<span data-ttu-id="797ef-153">String</span><span class="sxs-lookup"><span data-stu-id="797ef-153">String</span></span>                                                        | <span data-ttu-id="797ef-154">从 [businessFlowTemplate](../resources/businessflowtemplate.md)获取的业务流程模板标识符。</span><span class="sxs-lookup"><span data-stu-id="797ef-154">The business flow template identifier, obtained from a [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span>  |
| <span data-ttu-id="797ef-155">reviewerType</span><span class="sxs-lookup"><span data-stu-id="797ef-155">reviewerType</span></span>            |<span data-ttu-id="797ef-156">String</span><span class="sxs-lookup"><span data-stu-id="797ef-156">String</span></span>                                                        | <span data-ttu-id="797ef-157">审阅者对被审阅对象的访问权的关系类型，如 、 或 `self` `delegated` `entityOwners` 。</span><span class="sxs-lookup"><span data-stu-id="797ef-157">The relationship type of reviewer to the access rights of the reviewed object, one of `self`, `delegated`, or `entityOwners`.</span></span> | 
| <span data-ttu-id="797ef-158">reviewedEntity</span><span class="sxs-lookup"><span data-stu-id="797ef-158">reviewedEntity</span></span>          |[<span data-ttu-id="797ef-159">identity</span><span class="sxs-lookup"><span data-stu-id="797ef-159">identity</span></span>](../resources/identity.md)                                     | <span data-ttu-id="797ef-160">创建访问评审的对象，例如组的成员身份或用户到应用程序的分配。</span><span class="sxs-lookup"><span data-stu-id="797ef-160">The object for which an access review is created, such as the membership of a group or the assignments of users to an application.</span></span> | 


<span data-ttu-id="797ef-161">如果 **reviewerType** 具有值，则调用方还必须包含 `delegated` **reviewers** 属性，其中 [userIdentity](../resources/useridentity.md) 对象集合代表审阅者。</span><span class="sxs-lookup"><span data-stu-id="797ef-161">If the **reviewerType** has the value `delegated`, then the caller must also include the **reviewers** property, with a collection of [userIdentity](../resources/useridentity.md) objects representing the reviewers.</span></span>

<span data-ttu-id="797ef-162">如果你的应用在没有登录用户的情况下调用此 API，则调用方还必须包含 **createdBy** 属性，其值为将被标识为评价创建者的用户的 [userIdentity。](../resources/useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="797ef-162">If your app is calling this API without a signed-in user, then the caller must also include the **createdBy** property, the value for which is a [userIdentity](../resources/useridentity.md) of the user who will be identified as the creator of the review.</span></span>

<span data-ttu-id="797ef-163">此外，呼叫者可以包含 **设置**，以创建定期审阅系列或更改默认审阅行为。</span><span class="sxs-lookup"><span data-stu-id="797ef-163">In addition, the caller can include **settings**, to create a recurring review series or to change from the default review behavior.</span></span> <span data-ttu-id="797ef-164">具体而言，若要创建定期审阅，呼叫者必须在访问评审设置中包括[accessReviewRecurrenceSettings，](../resources/accessreviewrecurrencesettings.md)</span><span class="sxs-lookup"><span data-stu-id="797ef-164">In particular, to create a recurring review, the caller must include the [accessReviewRecurrenceSettings](../resources/accessreviewrecurrencesettings.md) within the access review settings,</span></span>


## <a name="response"></a><span data-ttu-id="797ef-165">响应</span><span class="sxs-lookup"><span data-stu-id="797ef-165">Response</span></span>
<span data-ttu-id="797ef-166">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [accessReview](../resources/accessreview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="797ef-166">If successful, this method returns a `201 Created` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="797ef-167">示例</span><span class="sxs-lookup"><span data-stu-id="797ef-167">Example</span></span>

<span data-ttu-id="797ef-168">这是一个创建一次性网站，而不是 (访问) ，明确指定两个用户作为审阅者的示例。</span><span class="sxs-lookup"><span data-stu-id="797ef-168">This is an example of creating a one-time (not recurring) access review, explicitly specifying two users as the reviewers.</span></span>

### <a name="request"></a><span data-ttu-id="797ef-169">请求</span><span class="sxs-lookup"><span data-stu-id="797ef-169">Request</span></span>
<span data-ttu-id="797ef-170">在请求正文中，提供 [accessReview](../resources/accessreview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="797ef-170">In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="797ef-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="797ef-171">HTTP</span></span>](#tab/http)
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
        "id": "99025615-a0b1-47ec-9117-35377b10998b"
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
# <a name="c"></a>[<span data-ttu-id="797ef-172">C#</span><span class="sxs-lookup"><span data-stu-id="797ef-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreview-from-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="797ef-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="797ef-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreview-from-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="797ef-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="797ef-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreview-from-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="797ef-175">Java</span><span class="sxs-lookup"><span data-stu-id="797ef-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreview-from-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="797ef-176">响应</span><span class="sxs-lookup"><span data-stu-id="797ef-176">Response</span></span>
><span data-ttu-id="797ef-177">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="797ef-177">**Note:** The response object shown here might be shortened for readability.</span></span>
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


