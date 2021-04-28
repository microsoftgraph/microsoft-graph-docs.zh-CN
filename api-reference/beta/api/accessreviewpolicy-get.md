---
title: 获取 accessReviewPolicy
description: 读取 accessReviewPolicy 对象的属性和关系。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 05b6cbae21ea3a40b179d646feaeb9ff243f0a81
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067845"
---
# <a name="get-accessreviewpolicy"></a><span data-ttu-id="d0b4a-103">获取 accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="d0b4a-103">Get accessReviewPolicy</span></span>
<span data-ttu-id="d0b4a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0b4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0b4a-105">读取 [accessReviewPolicy](../resources/accessreviewpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d0b4a-105">Read the properties and relationships of an [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0b4a-106">权限</span><span class="sxs-lookup"><span data-stu-id="d0b4a-106">Permissions</span></span>
<span data-ttu-id="d0b4a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0b4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0b4a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0b4a-109">Permission type</span></span>|<span data-ttu-id="d0b4a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0b4a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0b4a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0b4a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d0b4a-112">Policy.Read.All、Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="d0b4a-112">Policy.Read.All, Policy.ReadWrite.AccessReviews</span></span>|
|<span data-ttu-id="d0b4a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0b4a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0b4a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0b4a-114">Not supported.</span></span>|
|<span data-ttu-id="d0b4a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0b4a-115">Application</span></span>|<span data-ttu-id="d0b4a-116">Policy.Read.All、Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="d0b4a-116">Policy.Read.All, Policy.ReadWrite.AccessReviews</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0b4a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0b4a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/accessReviewPolicy
GET /identityGovernance/accessReviews/policy
```

## <a name="request-headers"></a><span data-ttu-id="d0b4a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0b4a-118">Request headers</span></span>
|<span data-ttu-id="d0b4a-119">名称</span><span class="sxs-lookup"><span data-stu-id="d0b4a-119">Name</span></span>|<span data-ttu-id="d0b4a-120">说明</span><span class="sxs-lookup"><span data-stu-id="d0b4a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d0b4a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0b4a-121">Authorization</span></span>|<span data-ttu-id="d0b4a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d0b4a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0b4a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0b4a-124">Request body</span></span>
<span data-ttu-id="d0b4a-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d0b4a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0b4a-126">响应</span><span class="sxs-lookup"><span data-stu-id="d0b4a-126">Response</span></span>

<span data-ttu-id="d0b4a-127">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewPolicy](../resources/accessreviewpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0b4a-127">If successful, this method returns a `200 OK` response code and an [accessReviewPolicy](../resources/accessreviewpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d0b4a-128">示例</span><span class="sxs-lookup"><span data-stu-id="d0b4a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d0b4a-129">请求</span><span class="sxs-lookup"><span data-stu-id="d0b4a-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accessreviewpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/accessReviewPolicy
```


### <a name="response"></a><span data-ttu-id="d0b4a-130">响应</span><span class="sxs-lookup"><span data-stu-id="d0b4a-130">Response</span></span>
<span data-ttu-id="d0b4a-131">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d0b4a-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.accessReviewPolicy",
    "displayName": "Access Review Policy",
    "description": "Policy contains directory-level access review settings.",
    "isGroupOwnerManagementEnabled": false
  }
}
```

### <a name="request"></a><span data-ttu-id="d0b4a-132">请求</span><span class="sxs-lookup"><span data-stu-id="d0b4a-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accessreviewpolicy_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/policy
```


### <a name="response"></a><span data-ttu-id="d0b4a-133">响应</span><span class="sxs-lookup"><span data-stu-id="d0b4a-133">Response</span></span>
<span data-ttu-id="d0b4a-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d0b4a-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.accessReviewPolicy",
    "displayName": "Access Review Policy",
    "description": "Policy contains directory-level access review settings.",
    "isGroupOwnerManagementEnabled": false
  }
}
```
