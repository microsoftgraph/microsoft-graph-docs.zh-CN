---
title: 获取 riskyUser
description: 读取 riskyUser 对象的属性和关系。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 523e5c3abe471ac2951615411c232517895dce64
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441388"
---
# <a name="get-riskyuser"></a><span data-ttu-id="428d5-103">获取 riskyUser</span><span class="sxs-lookup"><span data-stu-id="428d5-103">Get riskyUser</span></span>
<span data-ttu-id="428d5-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="428d5-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="428d5-105">读取 [riskyUser](../resources/managedtenants-riskyuser.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="428d5-105">Read the properties and relationships of a [riskyUser](../resources/managedtenants-riskyuser.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="428d5-106">权限</span><span class="sxs-lookup"><span data-stu-id="428d5-106">Permissions</span></span>
<span data-ttu-id="428d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="428d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="428d5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="428d5-109">Permission type</span></span>|<span data-ttu-id="428d5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="428d5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="428d5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="428d5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="428d5-112">IdentityRiskyUser.Read.All、IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="428d5-112">IdentityRiskyUser.Read.All, IdentityRiskyUser.ReadWrite.All</span></span>|
|<span data-ttu-id="428d5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="428d5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="428d5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="428d5-114">Not supported.</span></span>|
|<span data-ttu-id="428d5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="428d5-115">Application</span></span>|<span data-ttu-id="428d5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="428d5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="428d5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="428d5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/riskyUsers/{riskyUserId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="428d5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="428d5-118">Optional query parameters</span></span>
<span data-ttu-id="428d5-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="428d5-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="428d5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="428d5-120">Request headers</span></span>
|<span data-ttu-id="428d5-121">名称</span><span class="sxs-lookup"><span data-stu-id="428d5-121">Name</span></span>|<span data-ttu-id="428d5-122">说明</span><span class="sxs-lookup"><span data-stu-id="428d5-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="428d5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="428d5-123">Authorization</span></span>|<span data-ttu-id="428d5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="428d5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="428d5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="428d5-126">Request body</span></span>
<span data-ttu-id="428d5-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="428d5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="428d5-128">响应</span><span class="sxs-lookup"><span data-stu-id="428d5-128">Response</span></span>

<span data-ttu-id="428d5-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [riskyUser](../resources/managedtenants-riskyuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="428d5-129">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/managedtenants-riskyuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="428d5-130">示例</span><span class="sxs-lookup"><span data-stu-id="428d5-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="428d5-131">请求</span><span class="sxs-lookup"><span data-stu-id="428d5-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="428d5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="428d5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/riskyUsers/{riskyUserId}
```
# <a name="c"></a>[<span data-ttu-id="428d5-133">C#</span><span class="sxs-lookup"><span data-stu-id="428d5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="428d5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="428d5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="428d5-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="428d5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="428d5-136">Java</span><span class="sxs-lookup"><span data-stu-id="428d5-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="428d5-137">响应</span><span class="sxs-lookup"><span data-stu-id="428d5-137">Response</span></span>
><span data-ttu-id="428d5-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="428d5-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.riskyUser"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.riskyUser",
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
}
```
