---
title: 更新 accessReview
description: 在 "Azure AD 访问评论" 功能中, 更新现有 accessReview 对象以更改其一个或多个属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6818c8f2c8d7c0dca57577b784f85a7b9da30d5a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945947"
---
# <a name="update-accessreview"></a><span data-ttu-id="c0ffa-103">更新 accessReview</span><span class="sxs-lookup"><span data-stu-id="c0ffa-103">Update accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0ffa-104">在 "Azure AD[访问评论](../resources/accessreviews-root.md)" 功能中, 更新现有[accessReview](../resources/accessreview.md)对象以更改其一个或多个属性。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="c0ffa-105">此 API 不用于更改审阅的审阅者或决策。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-105">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="c0ffa-106">若要更改审阅者, 请使用[addReviewer](accessreview-addreviewer.md)或[removeReviewer](accessreview-removereviewer.md) api。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-106">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="c0ffa-107">若要停止已启动的一次性审核, 或提前审核已启动的定期检查实例, 请提前使用[stop](accessreview-stop.md) API。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-107">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="c0ffa-108">若要将决策应用于目标组或应用访问权限, 请使用[应用](accessreview-apply.md)API。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-108">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="c0ffa-109">权限</span><span class="sxs-lookup"><span data-stu-id="c0ffa-109">Permissions</span></span>
<span data-ttu-id="c0ffa-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0ffa-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0ffa-112">Permission type</span></span>                        | <span data-ttu-id="c0ffa-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0ffa-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0ffa-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0ffa-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0ffa-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0ffa-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="c0ffa-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0ffa-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0ffa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-117">Not supported.</span></span> |
|<span data-ttu-id="c0ffa-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0ffa-118">Application</span></span>                            | <span data-ttu-id="c0ffa-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0ffa-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0ffa-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="c0ffa-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0ffa-121">Request headers</span></span>
| <span data-ttu-id="c0ffa-122">名称</span><span class="sxs-lookup"><span data-stu-id="c0ffa-122">Name</span></span>         | <span data-ttu-id="c0ffa-123">类型</span><span class="sxs-lookup"><span data-stu-id="c0ffa-123">Type</span></span>        | <span data-ttu-id="c0ffa-124">说明</span><span class="sxs-lookup"><span data-stu-id="c0ffa-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c0ffa-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0ffa-125">Authorization</span></span> | <span data-ttu-id="c0ffa-126">string</span><span class="sxs-lookup"><span data-stu-id="c0ffa-126">string</span></span> | <span data-ttu-id="c0ffa-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0ffa-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0ffa-129">Request body</span></span>
<span data-ttu-id="c0ffa-130">在请求正文中, 提供[accessReview](../resources/accessreview.md)对象的参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-130">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="c0ffa-131">下表显示了在更新 accessReview 时可提供的属性。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="c0ffa-132">属性</span><span class="sxs-lookup"><span data-stu-id="c0ffa-132">Property</span></span>     | <span data-ttu-id="c0ffa-133">类型</span><span class="sxs-lookup"><span data-stu-id="c0ffa-133">Type</span></span>        | <span data-ttu-id="c0ffa-134">说明</span><span class="sxs-lookup"><span data-stu-id="c0ffa-134">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="c0ffa-135">访问审阅名称。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-135">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="c0ffa-136">计划开始评审时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-136">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="c0ffa-137">这必须是将来的日期。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-137">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="c0ffa-138">计划结束评审时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-138">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="c0ffa-139">此时间必须至少为一个晚于开始日期的一天。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-139">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="c0ffa-140">要向审阅者显示的说明。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-140">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="c0ffa-141">响应</span><span class="sxs-lookup"><span data-stu-id="c0ffa-141">Response</span></span>
<span data-ttu-id="c0ffa-142">如果成功, 此方法在响应`204, Accepted`正文中返回响应代码和[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-142">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0ffa-143">示例</span><span class="sxs-lookup"><span data-stu-id="c0ffa-143">Example</span></span>

<span data-ttu-id="c0ffa-144">这是更新一次性 (不定期) 访问评审的示例。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-144">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="c0ffa-145">请求</span><span class="sxs-lookup"><span data-stu-id="c0ffa-145">Request</span></span>
<span data-ttu-id="c0ffa-146">在请求正文中, 提供[accessReview](../resources/accessreview.md)对象的新属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-146">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c0ffa-147">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c0ffa-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews/006111db-0810-4494-a6df-904d368bd81b
Content-type: application/json

{
    "displayName":"TestReview new name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c0ffa-148">C#</span><span class="sxs-lookup"><span data-stu-id="c0ffa-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0ffa-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0ffa-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c0ffa-150">目标-C</span><span class="sxs-lookup"><span data-stu-id="c0ffa-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c0ffa-151">Java</span><span class="sxs-lookup"><span data-stu-id="c0ffa-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c0ffa-152">响应</span><span class="sxs-lookup"><span data-stu-id="c0ffa-152">Response</span></span>
><span data-ttu-id="c0ffa-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c0ffa-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
