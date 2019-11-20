---
title: 列出 accessReviews
description: 检索 businessFlowTemplate 的 accessReview 对象。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aa164aba8d59b2695ff39652e1ea12a587426321
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747144"
---
# <a name="list-accessreviews"></a><span data-ttu-id="2132f-103">列出 accessReviews</span><span class="sxs-lookup"><span data-stu-id="2132f-103">List accessReviews</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2132f-104">检索特定[businessFlowTemplate](../resources/businessflowtemplate.md)的[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2132f-104">Retrieve the [accessReview](../resources/accessreview.md) objects for a particular [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span> <span data-ttu-id="2132f-105">返回零个或多个**accessReview**对象的列表，对于使用该业务流模板创建的每个一次性和定期访问评审。</span><span class="sxs-lookup"><span data-stu-id="2132f-105">A list of zero or more **accessReview** objects are returned, for each one-time and recurring access review that was created with that business flow template.</span></span>  <span data-ttu-id="2132f-106">请注意，业务流模板 Id 区分大小写。</span><span class="sxs-lookup"><span data-stu-id="2132f-106">Note that business flow template IDs are case sensitive.</span></span>

>[!NOTE]
> <span data-ttu-id="2132f-107">如果与筛选器匹配的任何访问评审是定期访问审核，则将返回一个**accessReview**对象，以将每个定期系列表示为一个整体。</span><span class="sxs-lookup"><span data-stu-id="2132f-107">If any of the access reviews that match the filter is a recurring access review, one **accessReview** object will be returned to represent each recurring series as a whole.</span></span> <span data-ttu-id="2132f-108">例如，如果每月定期访问 a 组的来宾成员、组 B 的来宾成员的定期访问审核以及组 C 的来宾成员的一次性访问审核，并且呼叫者查询与业务流的访问审核对组的来宾成员审阅的模板，将返回三个对象。</span><span class="sxs-lookup"><span data-stu-id="2132f-108">For example, if there is a monthly recurring access review of guest members of group A, a quarterly recurring access review of guest members of group B, and a one-time access review of guest members of group C, and the caller queries for access reviews with a business flow template of reviews of guest members of groups, three objects will be returned.</span></span> <span data-ttu-id="2132f-109">若要检索定期访问审核实例或为特定月份或季度计划的访问评审实例，调用方可以随后导航到定期**accessReview**对象的**实例**关系。</span><span class="sxs-lookup"><span data-stu-id="2132f-109">To retrieve the instances of a recurring access review, or the access review instance scheduled for a particular month or quarter, the caller can subsequently navigate the **instance** relationship of the recurring **accessReview** object.</span></span> <span data-ttu-id="2132f-110">指向当前或过去的定期访问审核实例的**accessReview**对象的**实例**关系。</span><span class="sxs-lookup"><span data-stu-id="2132f-110">The **instance** relationship links to the **accessReview** objects for a current or the past instances of the recurring access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="2132f-111">权限</span><span class="sxs-lookup"><span data-stu-id="2132f-111">Permissions</span></span>
<span data-ttu-id="2132f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2132f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2132f-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="2132f-114">Permission type</span></span>                        | <span data-ttu-id="2132f-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2132f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2132f-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2132f-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="2132f-117">AccessReview、AccessReview、成员身份、AccessReview。所有</span><span class="sxs-lookup"><span data-stu-id="2132f-117">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="2132f-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2132f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2132f-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="2132f-119">Not supported.</span></span> |
|<span data-ttu-id="2132f-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="2132f-120">Application</span></span>                            | <span data-ttu-id="2132f-121">AccessReview、AccessReview、成员身份</span><span class="sxs-lookup"><span data-stu-id="2132f-121">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="2132f-122">登录用户还必须位于允许他们阅读访问审核的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="2132f-122">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="2132f-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2132f-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}
```
## <a name="request-headers"></a><span data-ttu-id="2132f-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="2132f-124">Request headers</span></span>
| <span data-ttu-id="2132f-125">名称</span><span class="sxs-lookup"><span data-stu-id="2132f-125">Name</span></span>         | <span data-ttu-id="2132f-126">类型</span><span class="sxs-lookup"><span data-stu-id="2132f-126">Type</span></span>        | <span data-ttu-id="2132f-127">说明</span><span class="sxs-lookup"><span data-stu-id="2132f-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2132f-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="2132f-128">Authorization</span></span> | <span data-ttu-id="2132f-129">string</span><span class="sxs-lookup"><span data-stu-id="2132f-129">string</span></span> | <span data-ttu-id="2132f-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="2132f-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2132f-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="2132f-132">Request body</span></span>
<span data-ttu-id="2132f-133">请勿提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="2132f-133">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="2132f-134">响应</span><span class="sxs-lookup"><span data-stu-id="2132f-134">Response</span></span>
<span data-ttu-id="2132f-135">如果成功，此方法在响应`200, OK`正文中返回响应代码和[accessReview](../resources/accessreview.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="2132f-135">If successful, this method returns a `200, OK` response code and an array of [accessReview](../resources/accessreview.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2132f-136">示例</span><span class="sxs-lookup"><span data-stu-id="2132f-136">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="2132f-137">请求</span><span class="sxs-lookup"><span data-stu-id="2132f-137">Request</span></span>
<span data-ttu-id="2132f-138">下面的示例演示检索业务流模板 "6e4f3d20-c5c3-407f-9695-8460952bcc68" 的所有一次性和定期访问评审的请求。</span><span class="sxs-lookup"><span data-stu-id="2132f-138">The following example shows a request to retrieve all the one-time and recurring access reviews for a business flow template '6e4f3d20-c5c3-407f-9695-8460952bcc68'.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2132f-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="2132f-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviews"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews?$filter=businessFlowTemplateId+eq+'6e4f3d20-c5c3-407f-9695-8460952bcc68'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2132f-140">C#</span><span class="sxs-lookup"><span data-stu-id="2132f-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2132f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2132f-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2132f-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2132f-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---
null
---


##### <a name="response"></a><span data-ttu-id="2132f-143">响应</span><span class="sxs-lookup"><span data-stu-id="2132f-143">Response</span></span>
><span data-ttu-id="2132f-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2132f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="2132f-146">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2132f-146">See also</span></span>

- [<span data-ttu-id="2132f-147">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="2132f-147">Get accessReview</span></span>](accessreview-get.md)


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
