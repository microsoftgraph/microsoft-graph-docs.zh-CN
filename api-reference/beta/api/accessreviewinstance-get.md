---
title: 获取 accessReviewInstance
description: 检索 accessReviewInstance 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e8132815289848c7290b0a09ce2478665e1bbd11
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507192"
---
# <a name="get-accessreviewinstance"></a><span data-ttu-id="268b1-103">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="268b1-103">Get accessReviewInstance</span></span>

<span data-ttu-id="268b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="268b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="268b1-105">使用 [accessReviewInstance](../resources/accessreviewinstance.md) 的标识符及其父 [accessReviewScheduleDefinition 检索 accessReviewInstance 对象](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="268b1-105">Retrieve an [accessReviewInstance](../resources/accessreviewinstance.md) object using the identifier of an accessReviewInstance and its parent [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="268b1-106">这将返回实例的所有属性，关联的 [accessReviewInstanceDecisionItems 除外](../resources/accessreviewinstancedecisionitem.md)。</span><span class="sxs-lookup"><span data-stu-id="268b1-106">This returns all properties of the instance except for the associated [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md).</span></span>

<span data-ttu-id="268b1-107">若要检索有关实例的决策，请使用 [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md)。</span><span class="sxs-lookup"><span data-stu-id="268b1-107">To retrieve the decisions on the instance, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="268b1-108">权限</span><span class="sxs-lookup"><span data-stu-id="268b1-108">Permissions</span></span>
<span data-ttu-id="268b1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="268b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="268b1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="268b1-111">Permission type</span></span>                        | <span data-ttu-id="268b1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="268b1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="268b1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="268b1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="268b1-114">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="268b1-114">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="268b1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="268b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="268b1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="268b1-116">Not supported.</span></span>|
|<span data-ttu-id="268b1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="268b1-117">Application</span></span>                            | <span data-ttu-id="268b1-118">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="268b1-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="268b1-119">为了调用此 API，已登录用户还必须位于允许他们阅读访问评审的目录角色中，或者可以将该用户分配为访问评审的审阅者。</span><span class="sxs-lookup"><span data-stu-id="268b1-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="268b1-120">有关详细信息，请参阅访问评审的角色和 [权限要求](../resources/accessreviewsv2-root.md)。</span><span class="sxs-lookup"><span data-stu-id="268b1-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="268b1-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="268b1-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}
```
## <a name="request-headers"></a><span data-ttu-id="268b1-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="268b1-122">Request headers</span></span>
<span data-ttu-id="268b1-123">无。</span><span class="sxs-lookup"><span data-stu-id="268b1-123">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="268b1-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="268b1-124">Request body</span></span>
<span data-ttu-id="268b1-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="268b1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="268b1-126">响应</span><span class="sxs-lookup"><span data-stu-id="268b1-126">Response</span></span>
<span data-ttu-id="268b1-127">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewInstance](../resources/accessreviewinstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="268b1-127">If successful, this method returns a `200 OK` response code and an [accessReviewInstance](../resources/accessreviewinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="268b1-128">示例</span><span class="sxs-lookup"><span data-stu-id="268b1-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="268b1-129">请求</span><span class="sxs-lookup"><span data-stu-id="268b1-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="268b1-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="268b1-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/6af553ce-104d-4842-ab5f-67d7b556e9dd/instances/9ea56d3c-8746-4cdf-9ccc-c7fe1a267c24
```
# <a name="c"></a>[<span data-ttu-id="268b1-131">C#</span><span class="sxs-lookup"><span data-stu-id="268b1-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="268b1-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="268b1-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="268b1-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="268b1-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="268b1-134">Java</span><span class="sxs-lookup"><span data-stu-id="268b1-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---



### <a name="response"></a><span data-ttu-id="268b1-135">响应</span><span class="sxs-lookup"><span data-stu-id="268b1-135">Response</span></span>
><span data-ttu-id="268b1-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="268b1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="268b1-138">另请参阅</span><span class="sxs-lookup"><span data-stu-id="268b1-138">See also</span></span>

- [<span data-ttu-id="268b1-139">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="268b1-139">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="268b1-140">列出 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="268b1-140">List accessReviewInstance</span></span>](accessreviewinstance-list.md)


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
