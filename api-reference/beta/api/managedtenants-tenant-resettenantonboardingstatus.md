---
title: tenant： resetTenantOnboardingStatus
description: 执行适当的过程以重置使用 offboardTenant 操作从多租户管理平台中删除的托管租户的载入状态。 通过调用此操作，平台将尝试载入托管租户进行管理。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: dadbf614e74da6d139e2a07e98a528ae2955cd8a
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402312"
---
# <a name="tenant-resettenantonboardingstatus"></a><span data-ttu-id="485de-104">tenant： resetTenantOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="485de-104">tenant: resetTenantOnboardingStatus</span></span>
<span data-ttu-id="485de-105">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="485de-105">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="485de-106">执行适当的过程以重置使用 [offboardTenant](../api/managedtenants-tenant-offboardtenant.md) 操作从多租户管理平台中删除的托管租户的载入状态。</span><span class="sxs-lookup"><span data-stu-id="485de-106">Carries out the appropriate procedures to reset the onboarding status for the managed tenant that was removed from the multi-tenant management platform using the [offboardTenant](../api/managedtenants-tenant-offboardtenant.md) action.</span></span> <span data-ttu-id="485de-107">通过调用此操作，平台将尝试载入托管租户进行管理。</span><span class="sxs-lookup"><span data-stu-id="485de-107">By invoking this action the platform will attempt to onboard the managed tenant for management.</span></span>

## <a name="permissions"></a><span data-ttu-id="485de-108">权限</span><span class="sxs-lookup"><span data-stu-id="485de-108">Permissions</span></span>
<span data-ttu-id="485de-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="485de-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="485de-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="485de-111">Permission type</span></span>|<span data-ttu-id="485de-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="485de-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="485de-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="485de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="485de-114">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="485de-114">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="485de-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="485de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="485de-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="485de-116">Not supported.</span></span>|
|<span data-ttu-id="485de-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="485de-117">Application</span></span>|<span data-ttu-id="485de-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="485de-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="485de-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="485de-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenants/{tenantId}/resetTenantOnboardingStatus
```

## <a name="request-headers"></a><span data-ttu-id="485de-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="485de-120">Request headers</span></span>
|<span data-ttu-id="485de-121">名称</span><span class="sxs-lookup"><span data-stu-id="485de-121">Name</span></span>|<span data-ttu-id="485de-122">说明</span><span class="sxs-lookup"><span data-stu-id="485de-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="485de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="485de-123">Authorization</span></span>|<span data-ttu-id="485de-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="485de-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="485de-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="485de-126">Request body</span></span>
<span data-ttu-id="485de-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="485de-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="485de-128">响应</span><span class="sxs-lookup"><span data-stu-id="485de-128">Response</span></span>

<span data-ttu-id="485de-129">如果成功，此操作在响应正文中返回 响应代码 `200 OK` 和租户。 [](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="485de-129">If successful, this action returns a `200 OK` response code and a [tenant](../resources/managedtenants-tenant.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="485de-130">示例</span><span class="sxs-lookup"><span data-stu-id="485de-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="485de-131">请求</span><span class="sxs-lookup"><span data-stu-id="485de-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "tenant_resettenantonboardingstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenants/{tenantId}/resetTenantOnboardingStatus
```

### <a name="response"></a><span data-ttu-id="485de-132">响应</span><span class="sxs-lookup"><span data-stu-id="485de-132">Response</span></span>
><span data-ttu-id="485de-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="485de-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "onboardingStatus": "inactive",
    "onboardingDateTime": "2012-02-20T00:00:00Z",
    "onboardedByUserId": "",
    "offboardedDateTime": "2012-02-20T00:00:00Z",
    "offboardedBy": "",
    "delegatedPrivilegeStatus": "delegatedAdminPrivileges",
    "workloadStatuses": []
  },
  "createdDateTime": "2012-02-20T00:00:00Z",
  "lastUpdatedDatetime": "2021-02-20T00:00:00Z"
}
```
