---
title: 更新 accessReview
description: 在 Azure AD 访问评论功能中，更新现有 accessReview 对象更改一个或多个其属性。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1256ccdabea8eb5c0c0ffb3365e0c87276999236
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524364"
---
# <a name="update-accessreview"></a><span data-ttu-id="0bca4-103">更新 accessReview</span><span class="sxs-lookup"><span data-stu-id="0bca4-103">Update accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bca4-104">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，更新现有[accessReview](../resources/accessreview.md)对象更改一个或多个其属性。</span><span class="sxs-lookup"><span data-stu-id="0bca4-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="0bca4-105">此 API 不是要更改的审阅者或评审的决策。</span><span class="sxs-lookup"><span data-stu-id="0bca4-105">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="0bca4-106">若要更改审阅者，请使用[addReviewer](accessreview-addreviewer.md)或[removeReviewer](accessreview-removereviewer.md) Api。</span><span class="sxs-lookup"><span data-stu-id="0bca4-106">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="0bca4-107">若要停止已启动一次性审阅中或已启动的定期查看实例，早期，使用[停止](accessreview-stop.md)API。</span><span class="sxs-lookup"><span data-stu-id="0bca4-107">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="0bca4-108">若要应用到目标组或应用程序的访问权限的决策，使用[应用](accessreview-apply.md)API。</span><span class="sxs-lookup"><span data-stu-id="0bca4-108">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="0bca4-109">权限</span><span class="sxs-lookup"><span data-stu-id="0bca4-109">Permissions</span></span>
<span data-ttu-id="0bca4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0bca4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bca4-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="0bca4-112">Permission type</span></span>                        | <span data-ttu-id="0bca4-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0bca4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bca4-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0bca4-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="0bca4-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bca4-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="0bca4-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0bca4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bca4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0bca4-117">Not supported.</span></span> |
|<span data-ttu-id="0bca4-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="0bca4-118">Application</span></span>                            | <span data-ttu-id="0bca4-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="0bca4-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bca4-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0bca4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="0bca4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0bca4-121">Request headers</span></span>
| <span data-ttu-id="0bca4-122">名称</span><span class="sxs-lookup"><span data-stu-id="0bca4-122">Name</span></span>         | <span data-ttu-id="0bca4-123">类型</span><span class="sxs-lookup"><span data-stu-id="0bca4-123">Type</span></span>        | <span data-ttu-id="0bca4-124">说明</span><span class="sxs-lookup"><span data-stu-id="0bca4-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0bca4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bca4-125">Authorization</span></span> | <span data-ttu-id="0bca4-126">string</span><span class="sxs-lookup"><span data-stu-id="0bca4-126">string</span></span> | <span data-ttu-id="0bca4-127">持有者令牌</span><span class="sxs-lookup"><span data-stu-id="0bca4-127">Bearer \{token\}.</span></span> <span data-ttu-id="0bca4-128">必需。</span><span class="sxs-lookup"><span data-stu-id="0bca4-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0bca4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0bca4-129">Request body</span></span>
<span data-ttu-id="0bca4-130">在请求正文中，提供[accessReview](../resources/accessreview.md)对象的参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0bca4-130">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="0bca4-131">下表显示可更新 accessReview 时提供的属性。</span><span class="sxs-lookup"><span data-stu-id="0bca4-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="0bca4-132">属性</span><span class="sxs-lookup"><span data-stu-id="0bca4-132">Property</span></span>     | <span data-ttu-id="0bca4-133">类型</span><span class="sxs-lookup"><span data-stu-id="0bca4-133">Type</span></span>        | <span data-ttu-id="0bca4-134">说明</span><span class="sxs-lookup"><span data-stu-id="0bca4-134">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="0bca4-135">访问审阅名称。</span><span class="sxs-lookup"><span data-stu-id="0bca4-135">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="0bca4-136">审阅安排在启动时 DateTime。</span><span class="sxs-lookup"><span data-stu-id="0bca4-136">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="0bca4-137">这必须是在将来的日期。</span><span class="sxs-lookup"><span data-stu-id="0bca4-137">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="0bca4-138">审阅安排结束时 DateTime。</span><span class="sxs-lookup"><span data-stu-id="0bca4-138">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="0bca4-139">这必须是至少一个日期晚于开始日期。</span><span class="sxs-lookup"><span data-stu-id="0bca4-139">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="0bca4-140">说明，向审阅者显示。</span><span class="sxs-lookup"><span data-stu-id="0bca4-140">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="0bca4-141">响应</span><span class="sxs-lookup"><span data-stu-id="0bca4-141">Response</span></span>
<span data-ttu-id="0bca4-142">如果成功，此方法返回`204, Accepted`响应代码和响应正文中的[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0bca4-142">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bca4-143">示例</span><span class="sxs-lookup"><span data-stu-id="0bca4-143">Example</span></span>

<span data-ttu-id="0bca4-144">这是一次性的 （不) 访问审阅更新的示例。</span><span class="sxs-lookup"><span data-stu-id="0bca4-144">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="0bca4-145">请求</span><span class="sxs-lookup"><span data-stu-id="0bca4-145">Request</span></span>
<span data-ttu-id="0bca4-146">在请求正文中，提供[accessReview](../resources/accessreview.md)对象的新属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0bca4-146">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="0bca4-147">响应</span><span class="sxs-lookup"><span data-stu-id="0bca4-147">Response</span></span>
><span data-ttu-id="0bca4-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0bca4-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
