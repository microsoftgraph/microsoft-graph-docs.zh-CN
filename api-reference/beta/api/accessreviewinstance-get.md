---
title: 获取 accessReviewInstance
description: 检索 accessReviewInstance 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: bd333a0620b8825400f89338112060c48611f302
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030738"
---
# <a name="get-accessreviewinstance"></a><span data-ttu-id="c2318-103">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="c2318-103">Get accessReviewInstance</span></span>

<span data-ttu-id="c2318-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2318-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2318-105">使用 [accessReviewInstance](../resources/accessreviewinstance.md) 的标识符及其父 [accessReviewScheduleDefinition 检索 accessReviewInstance 对象](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="c2318-105">Retrieve an [accessReviewInstance](../resources/accessreviewinstance.md) object using the identifier of an accessReviewInstance and its parent [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="c2318-106">这将返回实例的所有属性，关联的 [accessReviewInstanceDecisionItems 除外](../resources/accessreviewinstancedecisionitem.md)。</span><span class="sxs-lookup"><span data-stu-id="c2318-106">This returns all properties of the instance except for the associated [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md).</span></span>

<span data-ttu-id="c2318-107">若要检索有关实例的决策，请使用 [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md)。</span><span class="sxs-lookup"><span data-stu-id="c2318-107">To retrieve the decisions on the instance, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2318-108">权限</span><span class="sxs-lookup"><span data-stu-id="c2318-108">Permissions</span></span>
<span data-ttu-id="c2318-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2318-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2318-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2318-111">Permission type</span></span>                        | <span data-ttu-id="c2318-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2318-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2318-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2318-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2318-114">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2318-114">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="c2318-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2318-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2318-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2318-116">Not supported.</span></span>|
|<span data-ttu-id="c2318-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2318-117">Application</span></span>                            | <span data-ttu-id="c2318-118">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2318-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="c2318-119">为了调用此 API，已登录用户还必须位于允许他们阅读访问评审的目录角色中，或者可以将该用户分配为访问评审的审阅者。</span><span class="sxs-lookup"><span data-stu-id="c2318-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="c2318-120">有关详细信息，请参阅访问评审的角色和 [权限要求](../resources/accessreviewsv2-root.md)。</span><span class="sxs-lookup"><span data-stu-id="c2318-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="c2318-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2318-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c2318-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c2318-122">Optional query parameters</span></span>
<span data-ttu-id="c2318-123">此方法支持 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c2318-123">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="c2318-124">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c2318-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2318-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2318-125">Request headers</span></span>
<span data-ttu-id="c2318-126">无。</span><span class="sxs-lookup"><span data-stu-id="c2318-126">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="c2318-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2318-127">Request body</span></span>
<span data-ttu-id="c2318-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c2318-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2318-129">响应</span><span class="sxs-lookup"><span data-stu-id="c2318-129">Response</span></span>
<span data-ttu-id="c2318-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewInstance](../resources/accessreviewinstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c2318-130">If successful, this method returns a `200 OK` response code and an [accessReviewInstance](../resources/accessreviewinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c2318-131">示例</span><span class="sxs-lookup"><span data-stu-id="c2318-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="c2318-132">请求</span><span class="sxs-lookup"><span data-stu-id="c2318-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c2318-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2318-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/6af553ce-104d-4842-ab5f-67d7b556e9dd/instances/9ea56d3c-8746-4cdf-9ccc-c7fe1a267c24
```
# <a name="c"></a>[<span data-ttu-id="c2318-134">C#</span><span class="sxs-lookup"><span data-stu-id="c2318-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2318-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2318-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2318-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2318-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2318-137">Java</span><span class="sxs-lookup"><span data-stu-id="c2318-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---



### <a name="response"></a><span data-ttu-id="c2318-138">响应</span><span class="sxs-lookup"><span data-stu-id="c2318-138">Response</span></span>
><span data-ttu-id="c2318-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c2318-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="c2318-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c2318-140">See also</span></span>

- [<span data-ttu-id="c2318-141">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="c2318-141">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="c2318-142">列出 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="c2318-142">List accessReviewInstance</span></span>](accessreviewinstance-list.md)


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
