---
title: 获取 accessReviewInstanceDecisionItem
description: 读取 accessReviewInstanceDecisionItem 对象的属性和关系。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7354b9eba451c7ea19aac4def869fad4a31e4346
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207426"
---
# <a name="get-accessreviewinstancedecisionitem"></a><span data-ttu-id="47940-103">获取 accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="47940-103">Get accessReviewInstanceDecisionItem</span></span>
<span data-ttu-id="47940-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47940-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47940-105">读取 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="47940-105">Read the properties and relationships of an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="47940-106">权限</span><span class="sxs-lookup"><span data-stu-id="47940-106">Permissions</span></span>
<span data-ttu-id="47940-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47940-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47940-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="47940-109">Permission type</span></span>|<span data-ttu-id="47940-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="47940-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47940-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47940-111">Delegated (work or school account)</span></span>|<span data-ttu-id="47940-112">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47940-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="47940-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47940-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47940-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="47940-114">Not supported.</span></span>|
|<span data-ttu-id="47940-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="47940-115">Application</span></span>|<span data-ttu-id="47940-116">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47940-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47940-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47940-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47940-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="47940-118">Optional query parameters</span></span>
<span data-ttu-id="47940-119">此方法支持 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="47940-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="47940-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="47940-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="47940-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="47940-121">Request headers</span></span>
|<span data-ttu-id="47940-122">名称</span><span class="sxs-lookup"><span data-stu-id="47940-122">Name</span></span>|<span data-ttu-id="47940-123">说明</span><span class="sxs-lookup"><span data-stu-id="47940-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="47940-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="47940-124">Authorization</span></span>|<span data-ttu-id="47940-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="47940-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47940-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="47940-127">Request body</span></span>
<span data-ttu-id="47940-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="47940-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47940-129">响应</span><span class="sxs-lookup"><span data-stu-id="47940-129">Response</span></span>

<span data-ttu-id="47940-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="47940-130">If successful, this method returns a `200 OK` response code and an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47940-131">示例</span><span class="sxs-lookup"><span data-stu-id="47940-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47940-132">请求</span><span class="sxs-lookup"><span data-stu-id="47940-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="47940-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="47940-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0/instances/6444d4fd-ab55-4608-8cf9-c6702d172bcc/decisions/e6cafba0-cbf0-4748-8868-0810c7f4cc06
```
# <a name="c"></a>[<span data-ttu-id="47940-134">C#</span><span class="sxs-lookup"><span data-stu-id="47940-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47940-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47940-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47940-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47940-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47940-137">Java</span><span class="sxs-lookup"><span data-stu-id="47940-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="47940-138">响应</span><span class="sxs-lookup"><span data-stu-id="47940-138">Response</span></span>
><span data-ttu-id="47940-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="47940-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0')/instances('6444d4fd-ab55-4608-8cf9-c6702d172bcc')/decisions/$entity",
    "id": "e6cafba0-cbf0-4748-8868-0810c7f4cc06",
    "accessReviewId": "6444d4fd-ab55-4608-8cf9-c6702d172bcc",
    "reviewedDateTime": null,
    "decision": "NotReviewed",
    "justification": "",
    "appliedDateTime": null,
    "applyResult": "New",
    "recommendation": "Approve",
    "principalLink": "https://graph.microsoft.com/v1.0/users/04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
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
        "userId": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
        "userDisplayName": "Diego Siciliani",
        "userPrincipalName": "DiegoS@contoso.com"
    },
    "principal": {
        "@odata.type": "#microsoft.graph.userIdentity",
        "id": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
        "displayName": "Diego Siciliani",
        "userPrincipalName": "DiegoS@contoso.com"
    }
}
```
