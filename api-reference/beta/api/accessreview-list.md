---
title: 列出 accessReviews
description: 检索 businessFlowTemplate 的 accessReview 对象。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 46c9abdbc0a1d5dca4c4e61d423b23ed31691384
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36462520"
---
# <a name="list-accessreviews"></a><span data-ttu-id="078b5-103">列出 accessReviews</span><span class="sxs-lookup"><span data-stu-id="078b5-103">List accessReviews</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="078b5-104">检索特定[businessFlowTemplate](../resources/businessflowtemplate.md)的[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="078b5-104">Retrieve the [accessReview](../resources/accessreview.md) objects for a particular [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span> <span data-ttu-id="078b5-105">返回零个或多个**accessReview**对象的列表, 对于使用该业务流模板创建的每个一次性和定期访问评审。</span><span class="sxs-lookup"><span data-stu-id="078b5-105">A list of zero or more **accessReview** objects are returned, for each one-time and recurring access review that was created with that business flow template.</span></span>

>[!NOTE]
> <span data-ttu-id="078b5-106">如果与筛选器匹配的任何访问评审是定期访问审核, 则将返回一个**accessReview**对象, 以将每个定期系列表示为一个整体。</span><span class="sxs-lookup"><span data-stu-id="078b5-106">If any of the access reviews that match the filter is a recurring access review, one **accessReview** object will be returned to represent each recurring series as a whole.</span></span> <span data-ttu-id="078b5-107">例如, 如果每月定期访问 a 组的来宾成员、组 B 的来宾成员的定期访问审核以及组 C 的来宾成员的一次性访问审核, 并且呼叫者查询与业务流的访问审核对组的来宾成员审阅的模板, 将返回三个对象。</span><span class="sxs-lookup"><span data-stu-id="078b5-107">For example, if there is a monthly recurring access review of guest members of group A, a quarterly recurring access review of guest members of group B, and a one-time access review of guest members of group C, and the caller queries for access reviews with a business flow template of reviews of guest members of groups, three objects will be returned.</span></span> <span data-ttu-id="078b5-108">若要检索定期访问审核实例或为特定月份或季度计划的访问评审实例, 调用方可以随后导航到定期**accessReview**对象的**实例**关系。</span><span class="sxs-lookup"><span data-stu-id="078b5-108">To retrieve the instances of a recurring access review, or the access review instance scheduled for a particular month or quarter, the caller can subsequently navigate the **instance** relationship of the recurring **accessReview** object.</span></span> <span data-ttu-id="078b5-109">指向当前或过去的定期访问审核实例的**accessReview**对象的**实例**关系。</span><span class="sxs-lookup"><span data-stu-id="078b5-109">The **instance** relationship links to the **accessReview** objects for a current or the past instances of the recurring access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="078b5-110">权限</span><span class="sxs-lookup"><span data-stu-id="078b5-110">Permissions</span></span>
<span data-ttu-id="078b5-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="078b5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="078b5-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="078b5-113">Permission type</span></span>                        | <span data-ttu-id="078b5-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="078b5-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="078b5-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="078b5-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="078b5-116">AccessReview、AccessReview、成员身份、AccessReview。所有</span><span class="sxs-lookup"><span data-stu-id="078b5-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="078b5-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="078b5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="078b5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="078b5-118">Not supported.</span></span> |
|<span data-ttu-id="078b5-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="078b5-119">Application</span></span>                            | <span data-ttu-id="078b5-120">AccessReview、AccessReview、成员身份</span><span class="sxs-lookup"><span data-stu-id="078b5-120">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="078b5-121">登录用户还必须位于允许他们阅读访问审核的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="078b5-121">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="078b5-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="078b5-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}
```
## <a name="request-headers"></a><span data-ttu-id="078b5-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="078b5-123">Request headers</span></span>
| <span data-ttu-id="078b5-124">名称</span><span class="sxs-lookup"><span data-stu-id="078b5-124">Name</span></span>         | <span data-ttu-id="078b5-125">类型</span><span class="sxs-lookup"><span data-stu-id="078b5-125">Type</span></span>        | <span data-ttu-id="078b5-126">说明</span><span class="sxs-lookup"><span data-stu-id="078b5-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="078b5-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="078b5-127">Authorization</span></span> | <span data-ttu-id="078b5-128">string</span><span class="sxs-lookup"><span data-stu-id="078b5-128">string</span></span> | <span data-ttu-id="078b5-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="078b5-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="078b5-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="078b5-131">Request body</span></span>
<span data-ttu-id="078b5-132">请勿提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="078b5-132">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="078b5-133">响应</span><span class="sxs-lookup"><span data-stu-id="078b5-133">Response</span></span>
<span data-ttu-id="078b5-134">如果成功, 此方法在响应`200, OK`正文中返回响应代码和[accessReview](../resources/accessreview.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="078b5-134">If successful, this method returns a `200, OK` response code and an array of [accessReview](../resources/accessreview.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="078b5-135">示例</span><span class="sxs-lookup"><span data-stu-id="078b5-135">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="078b5-136">请求</span><span class="sxs-lookup"><span data-stu-id="078b5-136">Request</span></span>
<span data-ttu-id="078b5-137">下面的示例演示检索业务流模板 "6E4F3D20-C5C3-407F-9695-8460952BCC68" 的所有一次性和定期访问评审的请求。</span><span class="sxs-lookup"><span data-stu-id="078b5-137">The following example shows a request to retrieve all the one-time and recurring access reviews for a business flow template '6E4F3D20-C5C3-407F-9695-8460952BCC68'.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="078b5-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="078b5-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviews"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews?$filter=businessFlowTemplateId+eq+'6E4F3D20-C5C3-407F-9695-8460952BCC68'
```


---


##### <a name="response"></a><span data-ttu-id="078b5-139">响应</span><span class="sxs-lookup"><span data-stu-id="078b5-139">Response</span></span>
><span data-ttu-id="078b5-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="078b5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="078b5-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="078b5-142">See also</span></span>

- [<span data-ttu-id="078b5-143">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="078b5-143">Get accessReview</span></span>](accessreview-get.md)


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
