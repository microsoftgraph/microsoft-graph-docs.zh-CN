---
title: tenantTag：assignTag
description: 将租户标记分配给指定的托管租户。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 8f9d641cb0d3129802431948601d656f9036e2ef
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402361"
---
# <a name="tenanttag-assigntag"></a><span data-ttu-id="d39aa-103">tenantTag：assignTag</span><span class="sxs-lookup"><span data-stu-id="d39aa-103">tenantTag: assignTag</span></span>
<span data-ttu-id="d39aa-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="d39aa-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d39aa-105">将租户标记分配给指定的托管租户。</span><span class="sxs-lookup"><span data-stu-id="d39aa-105">Assign the tenant tag to the specified managed tenants.</span></span>

## <a name="permissions"></a><span data-ttu-id="d39aa-106">权限</span><span class="sxs-lookup"><span data-stu-id="d39aa-106">Permissions</span></span>
<span data-ttu-id="d39aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d39aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d39aa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d39aa-109">Permission type</span></span>|<span data-ttu-id="d39aa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d39aa-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d39aa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d39aa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d39aa-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="d39aa-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="d39aa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d39aa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d39aa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d39aa-114">Not supported.</span></span>|
|<span data-ttu-id="d39aa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d39aa-115">Application</span></span>|<span data-ttu-id="d39aa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d39aa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d39aa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d39aa-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenantTags/{tenantTagId}/assignTag
```

## <a name="request-headers"></a><span data-ttu-id="d39aa-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d39aa-118">Request headers</span></span>
|<span data-ttu-id="d39aa-119">名称</span><span class="sxs-lookup"><span data-stu-id="d39aa-119">Name</span></span>|<span data-ttu-id="d39aa-120">说明</span><span class="sxs-lookup"><span data-stu-id="d39aa-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d39aa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d39aa-121">Authorization</span></span>|<span data-ttu-id="d39aa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d39aa-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d39aa-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d39aa-124">Content-Type</span></span>|<span data-ttu-id="d39aa-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d39aa-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d39aa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d39aa-127">Request body</span></span>
<span data-ttu-id="d39aa-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d39aa-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d39aa-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="d39aa-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d39aa-130">参数</span><span class="sxs-lookup"><span data-stu-id="d39aa-130">Parameter</span></span>|<span data-ttu-id="d39aa-131">类型</span><span class="sxs-lookup"><span data-stu-id="d39aa-131">Type</span></span>|<span data-ttu-id="d39aa-132">说明</span><span class="sxs-lookup"><span data-stu-id="d39aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d39aa-133">tenantIds</span><span class="sxs-lookup"><span data-stu-id="d39aa-133">tenantIds</span></span>|<span data-ttu-id="d39aa-134">字符串集合</span><span class="sxs-lookup"><span data-stu-id="d39aa-134">String collection</span></span>|<span data-ttu-id="d39aa-135">应Azure Active Directory租户标记的租户标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="d39aa-135">The collection of Azure Active Directory tenant identifiers where the tenant tag should be assigned.</span></span>|

## <a name="response"></a><span data-ttu-id="d39aa-136">响应</span><span class="sxs-lookup"><span data-stu-id="d39aa-136">Response</span></span>

<span data-ttu-id="d39aa-137">如果成功，此操作在响应 `200 OK` 正文中返回 响应代码和[tenantTag。](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="d39aa-137">If successful, this action returns a `200 OK` response code and a [tenantTag](../resources/managedtenants-tenanttag.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d39aa-138">示例</span><span class="sxs-lookup"><span data-stu-id="d39aa-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d39aa-139">请求</span><span class="sxs-lookup"><span data-stu-id="d39aa-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "tenanttag_assigntag"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}/assignTag
Content-Type: application/json
Content-length: 41

{
  "tenantIds": [
    "String"
  ]
}
```

### <a name="response"></a><span data-ttu-id="d39aa-140">响应</span><span class="sxs-lookup"><span data-stu-id="d39aa-140">Response</span></span>
><span data-ttu-id="d39aa-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d39aa-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantTags/$entity",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b",
  "displayName": "Support",
  "description": "Tenants that have purchased support",
  "tenants": [
    {
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b"
    }
  ],
  "isDeleted": null,
  "createdDateTime": "2021-06-26T13:51:23.3927236Z",
  "createdByUserId": "65ca7649-4ccb-4823-9c39-42bd75191bf8",
  "lastActionDateTime": "2021-07-11T19:55:19.7230386Z",
  "lastActionByUserId": "50bf7bd8-1b3a-4d1d-94c5-86d27e68857f"
}
```
