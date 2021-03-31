---
title: 获取 appConsentRequest
description: 读取 appConsentRequest 对象的属性和关系。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f9dac66d1f8ce5d2625b0eca7e3307fb4ac02b56
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469529"
---
# <a name="get-appconsentrequest"></a><span data-ttu-id="0b324-103">获取 appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="0b324-103">Get appConsentRequest</span></span>

<span data-ttu-id="0b324-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b324-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b324-105">读取 [appConsentRequest](../resources/appconsentrequest.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0b324-105">Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b324-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0b324-106">Permissions</span></span>

<span data-ttu-id="0b324-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b324-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b324-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b324-109">Permission type</span></span>|<span data-ttu-id="0b324-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b324-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b324-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b324-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0b324-112">ConsentRequest.Read.All、ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b324-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="0b324-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b324-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b324-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b324-114">Not supported.</span></span>|
|<span data-ttu-id="0b324-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b324-115">Application</span></span>|<span data-ttu-id="0b324-116">ConsentRequest.Read.All、ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b324-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b324-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b324-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b324-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0b324-118">Optional query parameters</span></span>

<span data-ttu-id="0b324-119">此方法支持  `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0b324-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="0b324-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0b324-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b324-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b324-121">Request headers</span></span>

|<span data-ttu-id="0b324-122">名称</span><span class="sxs-lookup"><span data-stu-id="0b324-122">Name</span></span>|<span data-ttu-id="0b324-123">说明</span><span class="sxs-lookup"><span data-stu-id="0b324-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0b324-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b324-124">Authorization</span></span>|<span data-ttu-id="0b324-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b324-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b324-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b324-127">Request body</span></span>

<span data-ttu-id="0b324-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0b324-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b324-129">响应</span><span class="sxs-lookup"><span data-stu-id="0b324-129">Response</span></span>

<span data-ttu-id="0b324-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [appConsentRequest](../resources/appconsentrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0b324-130">If successful, this method returns a `200 OK` response code and an [appConsentRequest](../resources/appconsentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b324-131">示例</span><span class="sxs-lookup"><span data-stu-id="0b324-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0b324-132">请求</span><span class="sxs-lookup"><span data-stu-id="0b324-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_appconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/appConsent/appConsentRequests/af330b30-dd59-4482-a848-0fd81b0438ed
```

### <a name="response"></a><span data-ttu-id="0b324-133">响应</span><span class="sxs-lookup"><span data-stu-id="0b324-133">Response</span></span>

<span data-ttu-id="0b324-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b324-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appConsentRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests/$entity",
  "id": "af330b30-dd59-4482-a848-0fd81b0438ed",
  "appId": "3ca5f23f-94b4-4930-aec9-b8ca0f060e68",
  "appDisplayName": "Moodle",
  "pendingScopes": [],
  "userConsentRequests@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('af330b30-dd59-4482-a848-0fd81b0438ed')/userConsentRequests",
  "userConsentRequests": []
}
```
