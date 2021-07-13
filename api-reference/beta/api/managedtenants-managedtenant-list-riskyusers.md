---
title: 列出 riskyUsers
description: 获取 riskyUser 对象及其属性的列表。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 5c1f16969df71d9da8844fca7ff3a905a23a8838
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402379"
---
# <a name="list-riskyusers"></a><span data-ttu-id="7254d-103">列出 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="7254d-103">List riskyUsers</span></span>
<span data-ttu-id="7254d-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="7254d-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7254d-105">获取 [riskyUser](../resources/managedtenants-riskyuser.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="7254d-105">Get a list of the [riskyUser](../resources/managedtenants-riskyuser.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="7254d-106">权限</span><span class="sxs-lookup"><span data-stu-id="7254d-106">Permissions</span></span>
<span data-ttu-id="7254d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7254d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7254d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7254d-109">Permission type</span></span>|<span data-ttu-id="7254d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7254d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7254d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7254d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7254d-112">IdentityRiskyUser.Read.All、IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7254d-112">IdentityRiskyUser.Read.All, IdentityRiskyUser.ReadWrite.All</span></span>|
|<span data-ttu-id="7254d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7254d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7254d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7254d-114">Not supported.</span></span>|
|<span data-ttu-id="7254d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7254d-115">Application</span></span>|<span data-ttu-id="7254d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7254d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7254d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7254d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/riskyUsers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7254d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7254d-118">Optional query parameters</span></span>
<span data-ttu-id="7254d-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="7254d-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7254d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7254d-120">Request headers</span></span>
|<span data-ttu-id="7254d-121">名称</span><span class="sxs-lookup"><span data-stu-id="7254d-121">Name</span></span>|<span data-ttu-id="7254d-122">说明</span><span class="sxs-lookup"><span data-stu-id="7254d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7254d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7254d-123">Authorization</span></span>|<span data-ttu-id="7254d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7254d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7254d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7254d-126">Request body</span></span>
<span data-ttu-id="7254d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7254d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7254d-128">响应</span><span class="sxs-lookup"><span data-stu-id="7254d-128">Response</span></span>

<span data-ttu-id="7254d-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [riskyUser](../resources/managedtenants-riskyuser.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7254d-129">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/managedtenants-riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7254d-130">示例</span><span class="sxs-lookup"><span data-stu-id="7254d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7254d-131">请求</span><span class="sxs-lookup"><span data-stu-id="7254d-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/riskyUsers
```


### <a name="response"></a><span data-ttu-id="7254d-132">响应</span><span class="sxs-lookup"><span data-stu-id="7254d-132">Response</span></span>
><span data-ttu-id="7254d-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7254d-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.riskyUser)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyUsers",
  "value": [
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b_ae8d3a3f-be95-429c-8063-635ccc16e899",
      "userId": "ae8d3a3f-be95-429c-8063-635ccc16e899",
      "userDisplayName": "Cynthia Becker",
      "userPrincipalName": "cynthia@fourthcoffee002.onmicrosoft.com",
      "riskState": "atRisk",
      "riskLevel": "hidden",
      "riskDetail": "hidden",
      "isDeleted": false,
      "riskLastUpdatedDateTime": "2021-06-10T13:58:34.5171907Z",
      "lastRefreshedDateTime": "2021-07-11T11:32:55.2168558Z",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee"
    },
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320_05ec33c0-471d-4b1a-901c-093fc65c6401",
      "userId": "05ec33c0-471d-4b1a-901c-093fc65c6401",
      "userDisplayName": "Ina Anthony",
      "userPrincipalName": "ianthony@consolidatedmessenger001.onmicrosoft.com",
      "riskState": "atRisk",
      "riskLevel": "hidden",
      "riskDetail": "hidden",
      "isDeleted": false,
      "riskLastUpdatedDateTime": "2021-06-11T14:35:29.8061797Z",
      "lastRefreshedDateTime": "2021-07-11T14:42:10.8700665Z",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    }
  ]
}
```
