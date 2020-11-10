---
title: 列出 accessReviews
description: 检索 businessFlowTemplate 的 accessReview 对象。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c76dc3a245e003838290f3d233941e6535347b72
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951639"
---
# <a name="list-accessreviews"></a><span data-ttu-id="f57a6-103">列出 accessReviews</span><span class="sxs-lookup"><span data-stu-id="f57a6-103">List accessReviews</span></span>

<span data-ttu-id="f57a6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f57a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f57a6-105">检索特定[businessFlowTemplate](../resources/businessflowtemplate.md)的[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f57a6-105">Retrieve the [accessReview](../resources/accessreview.md) objects for a particular [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span> <span data-ttu-id="f57a6-106">返回零个或多个 **accessReview** 对象的列表，对于使用该业务流模板创建的每个一次性和定期访问评审。</span><span class="sxs-lookup"><span data-stu-id="f57a6-106">A list of zero or more **accessReview** objects are returned, for each one-time and recurring access review that was created with that business flow template.</span></span>  <span data-ttu-id="f57a6-107">请注意，业务流模板 Id 区分大小写。</span><span class="sxs-lookup"><span data-stu-id="f57a6-107">Note that business flow template IDs are case sensitive.</span></span>

>[!NOTE]
> <span data-ttu-id="f57a6-108">如果与筛选器匹配的任何访问评审是定期访问审核，则将返回一个 **accessReview** 对象，以将每个定期系列作为一个整体来表示，以及任何当前的过去和下一个即将开始的实例。</span><span class="sxs-lookup"><span data-stu-id="f57a6-108">If any of the access reviews that match the filter is a recurring access review, one **accessReview** object will be returned to represent each recurring series as a whole, in addition to any current, past and the next upcoming instance.</span></span> <span data-ttu-id="f57a6-109">例如，如果对组 A 的来宾成员进行每月定期访问审核，则为组 B 的来宾成员进行季度定期访问审核，并对组 C 中的来宾成员进行一次性访问审核，每个重复启动时刚刚启动，并且呼叫者使用对组的来宾成员审阅的业务流模板来查询访问审阅，将返回三个对象，其中包含三个系列，以及当前访问评审实例的三个对象，以及下一个即将发生的实例的可能三个对象。</span><span class="sxs-lookup"><span data-stu-id="f57a6-109">For example, if there is a monthly recurring access review of guest members of group A, a quarterly recurring access review of guest members of group B, and a one-time access review of guest members of group C, each of these recurrences have just started, and the caller queries for access reviews with a business flow template of reviews of guest members of groups, three objects will be returned representing the three series, as well as three objects for the current access review instances, and potentially three objects for the next upcoming instances.</span></span> <span data-ttu-id="f57a6-110">若要检索定期访问审核实例或为特定月份或季度计划的访问评审实例，调用方可以随后导航到定期 **accessReview** 对象的 **实例** 关系。</span><span class="sxs-lookup"><span data-stu-id="f57a6-110">To retrieve the instances of a recurring access review, or the access review instance scheduled for a particular month or quarter, the caller can subsequently navigate the **instance** relationship of the recurring **accessReview** object.</span></span> <span data-ttu-id="f57a6-111">指向当前或过去的定期访问审核实例的 **accessReview** 对象的 **实例** 关系。</span><span class="sxs-lookup"><span data-stu-id="f57a6-111">The **instance** relationship links to the **accessReview** objects for a current or the past instances of the recurring access review.</span></span>

<span data-ttu-id="f57a6-112">如果许多访问评审与筛选器匹配，则要提高效率并避免超时，请在页面中检索结果集，方法是将 `$top` 查询参数包含页面大小（例如，100）和 `$skip=0` 请求中的查询参数。</span><span class="sxs-lookup"><span data-stu-id="f57a6-112">If many access reviews match the filter, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the `$top` query parameter with a page size, for example 100, and the `$skip=0` query parameter in the request.</span></span> <span data-ttu-id="f57a6-113">即使您不预计请求将跨多个页面，也可以包含这些参数。</span><span class="sxs-lookup"><span data-stu-id="f57a6-113">These parameters can be included even when you do not anticipate that the request will span multiple pages.</span></span> <span data-ttu-id="f57a6-114">当结果集跨多个页面时，Microsoft Graph 将返回该页面，其中 `@odata.nextLink` 包含响应中包含指向下一页结果的 URL 的属性。</span><span class="sxs-lookup"><span data-stu-id="f57a6-114">When a result set spans multiple pages, Microsoft Graph returns that page with an `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="f57a6-115">如果该属性存在，请继续使用每次响应中的 `@odata.nextLink` URL 来创建额外请求，直至返回所有结果，如[在应用中对 Microsoft Graph 数据进行分页](/graph/paging.md)一文中所述。</span><span class="sxs-lookup"><span data-stu-id="f57a6-115">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging.md).</span></span>

<span data-ttu-id="f57a6-116">此 API 返回的 **accessReview** 对象将不包含嵌套的结构属性（如 **设置** 或关系）。</span><span class="sxs-lookup"><span data-stu-id="f57a6-116">The **accessReview** objects returned by this API will not include nested structure properties such as **settings** , or relationships.</span></span>  <span data-ttu-id="f57a6-117">若要检索访问审核设置或关系，请使用 [Get accessReview](accessreview-get.md) API。</span><span class="sxs-lookup"><span data-stu-id="f57a6-117">To retrieve an access review settings or relationships, use the [get accessReview](accessreview-get.md) API.</span></span>


## <a name="permissions"></a><span data-ttu-id="f57a6-118">权限</span><span class="sxs-lookup"><span data-stu-id="f57a6-118">Permissions</span></span>
<span data-ttu-id="f57a6-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f57a6-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f57a6-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="f57a6-121">Permission type</span></span>                        | <span data-ttu-id="f57a6-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f57a6-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f57a6-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f57a6-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="f57a6-124">AccessReview、AccessReview、成员身份、AccessReview。所有</span><span class="sxs-lookup"><span data-stu-id="f57a6-124">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="f57a6-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f57a6-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f57a6-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="f57a6-126">Not supported.</span></span> |
|<span data-ttu-id="f57a6-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="f57a6-127">Application</span></span>                            | <span data-ttu-id="f57a6-128">AccessReview、AccessReview、成员身份</span><span class="sxs-lookup"><span data-stu-id="f57a6-128">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="f57a6-129">登录用户还必须位于允许他们阅读访问审核的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="f57a6-129">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="f57a6-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f57a6-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}&$top={pagesize}&$skip=0
```
## <a name="request-headers"></a><span data-ttu-id="f57a6-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="f57a6-131">Request headers</span></span>
| <span data-ttu-id="f57a6-132">名称</span><span class="sxs-lookup"><span data-stu-id="f57a6-132">Name</span></span>         | <span data-ttu-id="f57a6-133">类型</span><span class="sxs-lookup"><span data-stu-id="f57a6-133">Type</span></span>        | <span data-ttu-id="f57a6-134">说明</span><span class="sxs-lookup"><span data-stu-id="f57a6-134">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f57a6-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="f57a6-135">Authorization</span></span> | <span data-ttu-id="f57a6-136">string</span><span class="sxs-lookup"><span data-stu-id="f57a6-136">string</span></span> | <span data-ttu-id="f57a6-p106">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="f57a6-p106">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f57a6-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="f57a6-139">Request body</span></span>
<span data-ttu-id="f57a6-140">请勿提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="f57a6-140">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="f57a6-141">响应</span><span class="sxs-lookup"><span data-stu-id="f57a6-141">Response</span></span>
<span data-ttu-id="f57a6-142">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [accessReview](../resources/accessreview.md) 对象的数组。</span><span class="sxs-lookup"><span data-stu-id="f57a6-142">If successful, this method returns a `200 OK` response code and an array of [accessReview](../resources/accessreview.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f57a6-143">示例</span><span class="sxs-lookup"><span data-stu-id="f57a6-143">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="f57a6-144">请求</span><span class="sxs-lookup"><span data-stu-id="f57a6-144">Request</span></span>
<span data-ttu-id="f57a6-145">下面的示例演示检索业务流模板 "6e4f3d20-c5c3-407f-9695-8460952bcc68" 的所有一次性和定期访问评审的请求。</span><span class="sxs-lookup"><span data-stu-id="f57a6-145">The following example shows a request to retrieve all the one-time and recurring access reviews for a business flow template '6e4f3d20-c5c3-407f-9695-8460952bcc68'.</span></span>

# <a name="http"></a>[<span data-ttu-id="f57a6-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="f57a6-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviews"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews?$filter=businessFlowTemplateId+eq+'6e4f3d20-c5c3-407f-9695-8460952bcc68'&$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="f57a6-147">C#</span><span class="sxs-lookup"><span data-stu-id="f57a6-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f57a6-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f57a6-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f57a6-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f57a6-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f57a6-150">Java</span><span class="sxs-lookup"><span data-stu-id="f57a6-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---


##### <a name="response"></a><span data-ttu-id="f57a6-151">响应</span><span class="sxs-lookup"><span data-stu-id="f57a6-151">Response</span></span>
><span data-ttu-id="f57a6-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f57a6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
       {
         "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
         "displayName": "review",
         "startDateTime": "2017-11-14T01:14:54.89Z",
         "endDateTime": "2017-12-14T01:14:54.89Z",
         "status": "InProgress",
         "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
         "reviewerType": "self",
         "description": "",
         "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"}
       }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="f57a6-154">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f57a6-154">See also</span></span>

- [<span data-ttu-id="f57a6-155">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="f57a6-155">Get accessReview</span></span>](accessreview-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviews",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


