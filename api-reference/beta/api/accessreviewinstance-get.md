---
title: 获取 accessReviewInstance
description: 检索 accessReviewInstance 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b14fe31961524b6aef67d08e683bfecd7a2324c2
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000814"
---
# <a name="get-accessreviewinstance"></a><span data-ttu-id="d9522-103">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="d9522-103">Get accessReviewInstance</span></span>

<span data-ttu-id="d9522-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9522-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9522-105">使用 accessReviewInstance 的标识符和父[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)检索[accessReviewInstance](../resources/accessreviewinstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d9522-105">Retrieve an [accessReviewInstance](../resources/accessreviewinstance.md) object using the identifier of an accessReviewInstance and its parent [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="d9522-106">这将返回除关联的 [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md)之外的实例的所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9522-106">This returns all properties of the instance except for the associated [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md).</span></span>

<span data-ttu-id="d9522-107">若要检索有关实例的决策，请使用 [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md)。</span><span class="sxs-lookup"><span data-stu-id="d9522-107">To retrieve the decisions on the instance, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d9522-108">权限</span><span class="sxs-lookup"><span data-stu-id="d9522-108">Permissions</span></span>
<span data-ttu-id="d9522-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9522-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9522-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9522-111">Permission type</span></span>                        | <span data-ttu-id="d9522-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d9522-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9522-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9522-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9522-114">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="d9522-114">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="d9522-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9522-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9522-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9522-116">Not supported.</span></span>|
|<span data-ttu-id="d9522-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9522-117">Application</span></span>                            | <span data-ttu-id="d9522-118">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="d9522-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="d9522-119">若要调用此 API，登录用户还必须位于允许他们读取访问审核的目录角色中，或者可以将用户作为访问评审的审阅者进行分配。</span><span class="sxs-lookup"><span data-stu-id="d9522-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="d9522-120">有关更多详细信息，请参阅 [access 评审](../resources/accessreviewsv2-root.md)的角色和权限要求。</span><span class="sxs-lookup"><span data-stu-id="d9522-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="d9522-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9522-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}
```
## <a name="request-headers"></a><span data-ttu-id="d9522-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9522-122">Request headers</span></span>
<span data-ttu-id="d9522-123">无。</span><span class="sxs-lookup"><span data-stu-id="d9522-123">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="d9522-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9522-124">Request body</span></span>
<span data-ttu-id="d9522-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d9522-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9522-126">响应</span><span class="sxs-lookup"><span data-stu-id="d9522-126">Response</span></span>
<span data-ttu-id="d9522-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [accessReviewInstance](../resources/accessreviewinstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9522-127">If successful, this method returns a `200 OK` response code and an [accessReviewInstance](../resources/accessreviewinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9522-128">示例</span><span class="sxs-lookup"><span data-stu-id="d9522-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="d9522-129">请求</span><span class="sxs-lookup"><span data-stu-id="d9522-129">Request</span></span>


<!-- {
  "blockType": "request",
  "name": "get_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-444404f3baa6/instances/12490cdb-6a18-4c08-ba2c-44442f0a0138
```


### <a name="response"></a><span data-ttu-id="d9522-130">响应</span><span class="sxs-lookup"><span data-stu-id="d9522-130">Response</span></span>
><span data-ttu-id="d9522-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d9522-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "12490cdb-6a18-4c08-ba2c-44442f0a0138",
    "startDateTime": "2020-09-21T20:03:36Z",
    "endDateTime": "2020-09-23T20:03:36Z",
    "status": "NotStarted",
    "scope": {
        "query": "/groups/b7a4444b-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
}
```

## <a name="see-also"></a><span data-ttu-id="d9522-133">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d9522-133">See also</span></span>

- [<span data-ttu-id="d9522-134">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="d9522-134">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="d9522-135">列出 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="d9522-135">List accessReviewInstance</span></span>](accessreviewinstance-list.md)


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
