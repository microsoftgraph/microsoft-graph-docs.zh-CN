---
title: 获取 accessReviewInstanceDecisionItem
description: 读取 accessReviewInstanceDecisionItem 对象的属性和关系。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2f72596f4f89fe71f6d7cee310e721dd230357ee
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209725"
---
# <a name="get-accessreviewinstancedecisionitem"></a><span data-ttu-id="d32d7-103">获取 accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="d32d7-103">Get accessReviewInstanceDecisionItem</span></span>
<span data-ttu-id="d32d7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d32d7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d32d7-105">读取 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d32d7-105">Read the properties and relationships of an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d32d7-106">权限</span><span class="sxs-lookup"><span data-stu-id="d32d7-106">Permissions</span></span>
<span data-ttu-id="d32d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d32d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d32d7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d32d7-109">Permission type</span></span>|<span data-ttu-id="d32d7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d32d7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d32d7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d32d7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d32d7-112">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d32d7-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="d32d7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d32d7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d32d7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d32d7-114">Not supported.</span></span>|
|<span data-ttu-id="d32d7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d32d7-115">Application</span></span>|<span data-ttu-id="d32d7-116">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d32d7-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d32d7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d32d7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d32d7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d32d7-118">Optional query parameters</span></span>
<span data-ttu-id="d32d7-119">此方法支持 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d32d7-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="d32d7-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d32d7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d32d7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d32d7-121">Request headers</span></span>
|<span data-ttu-id="d32d7-122">名称</span><span class="sxs-lookup"><span data-stu-id="d32d7-122">Name</span></span>|<span data-ttu-id="d32d7-123">说明</span><span class="sxs-lookup"><span data-stu-id="d32d7-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d32d7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d32d7-124">Authorization</span></span>|<span data-ttu-id="d32d7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d32d7-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d32d7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d32d7-127">Request body</span></span>
<span data-ttu-id="d32d7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d32d7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d32d7-129">响应</span><span class="sxs-lookup"><span data-stu-id="d32d7-129">Response</span></span>

<span data-ttu-id="d32d7-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d32d7-130">If successful, this method returns a `200 OK` response code and an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d32d7-131">示例</span><span class="sxs-lookup"><span data-stu-id="d32d7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d32d7-132">请求</span><span class="sxs-lookup"><span data-stu-id="d32d7-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d32d7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d32d7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/instances/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/decisions/9550e25b-f315-4454-9d87-16b885c35de4
```
# <a name="c"></a>[<span data-ttu-id="d32d7-134">C#</span><span class="sxs-lookup"><span data-stu-id="d32d7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d32d7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d32d7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d32d7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d32d7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d32d7-137">Java</span><span class="sxs-lookup"><span data-stu-id="d32d7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d32d7-138">响应</span><span class="sxs-lookup"><span data-stu-id="d32d7-138">Response</span></span>
><span data-ttu-id="d32d7-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d32d7-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd')/instances('7070ea1c-8d12-457b-bd35-a37dc59e54e0')/decisions/$entity",
    "id": "9550e25b-f315-4454-9d87-16b885c35de4",
    "accessReviewId": "7070ea1c-8d12-457b-bd35-a37dc59e54e0",
    "reviewedDateTime": null,
    "decision": "NotReviewed",
    "justification": "",
    "appliedDateTime": null,
    "applyResult": "New",
    "recommendation": "Deny",
    "principalLink": "https://graph.microsoft.com/v1.0/users/1800bb2c-955d-4205-8471-3a6c3116435d",
    "resourceLink": null,
    "resource": null,
    "reviewedBy": {
        "id": "00000000-0000-0000-0000-000000000000",
        "displayName": "",
        "userPrincipalName": ""
    },
    "appliedBy": {
        "id": "00000000-0000-0000-0000-000000000000",
        "displayName": "",
        "userPrincipalName": ""
    },
    "target": {
        "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
        "userId": "1800bb2c-955d-4205-8471-3a6c3116435d",
        "userDisplayName": "guest example",
        "userPrincipalName": "guest@guest.com"
    },
    "principal": {
        "@odata.type": "#microsoft.graph.userIdentity",
        "id": "1800bb2c-955d-4205-8471-3a6c3116435d",
        "displayName": "guest example",
        "userPrincipalName": "guest@guest.com"
    }
}
```
