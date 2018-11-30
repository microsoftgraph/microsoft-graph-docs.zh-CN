---
title: 创建 accessReview
description: Azure AD 中访问审阅功能，创建一个新的 accessReview 对象。
ms.openlocfilehash: 9d8e8b246c3c43e4f69172ea59715a8718d39d1e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042039"
---
# <a name="create-accessreview"></a><span data-ttu-id="c094c-103">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="c094c-103">Create accessReview</span></span>

> <span data-ttu-id="c094c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c094c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c094c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c094c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c094c-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中创建新的[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c094c-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="c094c-107">进行此请求之前, 将呼叫者必须具有之前[检索业务流程模板列表中的](businessflowtemplate-list.md)，具有的值`businessFlowTemplateId`要包含在请求中。</span><span class="sxs-lookup"><span data-stu-id="c094c-107">Prior to making this request, the caller must have previously [retrieved the list of business flow templates](businessflowtemplate-list.md), to have the value of `businessFlowTemplateId` to include in the request.</span></span>

<span data-ttu-id="c094c-108">进行此请求之后, 将呼叫者应[创建 programControl](programcontrol-create.md)，若要访问评审链接到的程序。</span><span class="sxs-lookup"><span data-stu-id="c094c-108">After making this request, the caller should [create a programControl](programcontrol-create.md), to link the access review to a program.</span></span>  

