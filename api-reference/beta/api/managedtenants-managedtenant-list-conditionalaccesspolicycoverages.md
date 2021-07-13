---
title: 列出 conditionalAccessPolicyCoverages
description: 获取 conditionalAccessPolicyCoverage 对象及其属性的列表。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 633a909778182a6da2ea04d9e37484db3cfdc286
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402028"
---
# <a name="list-conditionalaccesspolicycoverages"></a><span data-ttu-id="0657c-103">列出 conditionalAccessPolicyCoverages</span><span class="sxs-lookup"><span data-stu-id="0657c-103">List conditionalAccessPolicyCoverages</span></span>
<span data-ttu-id="0657c-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="0657c-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0657c-105">获取 [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="0657c-105">Get a list of the [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) objects and their properties.</span></span> <span data-ttu-id="0657c-106">使用此操作可列出Azure Active Directory多租户管理平台管理的所有租户中的条件访问策略覆盖范围。</span><span class="sxs-lookup"><span data-stu-id="0657c-106">Use this operation to list of Azure Active Directory conditional access policy coverage across all tenants that are being managed by the multi-tenant management platform.</span></span>

## <a name="permissions"></a><span data-ttu-id="0657c-107">权限</span><span class="sxs-lookup"><span data-stu-id="0657c-107">Permissions</span></span>
<span data-ttu-id="0657c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0657c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0657c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0657c-110">Permission type</span></span>|<span data-ttu-id="0657c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0657c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0657c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0657c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0657c-113">Policy.Read.All、Policy.ReadWrite.ConditionalAccess 和 Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="0657c-113">Policy.Read.All, Policy.ReadWrite.ConditionalAccess, and Application.Read.All</span></span>|
|<span data-ttu-id="0657c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0657c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0657c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0657c-115">Not supported.</span></span>|
|<span data-ttu-id="0657c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0657c-116">Application</span></span>|<span data-ttu-id="0657c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0657c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0657c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0657c-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/conditionalAccessPolicyCoverages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0657c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0657c-119">Optional query parameters</span></span>
<span data-ttu-id="0657c-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="0657c-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0657c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0657c-121">Request headers</span></span>
|<span data-ttu-id="0657c-122">名称</span><span class="sxs-lookup"><span data-stu-id="0657c-122">Name</span></span>|<span data-ttu-id="0657c-123">说明</span><span class="sxs-lookup"><span data-stu-id="0657c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0657c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0657c-124">Authorization</span></span>|<span data-ttu-id="0657c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0657c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0657c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0657c-127">Request body</span></span>
<span data-ttu-id="0657c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0657c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0657c-129">响应</span><span class="sxs-lookup"><span data-stu-id="0657c-129">Response</span></span>

<span data-ttu-id="0657c-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0657c-130">If successful, this method returns a `200 OK` response code and a collection of [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0657c-131">示例</span><span class="sxs-lookup"><span data-stu-id="0657c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0657c-132">请求</span><span class="sxs-lookup"><span data-stu-id="0657c-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_conditionalaccesspolicycoverage"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/conditionalAccessPolicyCoverages
```


### <a name="response"></a><span data-ttu-id="0657c-133">响应</span><span class="sxs-lookup"><span data-stu-id="0657c-133">Response</span></span>
><span data-ttu-id="0657c-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0657c-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.conditionalAccessPolicyCoverage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
      "id": "38227791-a88b-4fcc-81c5-58cf77668320",
      "conditionalAccessPolicyState": "enabled",
      "requiresDeviceCompliance": false,
      "latestPolicyModifiedDateTime": "2021-07-11T14:56:13.598304Z",
      "tenantDisplayName": "Consolidated Messenger"
    }
  ]
}
```
