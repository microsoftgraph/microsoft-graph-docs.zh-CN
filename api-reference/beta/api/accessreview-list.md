---
title: 列出 accessReviews
description: 检索 businessFlowTemplate 的 accessReview 对象。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 443ffc2c5a31ac33cba89cb689884a3bae4ab645
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048489"
---
# <a name="list-accessreviews"></a><span data-ttu-id="4d4d4-103">列出 accessReviews</span><span class="sxs-lookup"><span data-stu-id="4d4d4-103">List accessReviews</span></span>

<span data-ttu-id="4d4d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d4d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d4d4-105">检索特定[businessFlowTemplate](../resources/businessflowtemplate.md)的[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-105">Retrieve the [accessReview](../resources/accessreview.md) objects for a particular [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span> <span data-ttu-id="4d4d4-106">对于使用该业务流程模板创建的每次一次性和定期访问评审，将返回零个或多个 **accessReview** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-106">A list of zero or more **accessReview** objects are returned, for each one-time and recurring access review that was created with that business flow template.</span></span>  <span data-ttu-id="4d4d4-107">请注意，业务流程模板的 ID 区分大小写。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-107">Note that business flow template IDs are case sensitive.</span></span>

>[!NOTE]
> <span data-ttu-id="4d4d4-108">如果与筛选器匹配的任何访问评审是定期访问评审，则除了任何当前、过去和下一个即将发生的实例之外，还将返回一 **个 accessReview** 对象以表示整个定期系列。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-108">If any of the access reviews that match the filter is a recurring access review, one **accessReview** object will be returned to represent each recurring series as a whole, in addition to any current, past and the next upcoming instance.</span></span> <span data-ttu-id="4d4d4-109">例如，如果每月对组 A 的来宾成员进行定期访问评审，对组 B 的来宾成员进行季度定期访问评审，以及对组 C 的来宾成员的一次性访问评审，则每个定期访问评审都刚刚开始，并且调用方使用查看组的来宾成员的业务流程模板查询访问评审，将返回表示三个系列中的三个对象，以及当前访问评审实例的三个对象，以及下一个即将推出的实例可能返回的三个对象。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-109">For example, if there is a monthly recurring access review of guest members of group A, a quarterly recurring access review of guest members of group B, and a one-time access review of guest members of group C, each of these recurrences have just started, and the caller queries for access reviews with a business flow template of reviews of guest members of groups, three objects will be returned representing the three series, as well as three objects for the current access review instances, and potentially three objects for the next upcoming instances.</span></span> <span data-ttu-id="4d4d4-110">若要检索定期访问评审的实例，或为特定月份或季度安排的访问评审实例，调用方随后可以导航定期 **accessReview** 对象的实例关系。 </span><span class="sxs-lookup"><span data-stu-id="4d4d4-110">To retrieve the instances of a recurring access review, or the access review instance scheduled for a particular month or quarter, the caller can subsequently navigate the **instance** relationship of the recurring **accessReview** object.</span></span> <span data-ttu-id="4d4d4-111">实例 **关系** 链接到定期访问评审的当前或过去实例的 **accessReview** 对象。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-111">The **instance** relationship links to the **accessReview** objects for a current or the past instances of the recurring access review.</span></span>

<span data-ttu-id="4d4d4-112">如果许多访问评审与筛选器匹配，为了提高效率并避免超时，请检索页面中的 结果集，方法包括页面大小为 100 的查询参数和请求中的 query 参数。 `$top` `$skip=0`</span><span class="sxs-lookup"><span data-stu-id="4d4d4-112">If many access reviews match the filter, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the `$top` query parameter with a page size, for example 100, and the `$skip=0` query parameter in the request.</span></span> <span data-ttu-id="4d4d4-113">即使您预计请求将跨越多个页面，也可以包含这些参数。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-113">These parameters can be included even when you do not anticipate that the request will span multiple pages.</span></span> <span data-ttu-id="4d4d4-114">当结果集跨多个页面时，Microsoft Graph 返回该页面，该页面在响应中包含指向下一 `@odata.nextLink` 页结果的 URL 中的属性。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-114">When a result set spans multiple pages, Microsoft Graph returns that page with an `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="4d4d4-115">如果该属性存在，请继续使用每次响应中的 `@odata.nextLink` URL 来创建额外请求，直至返回所有结果，如[在应用中对 Microsoft Graph 数据进行分页](/graph/paging.md)一文中所述。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-115">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging.md).</span></span>

<span data-ttu-id="4d4d4-116">此 API 返回的 **accessReview** 对象不包括嵌套结构属性，如 **设置** 或 关系。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-116">The **accessReview** objects returned by this API will not include nested structure properties such as **settings**, or relationships.</span></span>  <span data-ttu-id="4d4d4-117">若要检索访问评审设置或关系，请使用 [get accessReview](accessreview-get.md) API。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-117">To retrieve an access review settings or relationships, use the [get accessReview](accessreview-get.md) API.</span></span>


## <a name="permissions"></a><span data-ttu-id="4d4d4-118">权限</span><span class="sxs-lookup"><span data-stu-id="4d4d4-118">Permissions</span></span>
<span data-ttu-id="4d4d4-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d4d4-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d4d4-121">Permission type</span></span>                        | <span data-ttu-id="4d4d4-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4d4d4-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d4d4-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d4d4-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d4d4-124">AccessReview.Read.All、AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d4d4-124">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="4d4d4-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d4d4-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d4d4-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-126">Not supported.</span></span> |
|<span data-ttu-id="4d4d4-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d4d4-127">Application</span></span>                            | <span data-ttu-id="4d4d4-128">AccessReview.Read.All、AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="4d4d4-128">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="4d4d4-129">登录用户还必须具有允许其阅读访问评审的目录角色。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-129">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="4d4d4-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d4d4-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}&$top={pagesize}&$skip=0
```
## <a name="request-headers"></a><span data-ttu-id="4d4d4-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d4d4-131">Request headers</span></span>
| <span data-ttu-id="4d4d4-132">名称</span><span class="sxs-lookup"><span data-stu-id="4d4d4-132">Name</span></span>         | <span data-ttu-id="4d4d4-133">类型</span><span class="sxs-lookup"><span data-stu-id="4d4d4-133">Type</span></span>        | <span data-ttu-id="4d4d4-134">说明</span><span class="sxs-lookup"><span data-stu-id="4d4d4-134">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4d4d4-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d4d4-135">Authorization</span></span> | <span data-ttu-id="4d4d4-136">string</span><span class="sxs-lookup"><span data-stu-id="4d4d4-136">string</span></span> | <span data-ttu-id="4d4d4-p106">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-p106">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d4d4-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d4d4-139">Request body</span></span>
<span data-ttu-id="4d4d4-140">不提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-140">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="4d4d4-141">响应</span><span class="sxs-lookup"><span data-stu-id="4d4d4-141">Response</span></span>
<span data-ttu-id="4d4d4-142">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReview](../resources/accessreview.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-142">If successful, this method returns a `200 OK` response code and an array of [accessReview](../resources/accessreview.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4d4d4-143">示例</span><span class="sxs-lookup"><span data-stu-id="4d4d4-143">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="4d4d4-144">请求</span><span class="sxs-lookup"><span data-stu-id="4d4d4-144">Request</span></span>
<span data-ttu-id="4d4d4-145">以下示例显示检索业务流程模板"6e4f3d20-c5c3-407f-9695-8460952bcc68"的所有一次性和定期访问评审的请求。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-145">The following example shows a request to retrieve all the one-time and recurring access reviews for a business flow template '6e4f3d20-c5c3-407f-9695-8460952bcc68'.</span></span>

# <a name="http"></a>[<span data-ttu-id="4d4d4-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d4d4-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviews"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews?$filter=businessFlowTemplateId+eq+'6e4f3d20-c5c3-407f-9695-8460952bcc68'&$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="4d4d4-147">C#</span><span class="sxs-lookup"><span data-stu-id="4d4d4-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d4d4-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d4d4-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d4d4-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d4d4-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4d4d4-150">Java</span><span class="sxs-lookup"><span data-stu-id="4d4d4-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---


##### <a name="response"></a><span data-ttu-id="4d4d4-151">响应</span><span class="sxs-lookup"><span data-stu-id="4d4d4-151">Response</span></span>
><span data-ttu-id="4d4d4-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4d4d4-152">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="4d4d4-153">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4d4d4-153">See also</span></span>

- [<span data-ttu-id="4d4d4-154">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="4d4d4-154">Get accessReview</span></span>](accessreview-get.md)


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


