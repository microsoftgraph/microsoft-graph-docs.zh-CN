---
title: tenant： offboardTenant
description: 执行适当的过程以从多租户管理平台中删除托管租户。 商业和委派管理权限等关系不会受到影响。 通过调用此操作进行的唯一更改是租户从多租户管理平台取消设置。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: d6d4d07c7af19299e679275354206bc55da3ffdb
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442488"
---
# <a name="tenant-offboardtenant"></a><span data-ttu-id="0a9c1-105">tenant： offboardTenant</span><span class="sxs-lookup"><span data-stu-id="0a9c1-105">tenant: offboardTenant</span></span>
<span data-ttu-id="0a9c1-106">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="0a9c1-106">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a9c1-107">执行适当的过程以从多租户管理平台中删除托管租户。</span><span class="sxs-lookup"><span data-stu-id="0a9c1-107">Carries out the appropriate procedures to remove a managed tenant from the multi-tenant management platform.</span></span> <span data-ttu-id="0a9c1-108">商业和委派管理权限等关系不会受到影响。</span><span class="sxs-lookup"><span data-stu-id="0a9c1-108">No relationships, such as commerce and delegate administrative privileges, will be impacted.</span></span> <span data-ttu-id="0a9c1-109">通过调用此操作进行的唯一更改是租户从多租户管理平台取消设置。</span><span class="sxs-lookup"><span data-stu-id="0a9c1-109">The only change made by invoking this action is the tenant will be deprovisioned from the multi-tenant management platform.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a9c1-110">权限</span><span class="sxs-lookup"><span data-stu-id="0a9c1-110">Permissions</span></span>
<span data-ttu-id="0a9c1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a9c1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a9c1-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a9c1-113">Permission type</span></span>|<span data-ttu-id="0a9c1-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a9c1-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a9c1-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a9c1-115">Delegated (work or school account)</span></span>|<span data-ttu-id="0a9c1-116">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a9c1-116">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="0a9c1-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a9c1-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a9c1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a9c1-118">Not supported.</span></span>|
|<span data-ttu-id="0a9c1-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a9c1-119">Application</span></span>|<span data-ttu-id="0a9c1-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a9c1-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a9c1-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a9c1-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenants/{tenantId}/offboardTenant
```

## <a name="request-headers"></a><span data-ttu-id="0a9c1-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a9c1-122">Request headers</span></span>
|<span data-ttu-id="0a9c1-123">名称</span><span class="sxs-lookup"><span data-stu-id="0a9c1-123">Name</span></span>|<span data-ttu-id="0a9c1-124">说明</span><span class="sxs-lookup"><span data-stu-id="0a9c1-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0a9c1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a9c1-125">Authorization</span></span>|<span data-ttu-id="0a9c1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0a9c1-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a9c1-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a9c1-128">Request body</span></span>
<span data-ttu-id="0a9c1-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0a9c1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a9c1-130">响应</span><span class="sxs-lookup"><span data-stu-id="0a9c1-130">Response</span></span>

<span data-ttu-id="0a9c1-131">如果成功，此操作在响应正文中返回 响应代码 `200 OK` 和租户。 [](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="0a9c1-131">If successful, this action returns a `200 OK` response code and a [tenant](../resources/managedtenants-tenant.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0a9c1-132">示例</span><span class="sxs-lookup"><span data-stu-id="0a9c1-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0a9c1-133">请求</span><span class="sxs-lookup"><span data-stu-id="0a9c1-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0a9c1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a9c1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tenant_offboardtenant"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenants/{tenantId}/offboardTenant
```
# <a name="c"></a>[<span data-ttu-id="0a9c1-135">C#</span><span class="sxs-lookup"><span data-stu-id="0a9c1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tenant-offboardtenant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a9c1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a9c1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tenant-offboardtenant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a9c1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a9c1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tenant-offboardtenant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a9c1-138">Java</span><span class="sxs-lookup"><span data-stu-id="0a9c1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tenant-offboardtenant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0a9c1-139">响应</span><span class="sxs-lookup"><span data-stu-id="0a9c1-139">Response</span></span>
><span data-ttu-id="0a9c1-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0a9c1-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "value": {
    "@odata.type": "#microsoft.graph.managedTenants.tenant",
    "id": "String (identifier)",
    "tenantId": "String",
    "displayName": "String",
    "contract": {
      "@odata.type": "microsoft.graph.managedTenants.tenantContract"
    },
    "tenantStatusInformation": {
      "@odata.type": "microsoft.graph.managedTenants.tenantStatusInformation"
    },
    "lastUpdatedDateTime": "String (timestamp)",
    "createdDateTime": "String (timestamp)"
  }
}
```
