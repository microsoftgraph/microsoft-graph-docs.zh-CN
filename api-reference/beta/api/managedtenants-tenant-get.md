---
title: 获取租户
description: 读取租户对象的属性和关系。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 82224f7a6c188c4a97fd6c20f97135ceb20ca192
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442483"
---
# <a name="get-tenant"></a><span data-ttu-id="9ecfa-103">获取租户</span><span class="sxs-lookup"><span data-stu-id="9ecfa-103">Get tenant</span></span>
<span data-ttu-id="9ecfa-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="9ecfa-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ecfa-105">读取租户对象的属性 [和](../resources/managedtenants-tenant.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="9ecfa-105">Read the properties and relationships of a [tenant](../resources/managedtenants-tenant.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ecfa-106">权限</span><span class="sxs-lookup"><span data-stu-id="9ecfa-106">Permissions</span></span>
<span data-ttu-id="9ecfa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ecfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ecfa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ecfa-109">Permission type</span></span>|<span data-ttu-id="9ecfa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ecfa-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ecfa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ecfa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9ecfa-112">ManagedTenants.Read.All、ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ecfa-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="9ecfa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ecfa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ecfa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ecfa-114">Not supported.</span></span>|
|<span data-ttu-id="9ecfa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ecfa-115">Application</span></span>|<span data-ttu-id="9ecfa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ecfa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ecfa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ecfa-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenants/{tenantId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ecfa-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9ecfa-118">Optional query parameters</span></span>
<span data-ttu-id="9ecfa-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="9ecfa-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ecfa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ecfa-120">Request headers</span></span>
|<span data-ttu-id="9ecfa-121">名称</span><span class="sxs-lookup"><span data-stu-id="9ecfa-121">Name</span></span>|<span data-ttu-id="9ecfa-122">说明</span><span class="sxs-lookup"><span data-stu-id="9ecfa-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9ecfa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ecfa-123">Authorization</span></span>|<span data-ttu-id="9ecfa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9ecfa-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ecfa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ecfa-126">Request body</span></span>
<span data-ttu-id="9ecfa-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9ecfa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ecfa-128">响应</span><span class="sxs-lookup"><span data-stu-id="9ecfa-128">Response</span></span>

<span data-ttu-id="9ecfa-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应[](../resources/managedtenants-tenant.md)代码和租户对象。</span><span class="sxs-lookup"><span data-stu-id="9ecfa-129">If successful, this method returns a `200 OK` response code and a [tenant](../resources/managedtenants-tenant.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ecfa-130">示例</span><span class="sxs-lookup"><span data-stu-id="9ecfa-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9ecfa-131">请求</span><span class="sxs-lookup"><span data-stu-id="9ecfa-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9ecfa-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ecfa-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tenant"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenants/{tenantId}
```
# <a name="c"></a>[<span data-ttu-id="9ecfa-133">C#</span><span class="sxs-lookup"><span data-stu-id="9ecfa-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tenant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ecfa-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ecfa-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tenant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ecfa-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ecfa-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tenant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ecfa-136">Java</span><span class="sxs-lookup"><span data-stu-id="9ecfa-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tenant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9ecfa-137">响应</span><span class="sxs-lookup"><span data-stu-id="9ecfa-137">Response</span></span>
><span data-ttu-id="9ecfa-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9ecfa-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenant"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.tenant",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b",
  "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
  "contract": {
    "displayName": "Fourth Coffee",
    "defaultDomainName": "fourthcoffe001.onmicrosoft.com",
    "contractType": 2
  },
  "tenantStatusInformation": {
    "onboardingStatus": "ineligible",
    "onboardingDateTime": "2012-02-20T00:00:00Z",
    "onboardedByUserId": "",
    "offboardedDateTime": "2012-02-20T00:00:00Z",
    "offboardedBy": "",
    "delegatedPrivilegeStatus": "delegatedAdminPrivileges",
    "workloadStatuses": [
      {
        "displayName": "Device Management",
        "onboardingStatus": "onboarded",
        "onboardedDateTime": "2012-02-20T00:00:00Z",
        "offboardedDateTime": null
      },
      {
        "displayName": "Cloud PC",
        "onboardingStatus": "notOnboarded",
        "onboardedDateTime": "2012-02-20T00:00:00Z",
        "offboardedDateTime": null
      }
    ]
  },
  "createdDateTime": "2012-02-20T00:00:00Z",
  "lastUpdatedDatetime": "2021-02-20T00:00:00Z"
}
```
