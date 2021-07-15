---
title: 列出 aggregatedPolicyCompliances
description: 获取聚合PolicyCompliance 对象及其属性的列表。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 160292f38035390d7b5ed769bbea42847bba71b2
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441520"
---
# <a name="list-aggregatedpolicycompliances"></a><span data-ttu-id="8aff6-103">列出 aggregatedPolicyCompliances</span><span class="sxs-lookup"><span data-stu-id="8aff6-103">List aggregatedPolicyCompliances</span></span>
<span data-ttu-id="8aff6-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="8aff6-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aff6-105">获取聚合 [PolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="8aff6-105">Get a list of the [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="8aff6-106">权限</span><span class="sxs-lookup"><span data-stu-id="8aff6-106">Permissions</span></span>
<span data-ttu-id="8aff6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8aff6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8aff6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8aff6-109">Permission type</span></span>|<span data-ttu-id="8aff6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8aff6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8aff6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8aff6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8aff6-112">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8aff6-112">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8aff6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8aff6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8aff6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8aff6-114">Not supported.</span></span>|
|<span data-ttu-id="8aff6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8aff6-115">Application</span></span>|<span data-ttu-id="8aff6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8aff6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8aff6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8aff6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/aggregatedPolicyCompliances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8aff6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8aff6-118">Optional query parameters</span></span>
<span data-ttu-id="8aff6-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="8aff6-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8aff6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8aff6-120">Request headers</span></span>
|<span data-ttu-id="8aff6-121">名称</span><span class="sxs-lookup"><span data-stu-id="8aff6-121">Name</span></span>|<span data-ttu-id="8aff6-122">说明</span><span class="sxs-lookup"><span data-stu-id="8aff6-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8aff6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8aff6-123">Authorization</span></span>|<span data-ttu-id="8aff6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8aff6-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8aff6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8aff6-126">Request body</span></span>
<span data-ttu-id="8aff6-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8aff6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8aff6-128">响应</span><span class="sxs-lookup"><span data-stu-id="8aff6-128">Response</span></span>

<span data-ttu-id="8aff6-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [聚合PolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8aff6-129">If successful, this method returns a `200 OK` response code and a collection of [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8aff6-130">示例</span><span class="sxs-lookup"><span data-stu-id="8aff6-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8aff6-131">请求</span><span class="sxs-lookup"><span data-stu-id="8aff6-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8aff6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8aff6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_aggregatedpolicycompliance"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/aggregatedPolicyCompliances
```
# <a name="c"></a>[<span data-ttu-id="8aff6-133">C#</span><span class="sxs-lookup"><span data-stu-id="8aff6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-aggregatedpolicycompliance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8aff6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8aff6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-aggregatedpolicycompliance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8aff6-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8aff6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-aggregatedpolicycompliance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8aff6-136">Java</span><span class="sxs-lookup"><span data-stu-id="8aff6-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-aggregatedpolicycompliance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8aff6-137">响应</span><span class="sxs-lookup"><span data-stu-id="8aff6-137">Response</span></span>
><span data-ttu-id="8aff6-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8aff6-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.aggregatedPolicyCompliance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#aggregatedPolicyCompliances",
  "value": [
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b_19a8d6a6-d87e-4059-85b3-c73bfc5cea15",
      "compliancePolicyId": "19a8d6a6-d87e-4059-85b3-c73bfc5cea15",
      "compliancePolicyName": "Baseline - Setup Compliance Policy for Windows devices",
      "compliancePolicyType": "Unknown",
      "compliancePolicyPlatform": "Windows10",
      "numberOfCompliantDevices": 0,
      "numberOfNonCompliantDevices": 0,
      "numberOfErrorDevices": 0,
      "policyModifiedDateTime": "2021-06-22T17:01:46Z",
      "lastRefreshedDateTime": "2021-07-11T01:02:33.4452876Z",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee"
    },
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b_3e4b612f-5ce0-42f6-9e21-a172adc5100d",
      "compliancePolicyId": "3e4b612f-5ce0-42f6-9e21-a172adc5100d",
      "compliancePolicyName": "Windows Level 2 Compliance Policy",
      "compliancePolicyType": "Unknown",
      "compliancePolicyPlatform": "Windows10",
      "numberOfCompliantDevices": 4,
      "numberOfNonCompliantDevices": 0,
      "numberOfErrorDevices": 0,
      "policyModifiedDateTime": "2021-04-20T22:27:20Z",
      "lastRefreshedDateTime": "2021-07-11T01:02:33.4452876Z",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee"
    }
  ]
}
```
