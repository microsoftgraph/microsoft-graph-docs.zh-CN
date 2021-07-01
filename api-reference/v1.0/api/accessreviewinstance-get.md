---
title: 获取 accessReviewInstance
description: 读取 accessReviewInstance 对象的属性和关系。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 62d18407a457de2c335656800c12d2b311ea90b6
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210992"
---
# <a name="get-accessreviewinstance"></a><span data-ttu-id="de619-103">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="de619-103">Get accessReviewInstance</span></span>
<span data-ttu-id="de619-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de619-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="de619-105">读取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="de619-105">Read the properties and relationships of an [accessReviewInstance](../resources/accessreviewinstance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="de619-106">权限</span><span class="sxs-lookup"><span data-stu-id="de619-106">Permissions</span></span>
<span data-ttu-id="de619-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de619-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de619-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="de619-109">Permission type</span></span>|<span data-ttu-id="de619-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="de619-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de619-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de619-111">Delegated (work or school account)</span></span>|<span data-ttu-id="de619-112">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de619-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="de619-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de619-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de619-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="de619-114">Not supported.</span></span>|
|<span data-ttu-id="de619-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="de619-115">Application</span></span>|<span data-ttu-id="de619-116">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de619-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de619-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de619-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de619-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="de619-118">Optional query parameters</span></span>
<span data-ttu-id="de619-119">此方法支持 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="de619-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="de619-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="de619-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="de619-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="de619-121">Request headers</span></span>
|<span data-ttu-id="de619-122">名称</span><span class="sxs-lookup"><span data-stu-id="de619-122">Name</span></span>|<span data-ttu-id="de619-123">说明</span><span class="sxs-lookup"><span data-stu-id="de619-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="de619-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="de619-124">Authorization</span></span>|<span data-ttu-id="de619-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="de619-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de619-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="de619-127">Request body</span></span>
<span data-ttu-id="de619-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="de619-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de619-129">响应</span><span class="sxs-lookup"><span data-stu-id="de619-129">Response</span></span>

<span data-ttu-id="de619-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewInstance](../resources/accessreviewinstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="de619-130">If successful, this method returns a `200 OK` response code and an [accessReviewInstance](../resources/accessreviewinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de619-131">示例</span><span class="sxs-lookup"><span data-stu-id="de619-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de619-132">请求</span><span class="sxs-lookup"><span data-stu-id="de619-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="de619-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="de619-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewinstance"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/12345ba0-cbf0-5678-8868-4444c7f4cc06
```
# <a name="c"></a>[<span data-ttu-id="de619-134">C#</span><span class="sxs-lookup"><span data-stu-id="de619-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de619-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de619-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de619-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de619-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="de619-137">Java</span><span class="sxs-lookup"><span data-stu-id="de619-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="de619-138">响应</span><span class="sxs-lookup"><span data-stu-id="de619-138">Response</span></span>
><span data-ttu-id="de619-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="de619-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.accessReviewInstance",
    "id": "d7fbc019-c019-d7fb-19c0-fbd719c0fbd7",
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
}
```
