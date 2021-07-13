---
title: 列出 credentialUserRegistrationsSummaries
description: 获取 credentialUserRegistrationsSummary 对象及其属性的列表。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: fcb42f7c00a518e270d4e937156e1e6f39b4b692
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402034"
---
# <a name="list-credentialuserregistrationssummaries"></a><span data-ttu-id="5af81-103">列出 credentialUserRegistrationsSummaries</span><span class="sxs-lookup"><span data-stu-id="5af81-103">List credentialUserRegistrationsSummaries</span></span>
<span data-ttu-id="5af81-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="5af81-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5af81-105">获取 [credentialUserRegistrationsSummary 对象](../resources/managedtenants-credentialuserregistrationssummary.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="5af81-105">Get a list of the [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="5af81-106">权限</span><span class="sxs-lookup"><span data-stu-id="5af81-106">Permissions</span></span>
<span data-ttu-id="5af81-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5af81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5af81-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5af81-109">Permission type</span></span>|<span data-ttu-id="5af81-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5af81-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5af81-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5af81-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5af81-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5af81-112">Reports.Read.All</span></span>|
|<span data-ttu-id="5af81-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5af81-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5af81-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5af81-114">Not supported.</span></span>|
|<span data-ttu-id="5af81-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5af81-115">Application</span></span>|<span data-ttu-id="5af81-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5af81-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5af81-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5af81-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/credentialUserRegistrationsSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5af81-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5af81-118">Optional query parameters</span></span>
<span data-ttu-id="5af81-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="5af81-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5af81-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5af81-120">Request headers</span></span>
|<span data-ttu-id="5af81-121">名称</span><span class="sxs-lookup"><span data-stu-id="5af81-121">Name</span></span>|<span data-ttu-id="5af81-122">说明</span><span class="sxs-lookup"><span data-stu-id="5af81-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5af81-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5af81-123">Authorization</span></span>|<span data-ttu-id="5af81-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5af81-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5af81-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5af81-126">Request body</span></span>
<span data-ttu-id="5af81-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5af81-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5af81-128">响应</span><span class="sxs-lookup"><span data-stu-id="5af81-128">Response</span></span>

<span data-ttu-id="5af81-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5af81-129">If successful, this method returns a `200 OK` response code and a collection of [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5af81-130">示例</span><span class="sxs-lookup"><span data-stu-id="5af81-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5af81-131">请求</span><span class="sxs-lookup"><span data-stu-id="5af81-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_credentialuserregistrationssummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/credentialUserRegistrationsSummaries
```


### <a name="response"></a><span data-ttu-id="5af81-132">响应</span><span class="sxs-lookup"><span data-stu-id="5af81-132">Response</span></span>
><span data-ttu-id="5af81-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5af81-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.credentialUserRegistrationsSummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#credentialUserRegistrationsSummaries",
  "value": [
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320",
      "mfaAndSsprCapableUserCount": 2,
      "ssprEnabledUserCount": 9,
      "mfaRegisteredUserCount": 3,
      "ssprRegisteredUserCount": 2,
      "totalUserCount": 9,
      "securityDefaultsEnabled": false,
      "mfaConditionalAccessPolicyState": "enabled",
      "lastRefreshedDateTime": "2021-07-11T09:58:11.5730661Z",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    },
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b",
      "mfaAndSsprCapableUserCount": 0,
      "ssprEnabledUserCount": 1,
      "mfaRegisteredUserCount": 0,
      "ssprRegisteredUserCount": 0,
      "totalUserCount": 7,
      "securityDefaultsEnabled": false,
      "mfaConditionalAccessPolicyState": "enabledForReportingButNotEnforced",
      "lastRefreshedDateTime": "2021-07-11T11:15:52.9375367Z",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee"
    }
  ]
}
```
