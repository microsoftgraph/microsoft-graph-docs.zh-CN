---
title: 列出租户
description: 获取租户对象及其属性的列表。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 2ffea17f39ee0db99b3b9aa964c73ccd5763f909
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440771"
---
# <a name="list-tenants"></a><span data-ttu-id="f44fe-103">列出租户</span><span class="sxs-lookup"><span data-stu-id="f44fe-103">List tenants</span></span>
<span data-ttu-id="f44fe-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="f44fe-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f44fe-105">获取租户对象 [及其](../resources/managedtenants-tenant.md) 属性的列表。</span><span class="sxs-lookup"><span data-stu-id="f44fe-105">Get a list of the [tenant](../resources/managedtenants-tenant.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="f44fe-106">权限</span><span class="sxs-lookup"><span data-stu-id="f44fe-106">Permissions</span></span>
<span data-ttu-id="f44fe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f44fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f44fe-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f44fe-109">Permission type</span></span>|<span data-ttu-id="f44fe-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f44fe-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f44fe-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f44fe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f44fe-112">ManagedTenants.Read.All、ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f44fe-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="f44fe-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f44fe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f44fe-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f44fe-114">Not supported.</span></span>|
|<span data-ttu-id="f44fe-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f44fe-115">Application</span></span>|<span data-ttu-id="f44fe-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f44fe-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f44fe-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f44fe-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f44fe-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f44fe-118">Optional query parameters</span></span>
<span data-ttu-id="f44fe-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="f44fe-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f44fe-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f44fe-120">Request headers</span></span>
|<span data-ttu-id="f44fe-121">名称</span><span class="sxs-lookup"><span data-stu-id="f44fe-121">Name</span></span>|<span data-ttu-id="f44fe-122">说明</span><span class="sxs-lookup"><span data-stu-id="f44fe-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f44fe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f44fe-123">Authorization</span></span>|<span data-ttu-id="f44fe-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f44fe-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f44fe-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f44fe-126">Request body</span></span>
<span data-ttu-id="f44fe-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f44fe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f44fe-128">响应</span><span class="sxs-lookup"><span data-stu-id="f44fe-128">Response</span></span>

<span data-ttu-id="f44fe-129">如果成功，此方法在响应正文中返回 响应代码 `200 OK` 和 [租户](../resources/managedtenants-tenant.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f44fe-129">If successful, this method returns a `200 OK` response code and a collection of [tenant](../resources/managedtenants-tenant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f44fe-130">示例</span><span class="sxs-lookup"><span data-stu-id="f44fe-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f44fe-131">请求</span><span class="sxs-lookup"><span data-stu-id="f44fe-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f44fe-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f44fe-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tenant"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenants
```
# <a name="c"></a>[<span data-ttu-id="f44fe-133">C#</span><span class="sxs-lookup"><span data-stu-id="f44fe-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tenant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f44fe-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f44fe-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tenant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f44fe-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f44fe-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tenant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f44fe-136">Java</span><span class="sxs-lookup"><span data-stu-id="f44fe-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tenant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f44fe-137">响应</span><span class="sxs-lookup"><span data-stu-id="f44fe-137">Response</span></span>
><span data-ttu-id="f44fe-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f44fe-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenant)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "contract": {
        "displayName": "Fourth Coffee",
        "defaultDomainName": "fourthcoffe01.onmicrosoft.com",
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
  ]
}
```
