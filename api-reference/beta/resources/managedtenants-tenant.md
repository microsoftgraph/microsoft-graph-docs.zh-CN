---
title: 租户资源类型
description: 表示与管理实体关联的租户。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: ee4bd57aa4e7fa2ea15c86376389d3b6e12198ea
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402396"
---
# <a name="tenant-resource-type"></a><span data-ttu-id="d904c-103">租户资源类型</span><span class="sxs-lookup"><span data-stu-id="d904c-103">tenant resource type</span></span>

<span data-ttu-id="d904c-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="d904c-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d904c-105">表示与管理实体关联的租户。</span><span class="sxs-lookup"><span data-stu-id="d904c-105">Represents a tenant associated with the managing entity.</span></span>

## <a name="methods"></a><span data-ttu-id="d904c-106">方法</span><span class="sxs-lookup"><span data-stu-id="d904c-106">Methods</span></span>
|<span data-ttu-id="d904c-107">方法</span><span class="sxs-lookup"><span data-stu-id="d904c-107">Method</span></span>|<span data-ttu-id="d904c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d904c-108">Return type</span></span>|<span data-ttu-id="d904c-109">说明</span><span class="sxs-lookup"><span data-stu-id="d904c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d904c-110">列出租户</span><span class="sxs-lookup"><span data-stu-id="d904c-110">List tenants</span></span>](../api/managedtenants-managedtenant-list-tenants.md)|<span data-ttu-id="d904c-111">[microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d904c-111">[microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md) collection</span></span>|<span data-ttu-id="d904c-112">获取租户对象 [及其](../resources/managedtenants-tenant.md) 属性的列表。</span><span class="sxs-lookup"><span data-stu-id="d904c-112">Get a list of the [tenant](../resources/managedtenants-tenant.md) objects and their properties.</span></span>|
|[<span data-ttu-id="d904c-113">获取租户</span><span class="sxs-lookup"><span data-stu-id="d904c-113">Get tenant</span></span>](../api/managedtenants-tenant-get.md)|[<span data-ttu-id="d904c-114">microsoft.graph.managedTenants.tenant</span><span class="sxs-lookup"><span data-stu-id="d904c-114">microsoft.graph.managedTenants.tenant</span></span>](../resources/managedtenants-tenant.md)|<span data-ttu-id="d904c-115">读取租户对象的属性 [和](../resources/managedtenants-tenant.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="d904c-115">Read the properties and relationships of a [tenant](../resources/managedtenants-tenant.md) object.</span></span>|
|[<span data-ttu-id="d904c-116">offboardTenant</span><span class="sxs-lookup"><span data-stu-id="d904c-116">offboardTenant</span></span>](../api/managedtenants-tenant-offboardtenant.md)|[<span data-ttu-id="d904c-117">microsoft.graph.managedTenants.tenant</span><span class="sxs-lookup"><span data-stu-id="d904c-117">microsoft.graph.managedTenants.tenant</span></span>](../resources/managedtenants-tenant.md)|<span data-ttu-id="d904c-118">从多租户管理平台注销租户。</span><span class="sxs-lookup"><span data-stu-id="d904c-118">Off boards a tenant from the multi-tenant management platform.</span></span>|
|[<span data-ttu-id="d904c-119">resetTenantOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="d904c-119">resetTenantOnboardingStatus</span></span>](../api/managedtenants-tenant-resettenantonboardingstatus.md)|[<span data-ttu-id="d904c-120">microsoft.graph.managedTenants.tenant</span><span class="sxs-lookup"><span data-stu-id="d904c-120">microsoft.graph.managedTenants.tenant</span></span>](../resources/managedtenants-tenant.md)|<span data-ttu-id="d904c-121">使用多租户管理平台重置租户载入状态。</span><span class="sxs-lookup"><span data-stu-id="d904c-121">Resets the tenant onboarding status with the multi-tenant management platform.</span></span>|

## <a name="properties"></a><span data-ttu-id="d904c-122">属性</span><span class="sxs-lookup"><span data-stu-id="d904c-122">Properties</span></span>
|<span data-ttu-id="d904c-123">属性</span><span class="sxs-lookup"><span data-stu-id="d904c-123">Property</span></span>|<span data-ttu-id="d904c-124">类型</span><span class="sxs-lookup"><span data-stu-id="d904c-124">Type</span></span>|<span data-ttu-id="d904c-125">说明</span><span class="sxs-lookup"><span data-stu-id="d904c-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d904c-126">contract</span><span class="sxs-lookup"><span data-stu-id="d904c-126">contract</span></span>|[<span data-ttu-id="d904c-127">microsoft.graph.managedTenants.tenantContract</span><span class="sxs-lookup"><span data-stu-id="d904c-127">microsoft.graph.managedTenants.tenantContract</span></span>](../resources/managedtenants-tenantcontract.md)|<span data-ttu-id="d904c-128">租户与管理实体的关系详细信息。</span><span class="sxs-lookup"><span data-stu-id="d904c-128">The relationship details for the tenant with the managing entity.</span></span>|
|<span data-ttu-id="d904c-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d904c-129">createdDateTime</span></span>|<span data-ttu-id="d904c-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d904c-130">DateTimeOffset</span></span>|<span data-ttu-id="d904c-131">在多租户管理平台中创建租户的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d904c-131">The date and time the tenant was created in the multi-tenant management platform.</span></span> <span data-ttu-id="d904c-132">可选。</span><span class="sxs-lookup"><span data-stu-id="d904c-132">Optional.</span></span> <span data-ttu-id="d904c-133">只读。</span><span class="sxs-lookup"><span data-stu-id="d904c-133">Read-only.</span></span>|
|<span data-ttu-id="d904c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d904c-134">displayName</span></span>|<span data-ttu-id="d904c-135">String</span><span class="sxs-lookup"><span data-stu-id="d904c-135">String</span></span>|<span data-ttu-id="d904c-136">租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d904c-136">The display name for the tenant.</span></span> <span data-ttu-id="d904c-137">必填。</span><span class="sxs-lookup"><span data-stu-id="d904c-137">Required.</span></span> <span data-ttu-id="d904c-138">只读。</span><span class="sxs-lookup"><span data-stu-id="d904c-138">Read-only.</span></span>|
|<span data-ttu-id="d904c-139">id</span><span class="sxs-lookup"><span data-stu-id="d904c-139">id</span></span>|<span data-ttu-id="d904c-140">String</span><span class="sxs-lookup"><span data-stu-id="d904c-140">String</span></span>|<span data-ttu-id="d904c-141">租户Azure Active Directory租户标识符。</span><span class="sxs-lookup"><span data-stu-id="d904c-141">The Azure Active Directory tenant identifier for the tenant.</span></span> <span data-ttu-id="d904c-142">必填。</span><span class="sxs-lookup"><span data-stu-id="d904c-142">Required.</span></span> <span data-ttu-id="d904c-143">只读。</span><span class="sxs-lookup"><span data-stu-id="d904c-143">Read-only.</span></span>|
|<span data-ttu-id="d904c-144">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d904c-144">lastUpdatedDateTime</span></span>|<span data-ttu-id="d904c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d904c-145">DateTimeOffset</span></span>|<span data-ttu-id="d904c-146">在多租户管理平台中上次更新租户的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d904c-146">The date and time the tenant was last updated within the multi-tenant management platform.</span></span> <span data-ttu-id="d904c-147">可选。</span><span class="sxs-lookup"><span data-stu-id="d904c-147">Optional.</span></span> <span data-ttu-id="d904c-148">只读。</span><span class="sxs-lookup"><span data-stu-id="d904c-148">Read-only.</span></span>|
|<span data-ttu-id="d904c-149">tenantId</span><span class="sxs-lookup"><span data-stu-id="d904c-149">tenantId</span></span>|<span data-ttu-id="d904c-150">String</span><span class="sxs-lookup"><span data-stu-id="d904c-150">String</span></span>|<span data-ttu-id="d904c-151">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="d904c-151">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="d904c-152">可选。</span><span class="sxs-lookup"><span data-stu-id="d904c-152">Optional.</span></span> <span data-ttu-id="d904c-153">只读。</span><span class="sxs-lookup"><span data-stu-id="d904c-153">Read-only.</span></span>|
|<span data-ttu-id="d904c-154">tenantStatusInformation</span><span class="sxs-lookup"><span data-stu-id="d904c-154">tenantStatusInformation</span></span>|[<span data-ttu-id="d904c-155">microsoft.graph.managedTenants.tenantStatusInformation</span><span class="sxs-lookup"><span data-stu-id="d904c-155">microsoft.graph.managedTenants.tenantStatusInformation</span></span>](../resources/managedtenants-tenantstatusinformation.md)|<span data-ttu-id="d904c-156">租户的载入状态信息。</span><span class="sxs-lookup"><span data-stu-id="d904c-156">The onboarding status information for the tenant.</span></span> <span data-ttu-id="d904c-157">可选。</span><span class="sxs-lookup"><span data-stu-id="d904c-157">Optional.</span></span> <span data-ttu-id="d904c-158">只读。</span><span class="sxs-lookup"><span data-stu-id="d904c-158">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d904c-159">关系</span><span class="sxs-lookup"><span data-stu-id="d904c-159">Relationships</span></span>
<span data-ttu-id="d904c-160">无。</span><span class="sxs-lookup"><span data-stu-id="d904c-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d904c-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d904c-161">JSON representation</span></span>
<span data-ttu-id="d904c-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d904c-162">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenant",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
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
```
