---
title: 获取 accessReviewInstance
description: 读取 accessReviewInstance 对象的属性和关系。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8a8e2ec2ec059201dabea44523bf45ef054a4f3f
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031081"
---
# <a name="get-accessreviewinstance"></a><span data-ttu-id="d1cc0-103">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="d1cc0-103">Get accessReviewInstance</span></span>
<span data-ttu-id="d1cc0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1cc0-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="d1cc0-105">读取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d1cc0-105">Read the properties and relationships of an [accessReviewInstance](../resources/accessreviewinstance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1cc0-106">权限</span><span class="sxs-lookup"><span data-stu-id="d1cc0-106">Permissions</span></span>
<span data-ttu-id="d1cc0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1cc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1cc0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1cc0-109">Permission type</span></span>|<span data-ttu-id="d1cc0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1cc0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1cc0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1cc0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d1cc0-112">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1cc0-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="d1cc0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1cc0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1cc0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1cc0-114">Not supported.</span></span>|
|<span data-ttu-id="d1cc0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1cc0-115">Application</span></span>|<span data-ttu-id="d1cc0-116">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1cc0-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1cc0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1cc0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1cc0-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d1cc0-118">Optional query parameters</span></span>
<span data-ttu-id="d1cc0-119">此方法支持 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d1cc0-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="d1cc0-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d1cc0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1cc0-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1cc0-121">Request headers</span></span>
|<span data-ttu-id="d1cc0-122">名称</span><span class="sxs-lookup"><span data-stu-id="d1cc0-122">Name</span></span>|<span data-ttu-id="d1cc0-123">说明</span><span class="sxs-lookup"><span data-stu-id="d1cc0-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d1cc0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1cc0-124">Authorization</span></span>|<span data-ttu-id="d1cc0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d1cc0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1cc0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1cc0-127">Request body</span></span>
<span data-ttu-id="d1cc0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d1cc0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1cc0-129">响应</span><span class="sxs-lookup"><span data-stu-id="d1cc0-129">Response</span></span>

<span data-ttu-id="d1cc0-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewInstance](../resources/accessreviewinstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d1cc0-130">If successful, this method returns a `200 OK` response code and an [accessReviewInstance](../resources/accessreviewinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1cc0-131">示例</span><span class="sxs-lookup"><span data-stu-id="d1cc0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d1cc0-132">请求</span><span class="sxs-lookup"><span data-stu-id="d1cc0-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accessreviewinstance"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/12345ba0-cbf0-5678-8868-4444c7f4cc06
```


### <a name="response"></a><span data-ttu-id="d1cc0-133">响应</span><span class="sxs-lookup"><span data-stu-id="d1cc0-133">Response</span></span>
><span data-ttu-id="d1cc0-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d1cc0-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
