---
title: 获取 conditionalAccessPolicyCoverage
description: 读取 conditionalAccessPolicyCoverage 对象的属性和关系。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 0283b41d7576cef1228861db168dbd5e3a3bb511
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402050"
---
# <a name="get-conditionalaccesspolicycoverage"></a><span data-ttu-id="e4bdb-103">获取 conditionalAccessPolicyCoverage</span><span class="sxs-lookup"><span data-stu-id="e4bdb-103">Get conditionalAccessPolicyCoverage</span></span>
<span data-ttu-id="e4bdb-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="e4bdb-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4bdb-105">读取 [conditionalAccessPolicyCoverage 对象的属性和](../resources/managedtenants-conditionalaccesspolicycoverage.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="e4bdb-105">Read the properties and relationships of a [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4bdb-106">权限</span><span class="sxs-lookup"><span data-stu-id="e4bdb-106">Permissions</span></span>
<span data-ttu-id="e4bdb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4bdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4bdb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4bdb-109">Permission type</span></span>|<span data-ttu-id="e4bdb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4bdb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4bdb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4bdb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e4bdb-112">Policy.Read.All、Policy.ReadWrite.ConditionalAccess 和 Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4bdb-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess, and Application.Read.All</span></span>|
|<span data-ttu-id="e4bdb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4bdb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4bdb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4bdb-114">Not supported.</span></span>|
|<span data-ttu-id="e4bdb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4bdb-115">Application</span></span>|<span data-ttu-id="e4bdb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4bdb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4bdb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4bdb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/conditionalAccessPolicyCoverages/{conditionalAccessPolicyCoverageId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4bdb-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e4bdb-118">Optional query parameters</span></span>
<span data-ttu-id="e4bdb-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="e4bdb-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4bdb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4bdb-120">Request headers</span></span>
|<span data-ttu-id="e4bdb-121">名称</span><span class="sxs-lookup"><span data-stu-id="e4bdb-121">Name</span></span>|<span data-ttu-id="e4bdb-122">说明</span><span class="sxs-lookup"><span data-stu-id="e4bdb-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e4bdb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4bdb-123">Authorization</span></span>|<span data-ttu-id="e4bdb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e4bdb-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4bdb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4bdb-126">Request body</span></span>
<span data-ttu-id="e4bdb-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e4bdb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4bdb-128">响应</span><span class="sxs-lookup"><span data-stu-id="e4bdb-128">Response</span></span>

<span data-ttu-id="e4bdb-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e4bdb-129">If successful, this method returns a `200 OK` response code and a [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e4bdb-130">示例</span><span class="sxs-lookup"><span data-stu-id="e4bdb-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e4bdb-131">请求</span><span class="sxs-lookup"><span data-stu-id="e4bdb-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conditionalaccesspolicycoverage"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/conditionalAccessPolicyCoverages/{conditionalAccessPolicyCoverageId}
```


### <a name="response"></a><span data-ttu-id="e4bdb-132">响应</span><span class="sxs-lookup"><span data-stu-id="e4bdb-132">Response</span></span>
><span data-ttu-id="e4bdb-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e4bdb-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.conditionalAccessPolicyCoverage"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
  "id": "38227791-a88b-4fcc-81c5-58cf77668320",
  "conditionalAccessPolicyState": "enabled",
  "requiresDeviceCompliance": false,
  "latestPolicyModifiedDateTime": "2021-07-11T14:56:13.598304Z",
  "tenantDisplayName": "Consolidated Messenger"
}
```