## <a name="permissions"></a><span data-ttu-id="c094c-109">权限</span><span class="sxs-lookup"><span data-stu-id="c094c-109">Permissions</span></span>
<span data-ttu-id="c094c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c094c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c094c-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c094c-112">Permission type</span></span>                        | <span data-ttu-id="c094c-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c094c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c094c-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c094c-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c094c-115">AccessReview.ReadWrite.All，也应具有完成后续呼叫中以创建 programControl 方案的 ProgramControl.ReadWrite.All 和</span><span class="sxs-lookup"><span data-stu-id="c094c-115">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with the subsequent call to create a programControl</span></span> |
|<span data-ttu-id="c094c-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c094c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c094c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c094c-117">Not supported.</span></span> |
|<span data-ttu-id="c094c-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="c094c-118">Application</span></span>                            | <span data-ttu-id="c094c-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c094c-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c094c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c094c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a><span data-ttu-id="c094c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c094c-121">Request headers</span></span>
| <span data-ttu-id="c094c-122">名称</span><span class="sxs-lookup"><span data-stu-id="c094c-122">Name</span></span>         | <span data-ttu-id="c094c-123">类型</span><span class="sxs-lookup"><span data-stu-id="c094c-123">Type</span></span>        | <span data-ttu-id="c094c-124">说明</span><span class="sxs-lookup"><span data-stu-id="c094c-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c094c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c094c-125">Authorization</span></span> | <span data-ttu-id="c094c-126">string</span><span class="sxs-lookup"><span data-stu-id="c094c-126">string</span></span> | <span data-ttu-id="c094c-127">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="c094c-127">Bearer \{token\}.</span></span> <span data-ttu-id="c094c-128">必需。</span><span class="sxs-lookup"><span data-stu-id="c094c-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c094c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c094c-129">Request body</span></span>
<span data-ttu-id="c094c-130">在请求正文中，提供[accessReview](../resources/accessreview.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c094c-130">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="c094c-131">下表显示时创建 accessReview 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c094c-131">The following table shows the properties that are required when you create an accessReview.</span></span>

| <span data-ttu-id="c094c-132">属性</span><span class="sxs-lookup"><span data-stu-id="c094c-132">Property</span></span>     | <span data-ttu-id="c094c-133">类型</span><span class="sxs-lookup"><span data-stu-id="c094c-133">Type</span></span>        | <span data-ttu-id="c094c-134">说明</span><span class="sxs-lookup"><span data-stu-id="c094c-134">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="c094c-135">访问审阅名称。</span><span class="sxs-lookup"><span data-stu-id="c094c-135">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="c094c-136">审阅安排在启动时 DateTime。</span><span class="sxs-lookup"><span data-stu-id="c094c-136">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="c094c-137">这必须是在将来的日期。</span><span class="sxs-lookup"><span data-stu-id="c094c-137">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="c094c-138">审阅安排结束时 DateTime。</span><span class="sxs-lookup"><span data-stu-id="c094c-138">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="c094c-139">这必须是至少一个日期晚于开始日期。</span><span class="sxs-lookup"><span data-stu-id="c094c-139">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="c094c-140">说明，向审阅者显示。</span><span class="sxs-lookup"><span data-stu-id="c094c-140">The description, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="c094c-141">业务流程模板标识符，从[businessFlowTemplate](../resources/businessflowtemplate.md)获得。</span><span class="sxs-lookup"><span data-stu-id="c094c-141">The business flow template identifier, obtained from a [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span>  |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="c094c-142">审阅者已审阅对象之一的访问权限的关系类型`self`，`delegate`或`entityOwners`。</span><span class="sxs-lookup"><span data-stu-id="c094c-142">The relationship type of reviewer to the access rights of the reviewed object, one of `self`, `delegate` or `entityOwners`.</span></span> | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="c094c-143">为其访问审阅创建对象，如组的成员身份或向应用程序的用户的分配。</span><span class="sxs-lookup"><span data-stu-id="c094c-143">The object for which an access review is created, such as a memberships of an group or the assignments of users to an application.</span></span> | 


<span data-ttu-id="c094c-144">如果要提供 reviewerType 具有值`delegate`，然后将呼叫者还必须包括`reviewers`属性，与[userIdentity](../resources/useridentity.md)审阅者的集合。</span><span class="sxs-lookup"><span data-stu-id="c094c-144">If the reviewerType being supplied has the value `delegate`, then the caller must also include the `reviewers` property, with a collection of [userIdentity](../resources/useridentity.md) of the reviewers.</span></span>

<span data-ttu-id="c094c-145">此外，呼叫者可以包括设置，以创建定期查看系列或更改默认查看行为。</span><span class="sxs-lookup"><span data-stu-id="c094c-145">In addition, the caller can include settings, to create a recurring review series or to change from the default review behavior.</span></span> <span data-ttu-id="c094c-146">具体而言，若要创建定期查看，呼叫者必须包括`accessReviewRecurrenceSettings`中访问检查设置，</span><span class="sxs-lookup"><span data-stu-id="c094c-146">In particular, to create a recurring review, the caller must include the `accessReviewRecurrenceSettings` within the access review settings,</span></span>


## <a name="response"></a><span data-ttu-id="c094c-147">响应</span><span class="sxs-lookup"><span data-stu-id="c094c-147">Response</span></span>
<span data-ttu-id="c094c-148">如果成功，此方法返回`201, Created`响应代码和响应正文中的[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c094c-148">If successful, this method returns a `201, Created` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c094c-149">示例</span><span class="sxs-lookup"><span data-stu-id="c094c-149">Example</span></span>

<span data-ttu-id="c094c-150">这是创建一次性 （而不是定期） 访问回顾，显式指定为审阅者的两个用户的一个示例。</span><span class="sxs-lookup"><span data-stu-id="c094c-150">This is an example of creating a one-time (not recurring) access review, explicitly specifying two users as the reviewers.</span></span>

##### <a name="request"></a><span data-ttu-id="c094c-151">请求</span><span class="sxs-lookup"><span data-stu-id="c094c-151">Request</span></span>
<span data-ttu-id="c094c-152">在请求正文中，提供[accessReview](../resources/accessreview.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c094c-152">In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.</span></span>

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
    "reviewerType" : "delegate",
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
        "justificationRequiredOnApproval": true,
        "activityHistoryInDays":30,
        "mailNotificationsEnabled":true,
        "remindersEnabled":true
    }
}
```

##### <a name="response"></a><span data-ttu-id="c094c-153">响应</span><span class="sxs-lookup"><span data-stu-id="c094c-153">Response</span></span>
><span data-ttu-id="c094c-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c094c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "reviewerType": "delegate",
    "description": "Sample description"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
