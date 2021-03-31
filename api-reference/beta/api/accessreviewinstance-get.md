---
title: 获取 accessReviewInstance
description: 检索 accessReviewInstance 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 5f06848a6f1e77d97d7716b1d62a288368047c57
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468945"
---
# <a name="get-accessreviewinstance"></a><span data-ttu-id="04596-103">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="04596-103">Get accessReviewInstance</span></span>

<span data-ttu-id="04596-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04596-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04596-105">使用 [accessReviewInstance](../resources/accessreviewinstance.md) 的标识符及其父 [accessReviewScheduleDefinition 检索 accessReviewInstance 对象](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="04596-105">Retrieve an [accessReviewInstance](../resources/accessreviewinstance.md) object using the identifier of an accessReviewInstance and its parent [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="04596-106">这将返回实例的所有属性，关联的 [accessReviewInstanceDecisionItems 除外](../resources/accessreviewinstancedecisionitem.md)。</span><span class="sxs-lookup"><span data-stu-id="04596-106">This returns all properties of the instance except for the associated [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md).</span></span>

<span data-ttu-id="04596-107">若要检索有关实例的决策，请使用 [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md)。</span><span class="sxs-lookup"><span data-stu-id="04596-107">To retrieve the decisions on the instance, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="04596-108">权限</span><span class="sxs-lookup"><span data-stu-id="04596-108">Permissions</span></span>
<span data-ttu-id="04596-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="04596-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04596-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="04596-111">Permission type</span></span>                        | <span data-ttu-id="04596-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="04596-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="04596-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04596-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="04596-114">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04596-114">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="04596-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04596-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04596-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="04596-116">Not supported.</span></span>|
|<span data-ttu-id="04596-117">Application</span><span class="sxs-lookup"><span data-stu-id="04596-117">Application</span></span>                            | <span data-ttu-id="04596-118">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04596-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="04596-119">为了调用此 API，已登录用户还必须位于允许他们阅读访问评审的目录角色中，或者可以将该用户分配为访问评审的审阅者。</span><span class="sxs-lookup"><span data-stu-id="04596-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="04596-120">有关详细信息，请参阅访问评审的角色和 [权限要求](../resources/accessreviewsv2-root.md)。</span><span class="sxs-lookup"><span data-stu-id="04596-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="04596-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04596-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}
```
## <a name="request-headers"></a><span data-ttu-id="04596-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="04596-122">Request headers</span></span>
<span data-ttu-id="04596-123">无。</span><span class="sxs-lookup"><span data-stu-id="04596-123">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="04596-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="04596-124">Request body</span></span>
<span data-ttu-id="04596-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="04596-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04596-126">响应</span><span class="sxs-lookup"><span data-stu-id="04596-126">Response</span></span>
<span data-ttu-id="04596-127">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewInstance](../resources/accessreviewinstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="04596-127">If successful, this method returns a `200 OK` response code and an [accessReviewInstance](../resources/accessreviewinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04596-128">示例</span><span class="sxs-lookup"><span data-stu-id="04596-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="04596-129">请求</span><span class="sxs-lookup"><span data-stu-id="04596-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/6af553ce-104d-4842-ab5f-67d7b556e9dd/instances/9ea56d3c-8746-4cdf-9ccc-c7fe1a267c24
```
---



### <a name="response"></a><span data-ttu-id="04596-130">响应</span><span class="sxs-lookup"><span data-stu-id="04596-130">Response</span></span>
><span data-ttu-id="04596-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="04596-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('6af553ce-104d-4842-ab5f-67d7b556e9dd')/instances/$entity",
    "id": "9ea56d3c-8746-4cdf-9ccc-c7fe1a267c24",
    "startDateTime": "2021-03-11T16:44:59.337Z",
    "endDateTime": "2021-06-09T16:44:59.337Z",
    "status": "InProgress",
    "scope": {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/v1.0/groups/97eebd44-61fd-4d42-8b2a-a4de41b6c572/transitiveMembers",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
    }
}
```

## <a name="see-also"></a><span data-ttu-id="04596-133">另请参阅</span><span class="sxs-lookup"><span data-stu-id="04596-133">See also</span></span>

- [<span data-ttu-id="04596-134">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="04596-134">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="04596-135">列出 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="04596-135">List accessReviewInstance</span></span>](accessreviewinstance-list.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
