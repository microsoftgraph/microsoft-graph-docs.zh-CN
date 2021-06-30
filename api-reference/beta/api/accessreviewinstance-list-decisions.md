---
title: 列出决策
description: 从 decisions 导航属性获取 accessReviewInstanceDecisionItem 资源。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d86b5c939205fd03719ee6fcea543feaae751f28
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207642"
---
# <a name="list-decisions"></a><span data-ttu-id="22d08-103">列出决策</span><span class="sxs-lookup"><span data-stu-id="22d08-103">List decisions</span></span>
<span data-ttu-id="22d08-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22d08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22d08-105">从 [accessReviewInstance 上的决策获取 accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) [对象](../resources/accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="22d08-105">Get the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects from the decisions on an [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

>[!NOTE]
><span data-ttu-id="22d08-106">此 API 的默认页面大小为 100 accessReviewInstance 对象。</span><span class="sxs-lookup"><span data-stu-id="22d08-106">The default page size for this API is 100 accessReviewInstance objects.</span></span> <span data-ttu-id="22d08-107">若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。</span><span class="sxs-lookup"><span data-stu-id="22d08-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="22d08-108">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="22d08-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="22d08-109">权限</span><span class="sxs-lookup"><span data-stu-id="22d08-109">Permissions</span></span>
<span data-ttu-id="22d08-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22d08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22d08-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="22d08-112">Permission type</span></span>|<span data-ttu-id="22d08-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22d08-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22d08-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22d08-114">Delegated (work or school account)</span></span>|<span data-ttu-id="22d08-115">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22d08-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="22d08-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22d08-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22d08-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="22d08-117">Not supported.</span></span>|
|<span data-ttu-id="22d08-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="22d08-118">Application</span></span>|<span data-ttu-id="22d08-119">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22d08-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22d08-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22d08-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22d08-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="22d08-121">Optional query parameters</span></span>
<span data-ttu-id="22d08-122">此方法支持 `$select` 、 、 、 和 OData 查询参数 `$filter` `$orderBy` `$skip` `$top` 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="22d08-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="22d08-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="22d08-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="22d08-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="22d08-124">Request headers</span></span>
|<span data-ttu-id="22d08-125">名称</span><span class="sxs-lookup"><span data-stu-id="22d08-125">Name</span></span>|<span data-ttu-id="22d08-126">说明</span><span class="sxs-lookup"><span data-stu-id="22d08-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="22d08-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="22d08-127">Authorization</span></span>|<span data-ttu-id="22d08-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="22d08-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="22d08-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="22d08-130">Request body</span></span>
<span data-ttu-id="22d08-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="22d08-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22d08-132">响应</span><span class="sxs-lookup"><span data-stu-id="22d08-132">Response</span></span>

<span data-ttu-id="22d08-133">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="22d08-133">If successful, this method returns a `200 OK` response code and a collection of [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22d08-134">示例</span><span class="sxs-lookup"><span data-stu-id="22d08-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="22d08-135">请求</span><span class="sxs-lookup"><span data-stu-id="22d08-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="22d08-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="22d08-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/16d424f6-0100-4bf1-9ebc-fe009c5e5006/instances/bb14c722-51b8-4962-9bd2-1d96ba773d80/decisions
```
# <a name="c"></a>[<span data-ttu-id="22d08-137">C#</span><span class="sxs-lookup"><span data-stu-id="22d08-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22d08-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22d08-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22d08-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22d08-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22d08-140">Java</span><span class="sxs-lookup"><span data-stu-id="22d08-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="22d08-141">响应</span><span class="sxs-lookup"><span data-stu-id="22d08-141">Response</span></span>
><span data-ttu-id="22d08-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="22d08-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewInstanceDecisionItem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('16d424f6-0100-4bf1-9ebc-fe009c5e5006')/instances('bb14c722-51b8-4962-9bd2-1d96ba773d80')/decisions",
    "@odata.count": 1,
    "value": [
        {
            "id": "bfbd4d74-275c-4368-aaa1-06c93838d0d5",
            "accessReviewId": "bb14c722-51b8-4962-9bd2-1d96ba773d80",
            "reviewedDateTime": "2021-05-05T16:48:28.79Z",
            "decision": "Deny",
            "justification": "bye alexxxxx",
            "appliedDateTime": "2021-05-05T16:50:30.9Z",
            "applyResult": "AppliedSuccessfully",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/540da31b-4d25-4934-b7f7-98bc230eb15a",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "ff15bedb-22de-49ad-b2d7-59656607484d",
                "displayName": "group owner",
                "userPrincipalName": "group owner"
            },
            "appliedBy": {
                "id": "8798d204-fa3c-4d7b-977d-bc939b8a0848",
                "displayName": "Access Reviews",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "540da31b-4d25-4934-b7f7-98bc230eb15a",
                "userDisplayName": "Alex Wilber",
                "userPrincipalName": "AlexW@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "540da31b-4d25-4934-b7f7-98bc230eb15a",
                "displayName": "Alex Wilber",
                "userPrincipalName": "AlexW@contoso.com"
            }
        }
    ]
}
```
