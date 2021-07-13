---
title: 创建 tenantTag
description: 创建新的 tenantTag 对象。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 9de058914e2262debcbe87d449b5ffc7fc15db7b
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402320"
---
# <a name="create-tenanttag"></a><span data-ttu-id="3324d-103">创建 tenantTag</span><span class="sxs-lookup"><span data-stu-id="3324d-103">Create tenantTag</span></span>
<span data-ttu-id="3324d-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="3324d-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3324d-105">创建新的 [tenantTag](../resources/managedtenants-tenanttag.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3324d-105">Create a new [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3324d-106">权限</span><span class="sxs-lookup"><span data-stu-id="3324d-106">Permissions</span></span>
<span data-ttu-id="3324d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3324d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3324d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3324d-109">Permission type</span></span>|<span data-ttu-id="3324d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3324d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3324d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3324d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3324d-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="3324d-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="3324d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3324d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3324d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3324d-114">Not supported.</span></span>|
|<span data-ttu-id="3324d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3324d-115">Application</span></span>|<span data-ttu-id="3324d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3324d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3324d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3324d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenantTags
```

## <a name="request-headers"></a><span data-ttu-id="3324d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3324d-118">Request headers</span></span>
|<span data-ttu-id="3324d-119">名称</span><span class="sxs-lookup"><span data-stu-id="3324d-119">Name</span></span>|<span data-ttu-id="3324d-120">说明</span><span class="sxs-lookup"><span data-stu-id="3324d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3324d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3324d-121">Authorization</span></span>|<span data-ttu-id="3324d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3324d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3324d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3324d-124">Content-Type</span></span>|<span data-ttu-id="3324d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3324d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3324d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3324d-127">Request body</span></span>
<span data-ttu-id="3324d-128">在请求正文中，提供 [tenantTag](../resources/managedtenants-tenanttag.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3324d-128">In the request body, supply a JSON representation of the [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

<span data-ttu-id="3324d-129">下表显示创建 [tenantTag](../resources/managedtenants-tenanttag.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3324d-129">The following table shows the properties that are required when you create the [tenantTag](../resources/managedtenants-tenanttag.md).</span></span>

|<span data-ttu-id="3324d-130">属性</span><span class="sxs-lookup"><span data-stu-id="3324d-130">Property</span></span>|<span data-ttu-id="3324d-131">类型</span><span class="sxs-lookup"><span data-stu-id="3324d-131">Type</span></span>|<span data-ttu-id="3324d-132">说明</span><span class="sxs-lookup"><span data-stu-id="3324d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3324d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3324d-133">displayName</span></span>|<span data-ttu-id="3324d-134">String</span><span class="sxs-lookup"><span data-stu-id="3324d-134">String</span></span>|<span data-ttu-id="3324d-135">租户显示名称的变量。</span><span class="sxs-lookup"><span data-stu-id="3324d-135">The display name for the tenant tag.</span></span>|
|<span data-ttu-id="3324d-136">说明</span><span class="sxs-lookup"><span data-stu-id="3324d-136">description</span></span>|<span data-ttu-id="3324d-137">String</span><span class="sxs-lookup"><span data-stu-id="3324d-137">String</span></span>|<span data-ttu-id="3324d-138">租户标记的说明。</span><span class="sxs-lookup"><span data-stu-id="3324d-138">The description for the tenant tag.</span></span>|

## <a name="response"></a><span data-ttu-id="3324d-139">响应</span><span class="sxs-lookup"><span data-stu-id="3324d-139">Response</span></span>

<span data-ttu-id="3324d-140">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [tenantTag](../resources/managedtenants-tenanttag.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3324d-140">If successful, this method returns a `201 Created` response code and a [tenantTag](../resources/managedtenants-tenanttag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3324d-141">示例</span><span class="sxs-lookup"><span data-stu-id="3324d-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3324d-142">请求</span><span class="sxs-lookup"><span data-stu-id="3324d-142">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tenanttag_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags
Content-Type: application/json
Content-length: 382

{
  "displayName": "Support",
  "description": "Tenants that have purchased extended support"
}
```

### <a name="response"></a><span data-ttu-id="3324d-143">响应</span><span class="sxs-lookup"><span data-stu-id="3324d-143">Response</span></span>
><span data-ttu-id="3324d-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3324d-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantTag"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantTags/$entity",
  "id": "11103b2b-0e28-456b-901d-45f98890ab1d",
  "displayName": "Support",
  "description": "Tenants that have purchased extended support",
  "tenantIds": [],
  "isDeleted": null,
  "createdDateTime": "2021-07-11T19:31:49.807267Z",
  "createdByUserId": "cad28f13-0158-43c5-9c59-952f2caa62c0",
  "lastActionDateTime": "2021-07-11T19:31:49.8072716Z",
  "lastActionByUserId": "cad28f13-0158-43c5-9c59-952f2caa62c0"
}
```
