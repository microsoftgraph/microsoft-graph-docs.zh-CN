---
title: tenantGroup：tenantSearch
description: 跨租户组搜索指定的托管租户。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 0699ebc7b9890826d714a108e7738fe0fd2b92b4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402085"
---
# <a name="tenantgroup-tenantsearch"></a><span data-ttu-id="7d175-103">tenantGroup：tenantSearch</span><span class="sxs-lookup"><span data-stu-id="7d175-103">tenantGroup: tenantSearch</span></span>
<span data-ttu-id="7d175-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="7d175-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d175-105">跨租户组搜索指定的托管租户。</span><span class="sxs-lookup"><span data-stu-id="7d175-105">Searches for the specified managed tenants across tenant groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d175-106">权限</span><span class="sxs-lookup"><span data-stu-id="7d175-106">Permissions</span></span>
<span data-ttu-id="7d175-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7d175-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d175-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d175-109">Permission type</span></span>|<span data-ttu-id="7d175-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7d175-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d175-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d175-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7d175-112">ManagedTenants.Read.All、ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d175-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="7d175-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d175-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d175-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d175-114">Not supported.</span></span>|
|<span data-ttu-id="7d175-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7d175-115">Application</span></span>|<span data-ttu-id="7d175-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d175-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d175-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d175-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenantGroups/tenantSearch
```

## <a name="request-headers"></a><span data-ttu-id="7d175-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7d175-118">Request headers</span></span>
|<span data-ttu-id="7d175-119">名称</span><span class="sxs-lookup"><span data-stu-id="7d175-119">Name</span></span>|<span data-ttu-id="7d175-120">说明</span><span class="sxs-lookup"><span data-stu-id="7d175-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7d175-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d175-121">Authorization</span></span>|<span data-ttu-id="7d175-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7d175-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7d175-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7d175-124">Content-Type</span></span>|<span data-ttu-id="7d175-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7d175-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d175-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d175-127">Request body</span></span>
<span data-ttu-id="7d175-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d175-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7d175-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="7d175-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7d175-130">参数</span><span class="sxs-lookup"><span data-stu-id="7d175-130">Parameter</span></span>|<span data-ttu-id="7d175-131">类型</span><span class="sxs-lookup"><span data-stu-id="7d175-131">Type</span></span>|<span data-ttu-id="7d175-132">说明</span><span class="sxs-lookup"><span data-stu-id="7d175-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d175-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="7d175-133">tenantId</span></span>|<span data-ttu-id="7d175-134">String</span><span class="sxs-lookup"><span data-stu-id="7d175-134">String</span></span>|<span data-ttu-id="7d175-135">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="7d175-135">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|



## <a name="response"></a><span data-ttu-id="7d175-136">响应</span><span class="sxs-lookup"><span data-stu-id="7d175-136">Response</span></span>

<span data-ttu-id="7d175-137">如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="7d175-137">If successful, this action returns a `200 OK` response code and a [microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7d175-138">示例</span><span class="sxs-lookup"><span data-stu-id="7d175-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7d175-139">请求</span><span class="sxs-lookup"><span data-stu-id="7d175-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "tenantgroup_tenantsearch"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantGroups/tenantSearch
Content-Type: application/json
Content-length: 28

{
  "tenantId": "String"
}
```

### <a name="response"></a><span data-ttu-id="7d175-140">响应</span><span class="sxs-lookup"><span data-stu-id="7d175-140">Response</span></span>
><span data-ttu-id="7d175-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7d175-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenantGroup)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantGroups",
  "value": [
    {
      "id": "2e6a0c9f-986d-480e-ad4b-bdfddc047aba",
      "displayName": "Default",
      "allTenantsIncluded": true,
      "tenantIds": [],
      "managementIntents": [
        {
          "managementIntentId": "586895ab-8a59-4b79-be25-b06949a819bb",
          "managementIntentDisplayName": "Default Baseline",
          "managementTemplates": [
            {
              "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
              "displayName": "Baseline - Block Legacy Authentication",
              "category": "identity"
            },
            {
              "managementTemplateId": "12524106-036f-457f-b7a6-b003509d29c8",
              "displayName": "Baseline - Require MFA for Admins",
              "category": "identity"
            },
            {
              "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
              "displayName": "Baseline - Require MFA for end users",
              "category": "identity"
            },
            {
              "managementTemplateId": "e2cadc41-a08f-45e7-8eb1-942d224dfb9a",
              "displayName": "Baseline - Enroll devices in MEM",
              "category": "devices"
            },
            {
              "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
              "displayName": "Baseline - Setup Compliance Policy for Windows 10 devices",
              "category": "devices"
            },
            {
              "managementTemplateId": "b2d6d189-ea31-4cf8-b75e-41210c583127",
              "displayName": "Baseline - Setup Microsoft Defender Antivirus Policy for Windows 10 devices",
              "category": "devices"
            }
          ]
        }
      ],
      "managementActions": []
    }
  ]
}
```
