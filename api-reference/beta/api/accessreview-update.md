---
title: 更新 accessReview
description: 在 Azure AD 访问评审功能中，更新现有 accessReview 对象以更改其一个或多个属性。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 817cf535c68a775c7a90a639e09120e226c46115
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751006"
---
# <a name="update-accessreview"></a><span data-ttu-id="55b6f-103">更新 accessReview</span><span class="sxs-lookup"><span data-stu-id="55b6f-103">Update accessReview</span></span>

<span data-ttu-id="55b6f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55b6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55b6f-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，更新现有 [accessReview](../resources/accessreview.md) 对象以更改其一个或多个属性。</span><span class="sxs-lookup"><span data-stu-id="55b6f-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="55b6f-106">此 API 不用于更改审阅者或审阅决策。</span><span class="sxs-lookup"><span data-stu-id="55b6f-106">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="55b6f-107">若要更改审阅者，请使用 [addReviewer](accessreview-addreviewer.md) 或 [removeReviewer](accessreview-removereviewer.md) API。</span><span class="sxs-lookup"><span data-stu-id="55b6f-107">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="55b6f-108">若要停止已启动的一次性审阅或已启动的定期审阅实例，请尽早使用 [停止](accessreview-stop.md) API。</span><span class="sxs-lookup"><span data-stu-id="55b6f-108">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="55b6f-109">若要将决策应用于目标组或应用访问权限，请使用 [应用](accessreview-apply.md) API。</span><span class="sxs-lookup"><span data-stu-id="55b6f-109">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="55b6f-110">权限</span><span class="sxs-lookup"><span data-stu-id="55b6f-110">Permissions</span></span>
<span data-ttu-id="55b6f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55b6f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55b6f-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="55b6f-113">Permission type</span></span>                        | <span data-ttu-id="55b6f-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="55b6f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="55b6f-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55b6f-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="55b6f-116">AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55b6f-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="55b6f-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55b6f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55b6f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="55b6f-118">Not supported.</span></span> |
|<span data-ttu-id="55b6f-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="55b6f-119">Application</span></span>                            | <span data-ttu-id="55b6f-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="55b6f-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="55b6f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55b6f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="55b6f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="55b6f-122">Request headers</span></span>
| <span data-ttu-id="55b6f-123">名称</span><span class="sxs-lookup"><span data-stu-id="55b6f-123">Name</span></span>         | <span data-ttu-id="55b6f-124">类型</span><span class="sxs-lookup"><span data-stu-id="55b6f-124">Type</span></span>        | <span data-ttu-id="55b6f-125">说明</span><span class="sxs-lookup"><span data-stu-id="55b6f-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="55b6f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="55b6f-126">Authorization</span></span> | <span data-ttu-id="55b6f-127">string</span><span class="sxs-lookup"><span data-stu-id="55b6f-127">string</span></span> | <span data-ttu-id="55b6f-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="55b6f-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55b6f-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="55b6f-130">Request body</span></span>
<span data-ttu-id="55b6f-131">在请求正文中，提供 [accessReview](../resources/accessreview.md) 对象的参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55b6f-131">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="55b6f-132">下表显示更新 accessReview 时提供的属性。</span><span class="sxs-lookup"><span data-stu-id="55b6f-132">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="55b6f-133">属性</span><span class="sxs-lookup"><span data-stu-id="55b6f-133">Property</span></span>      | <span data-ttu-id="55b6f-134">类型</span><span class="sxs-lookup"><span data-stu-id="55b6f-134">Type</span></span>           | <span data-ttu-id="55b6f-135">说明</span><span class="sxs-lookup"><span data-stu-id="55b6f-135">Description</span></span>                                                                                                |
|:--------------|:---------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="55b6f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="55b6f-136">displayName</span></span>   | <span data-ttu-id="55b6f-137">String</span><span class="sxs-lookup"><span data-stu-id="55b6f-137">String</span></span>         | <span data-ttu-id="55b6f-138">访问评审名称。</span><span class="sxs-lookup"><span data-stu-id="55b6f-138">The access review name.</span></span>                                                                                    |
| <span data-ttu-id="55b6f-139">startDateTime</span><span class="sxs-lookup"><span data-stu-id="55b6f-139">startDateTime</span></span> | <span data-ttu-id="55b6f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55b6f-140">DateTimeOffset</span></span> | <span data-ttu-id="55b6f-141">计划开始审阅的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="55b6f-141">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="55b6f-142">这必须是将来的日期。</span><span class="sxs-lookup"><span data-stu-id="55b6f-142">This must be a date in the future.</span></span>                 |
| <span data-ttu-id="55b6f-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="55b6f-143">endDateTime</span></span>   | <span data-ttu-id="55b6f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55b6f-144">DateTimeOffset</span></span> | <span data-ttu-id="55b6f-145">计划结束审阅的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="55b6f-145">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="55b6f-146">这必须至少比开始日期晚一天。</span><span class="sxs-lookup"><span data-stu-id="55b6f-146">This must be at least one day later than the start date.</span></span> |
| <span data-ttu-id="55b6f-147">说明</span><span class="sxs-lookup"><span data-stu-id="55b6f-147">description</span></span>   | <span data-ttu-id="55b6f-148">String</span><span class="sxs-lookup"><span data-stu-id="55b6f-148">String</span></span>         | <span data-ttu-id="55b6f-149">向审阅者显示的说明。</span><span class="sxs-lookup"><span data-stu-id="55b6f-149">The description, to show to the reviewers.</span></span>                                                                 |



## <a name="response"></a><span data-ttu-id="55b6f-150">响应</span><span class="sxs-lookup"><span data-stu-id="55b6f-150">Response</span></span>
<span data-ttu-id="55b6f-151">如果成功，此方法在响应 `204 Accepted` 正文中返回 响应代码和 [accessReview](../resources/accessreview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="55b6f-151">If successful, this method returns a `204 Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55b6f-152">示例</span><span class="sxs-lookup"><span data-stu-id="55b6f-152">Example</span></span>

<span data-ttu-id="55b6f-153">这是一个更新一次访问 (访问) 的示例。</span><span class="sxs-lookup"><span data-stu-id="55b6f-153">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="55b6f-154">请求</span><span class="sxs-lookup"><span data-stu-id="55b6f-154">Request</span></span>
<span data-ttu-id="55b6f-155">在请求正文中，提供 [accessReview](../resources/accessreview.md) 对象的新属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55b6f-155">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="55b6f-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="55b6f-156">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="55b6f-157">C#</span><span class="sxs-lookup"><span data-stu-id="55b6f-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55b6f-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55b6f-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55b6f-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55b6f-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55b6f-160">Java</span><span class="sxs-lookup"><span data-stu-id="55b6f-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="55b6f-161">响应</span><span class="sxs-lookup"><span data-stu-id="55b6f-161">Response</span></span>
><span data-ttu-id="55b6f-162">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="55b6f-162">**Note:** The response object shown here might be shortened for readability.</span></span>
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


