---
title: 更新 accessReview
description: 在 Azure AD 访问评审功能中，更新现有 accessReview 对象以更改其一个或多个属性。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6de1862411d20f1e1fc68fc202a5e59aa888f165
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439259"
---
# <a name="update-accessreview"></a><span data-ttu-id="f7d17-103">更新 accessReview</span><span class="sxs-lookup"><span data-stu-id="f7d17-103">Update accessReview</span></span>

<span data-ttu-id="f7d17-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7d17-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7d17-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，更新现有 [accessReview](../resources/accessreview.md) 对象以更改其一个或多个属性。</span><span class="sxs-lookup"><span data-stu-id="f7d17-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="f7d17-106">此 API 不用于更改审阅者或审阅决策。</span><span class="sxs-lookup"><span data-stu-id="f7d17-106">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="f7d17-107">若要更改审阅者，请使用 [addReviewer](accessreview-addreviewer.md) [或 removeReviewer](accessreview-removereviewer.md) API。</span><span class="sxs-lookup"><span data-stu-id="f7d17-107">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="f7d17-108">若要停止已启动的一次性审阅或已启动的定期评审实例，请尽早使用 [停止](accessreview-stop.md) API。</span><span class="sxs-lookup"><span data-stu-id="f7d17-108">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="f7d17-109">若要将决策应用于目标组或应用访问权限，请使用 [应用](accessreview-apply.md) API。</span><span class="sxs-lookup"><span data-stu-id="f7d17-109">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="f7d17-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="f7d17-110">Permissions</span></span>
<span data-ttu-id="f7d17-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7d17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7d17-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7d17-113">Permission type</span></span>                        | <span data-ttu-id="f7d17-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7d17-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7d17-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7d17-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7d17-116">AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7d17-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="f7d17-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7d17-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7d17-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7d17-118">Not supported.</span></span> |
|<span data-ttu-id="f7d17-119">Application</span><span class="sxs-lookup"><span data-stu-id="f7d17-119">Application</span></span>                            | <span data-ttu-id="f7d17-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="f7d17-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7d17-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7d17-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="f7d17-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7d17-122">Request headers</span></span>
| <span data-ttu-id="f7d17-123">名称</span><span class="sxs-lookup"><span data-stu-id="f7d17-123">Name</span></span>         | <span data-ttu-id="f7d17-124">类型</span><span class="sxs-lookup"><span data-stu-id="f7d17-124">Type</span></span>        | <span data-ttu-id="f7d17-125">说明</span><span class="sxs-lookup"><span data-stu-id="f7d17-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f7d17-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7d17-126">Authorization</span></span> | <span data-ttu-id="f7d17-127">string</span><span class="sxs-lookup"><span data-stu-id="f7d17-127">string</span></span> | <span data-ttu-id="f7d17-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7d17-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7d17-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7d17-130">Request body</span></span>
<span data-ttu-id="f7d17-131">在请求正文中，提供 [accessReview](../resources/accessreview.md) 对象参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7d17-131">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="f7d17-132">下表显示了在更新 accessReview 时提供的属性。</span><span class="sxs-lookup"><span data-stu-id="f7d17-132">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="f7d17-133">属性</span><span class="sxs-lookup"><span data-stu-id="f7d17-133">Property</span></span>     | <span data-ttu-id="f7d17-134">类型</span><span class="sxs-lookup"><span data-stu-id="f7d17-134">Type</span></span>        | <span data-ttu-id="f7d17-135">说明</span><span class="sxs-lookup"><span data-stu-id="f7d17-135">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="f7d17-136">访问评审名称。</span><span class="sxs-lookup"><span data-stu-id="f7d17-136">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="f7d17-137">计划开始审阅的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f7d17-137">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="f7d17-138">这必须是将来的日期。</span><span class="sxs-lookup"><span data-stu-id="f7d17-138">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="f7d17-139">计划结束审阅的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f7d17-139">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="f7d17-140">这必须至少比开始日期晚一天。</span><span class="sxs-lookup"><span data-stu-id="f7d17-140">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="f7d17-141">向审阅者显示的说明。</span><span class="sxs-lookup"><span data-stu-id="f7d17-141">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="f7d17-142">响应</span><span class="sxs-lookup"><span data-stu-id="f7d17-142">Response</span></span>
<span data-ttu-id="f7d17-143">如果成功，此方法在响应正文中返回响应代码 `204, Accepted` 和 [accessReview](../resources/accessreview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f7d17-143">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7d17-144">示例</span><span class="sxs-lookup"><span data-stu-id="f7d17-144">Example</span></span>

<span data-ttu-id="f7d17-145">这是一个更新一次访问 (访问评审) 的示例。</span><span class="sxs-lookup"><span data-stu-id="f7d17-145">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="f7d17-146">请求</span><span class="sxs-lookup"><span data-stu-id="f7d17-146">Request</span></span>
<span data-ttu-id="f7d17-147">在请求正文中，提供 [accessReview](../resources/accessreview.md) 对象的新属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7d17-147">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="f7d17-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7d17-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f7d17-149">C#</span><span class="sxs-lookup"><span data-stu-id="f7d17-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7d17-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7d17-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7d17-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7d17-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7d17-152">Java</span><span class="sxs-lookup"><span data-stu-id="f7d17-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f7d17-153">响应</span><span class="sxs-lookup"><span data-stu-id="f7d17-153">Response</span></span>
><span data-ttu-id="f7d17-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f7d17-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


