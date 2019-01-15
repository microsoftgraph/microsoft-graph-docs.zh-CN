---
title: 更新 accessReview
description: 在 Azure AD 访问评论功能中，更新现有 accessReview 对象更改一个或多个其属性。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e4e74daa092c6f18c845c7f0c468af90385b899b
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016749"
---
# <a name="update-accessreview"></a><span data-ttu-id="b08ab-103">更新 accessReview</span><span class="sxs-lookup"><span data-stu-id="b08ab-103">Update accessReview</span></span>

> <span data-ttu-id="b08ab-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b08ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b08ab-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b08ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b08ab-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，更新现有[accessReview](../resources/accessreview.md)对象更改一个或多个其属性。</span><span class="sxs-lookup"><span data-stu-id="b08ab-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="b08ab-107">此 API 不是要更改的审阅者或评审的决策。</span><span class="sxs-lookup"><span data-stu-id="b08ab-107">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="b08ab-108">若要更改审阅者，请使用[addReviewer](accessreview-addreviewer.md)或[removeReviewer](accessreview-removereviewer.md) Api。</span><span class="sxs-lookup"><span data-stu-id="b08ab-108">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="b08ab-109">若要停止已启动一次性审阅中或已启动的定期查看实例，早期，使用[停止](accessreview-stop.md)API。</span><span class="sxs-lookup"><span data-stu-id="b08ab-109">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="b08ab-110">若要应用到目标组或应用程序的访问权限的决策，使用[应用](accessreview-apply.md)API。</span><span class="sxs-lookup"><span data-stu-id="b08ab-110">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="b08ab-111">权限</span><span class="sxs-lookup"><span data-stu-id="b08ab-111">Permissions</span></span>
<span data-ttu-id="b08ab-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b08ab-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b08ab-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="b08ab-114">Permission type</span></span>                        | <span data-ttu-id="b08ab-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b08ab-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b08ab-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b08ab-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="b08ab-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b08ab-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="b08ab-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b08ab-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b08ab-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="b08ab-119">Not supported.</span></span> |
|<span data-ttu-id="b08ab-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="b08ab-120">Application</span></span>                            | <span data-ttu-id="b08ab-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="b08ab-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b08ab-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b08ab-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="b08ab-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b08ab-123">Request headers</span></span>
| <span data-ttu-id="b08ab-124">名称</span><span class="sxs-lookup"><span data-stu-id="b08ab-124">Name</span></span>         | <span data-ttu-id="b08ab-125">类型</span><span class="sxs-lookup"><span data-stu-id="b08ab-125">Type</span></span>        | <span data-ttu-id="b08ab-126">说明</span><span class="sxs-lookup"><span data-stu-id="b08ab-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b08ab-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b08ab-127">Authorization</span></span> | <span data-ttu-id="b08ab-128">string</span><span class="sxs-lookup"><span data-stu-id="b08ab-128">string</span></span> | <span data-ttu-id="b08ab-129">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="b08ab-129">Bearer \{token\}.</span></span> <span data-ttu-id="b08ab-130">必需。</span><span class="sxs-lookup"><span data-stu-id="b08ab-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b08ab-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="b08ab-131">Request body</span></span>
<span data-ttu-id="b08ab-132">在请求正文中，提供[accessReview](../resources/accessreview.md)对象的参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b08ab-132">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="b08ab-133">下表显示可更新 accessReview 时提供的属性。</span><span class="sxs-lookup"><span data-stu-id="b08ab-133">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="b08ab-134">属性</span><span class="sxs-lookup"><span data-stu-id="b08ab-134">Property</span></span>     | <span data-ttu-id="b08ab-135">类型</span><span class="sxs-lookup"><span data-stu-id="b08ab-135">Type</span></span>        | <span data-ttu-id="b08ab-136">说明</span><span class="sxs-lookup"><span data-stu-id="b08ab-136">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="b08ab-137">访问审阅名称。</span><span class="sxs-lookup"><span data-stu-id="b08ab-137">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="b08ab-138">审阅安排在启动时 DateTime。</span><span class="sxs-lookup"><span data-stu-id="b08ab-138">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="b08ab-139">这必须是在将来的日期。</span><span class="sxs-lookup"><span data-stu-id="b08ab-139">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="b08ab-140">审阅安排结束时 DateTime。</span><span class="sxs-lookup"><span data-stu-id="b08ab-140">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="b08ab-141">这必须是至少一个日期晚于开始日期。</span><span class="sxs-lookup"><span data-stu-id="b08ab-141">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="b08ab-142">说明，向审阅者显示。</span><span class="sxs-lookup"><span data-stu-id="b08ab-142">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="b08ab-143">响应</span><span class="sxs-lookup"><span data-stu-id="b08ab-143">Response</span></span>
<span data-ttu-id="b08ab-144">如果成功，此方法返回`204, Accepted`响应代码和响应正文中的[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b08ab-144">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b08ab-145">示例</span><span class="sxs-lookup"><span data-stu-id="b08ab-145">Example</span></span>

<span data-ttu-id="b08ab-146">这是一次性的 （不) 访问审阅更新的示例。</span><span class="sxs-lookup"><span data-stu-id="b08ab-146">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="b08ab-147">请求</span><span class="sxs-lookup"><span data-stu-id="b08ab-147">Request</span></span>
<span data-ttu-id="b08ab-148">在请求正文中，提供[accessReview](../resources/accessreview.md)对象的新属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b08ab-148">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews('006111db-0810-4494-a6df-904d368bd81b')
Content-type: application/json

{
    "displayName":"TestReview new name"
}
```

##### <a name="response"></a><span data-ttu-id="b08ab-149">响应</span><span class="sxs-lookup"><span data-stu-id="b08ab-149">Response</span></span>
><span data-ttu-id="b08ab-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b08ab-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview new name",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
