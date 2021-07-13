---
title: cloudPcDevice 资源类型
description: 表示属于给定托管租户的云电脑设备。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 57eabb6720987a8a9bfca4c18e283057848b65cf
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402071"
---
# <a name="cloudpcdevice-resource-type"></a><span data-ttu-id="78d5f-103">cloudPcDevice 资源类型</span><span class="sxs-lookup"><span data-stu-id="78d5f-103">cloudPcDevice resource type</span></span>

<span data-ttu-id="78d5f-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="78d5f-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78d5f-105">表示属于给定托管租户的云电脑设备。</span><span class="sxs-lookup"><span data-stu-id="78d5f-105">Represents a cloud PC device that belongs to a given managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="78d5f-106">方法</span><span class="sxs-lookup"><span data-stu-id="78d5f-106">Methods</span></span>
|<span data-ttu-id="78d5f-107">方法</span><span class="sxs-lookup"><span data-stu-id="78d5f-107">Method</span></span>|<span data-ttu-id="78d5f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="78d5f-108">Return type</span></span>|<span data-ttu-id="78d5f-109">说明</span><span class="sxs-lookup"><span data-stu-id="78d5f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="78d5f-110">列出 cloudPcDevices</span><span class="sxs-lookup"><span data-stu-id="78d5f-110">List cloudPcDevices</span></span>](../api/managedtenants-managedtenant-list-cloudpcdevices.md)|<span data-ttu-id="78d5f-111">[microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="78d5f-111">[microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) collection</span></span>|<span data-ttu-id="78d5f-112">获取 [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="78d5f-112">Get a list of the [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) objects and their properties.</span></span>|
|[<span data-ttu-id="78d5f-113">获取 cloudPcDevice</span><span class="sxs-lookup"><span data-stu-id="78d5f-113">Get cloudPcDevice</span></span>](../api/managedtenants-cloudpcdevice-get.md)|[<span data-ttu-id="78d5f-114">microsoft.graph.managedTenants.cloudPcDevice</span><span class="sxs-lookup"><span data-stu-id="78d5f-114">microsoft.graph.managedTenants.cloudPcDevice</span></span>](../resources/managedtenants-cloudpcdevice.md)|<span data-ttu-id="78d5f-115">读取 [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="78d5f-115">Read the properties and relationships of a [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="78d5f-116">属性</span><span class="sxs-lookup"><span data-stu-id="78d5f-116">Properties</span></span>
|<span data-ttu-id="78d5f-117">属性</span><span class="sxs-lookup"><span data-stu-id="78d5f-117">Property</span></span>|<span data-ttu-id="78d5f-118">类型</span><span class="sxs-lookup"><span data-stu-id="78d5f-118">Type</span></span>|<span data-ttu-id="78d5f-119">说明</span><span class="sxs-lookup"><span data-stu-id="78d5f-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78d5f-120">cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="78d5f-120">cloudPcStatus</span></span>|<span data-ttu-id="78d5f-121">String</span><span class="sxs-lookup"><span data-stu-id="78d5f-121">String</span></span>|<span data-ttu-id="78d5f-122">云电脑的状态。</span><span class="sxs-lookup"><span data-stu-id="78d5f-122">The status of the cloud PC.</span></span> <span data-ttu-id="78d5f-123">可取值为：`notProvisioned`、`provisioning`、`provisioned`、`upgrading`、`inGracePeriod`、`deprovisioning` 或 `failed`。</span><span class="sxs-lookup"><span data-stu-id="78d5f-123">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span></span> <span data-ttu-id="78d5f-124">必填。</span><span class="sxs-lookup"><span data-stu-id="78d5f-124">Required.</span></span> <span data-ttu-id="78d5f-125">只读。</span><span class="sxs-lookup"><span data-stu-id="78d5f-125">Read-only.</span></span>|
|<span data-ttu-id="78d5f-126">displayName</span><span class="sxs-lookup"><span data-stu-id="78d5f-126">displayName</span></span>|<span data-ttu-id="78d5f-127">String</span><span class="sxs-lookup"><span data-stu-id="78d5f-127">String</span></span>|<span data-ttu-id="78d5f-128">云显示名称应用。</span><span class="sxs-lookup"><span data-stu-id="78d5f-128">The display name for the cloud PC.</span></span> <span data-ttu-id="78d5f-129">必填。</span><span class="sxs-lookup"><span data-stu-id="78d5f-129">Required.</span></span> <span data-ttu-id="78d5f-130">只读。</span><span class="sxs-lookup"><span data-stu-id="78d5f-130">Read-only.</span></span>|
|<span data-ttu-id="78d5f-131">id</span><span class="sxs-lookup"><span data-stu-id="78d5f-131">id</span></span>|<span data-ttu-id="78d5f-132">String</span><span class="sxs-lookup"><span data-stu-id="78d5f-132">String</span></span>|<span data-ttu-id="78d5f-133">云电脑的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="78d5f-133">The unique identifier for the cloud PC.</span></span> <span data-ttu-id="78d5f-134">必填。</span><span class="sxs-lookup"><span data-stu-id="78d5f-134">Required.</span></span> <span data-ttu-id="78d5f-135">只读。</span><span class="sxs-lookup"><span data-stu-id="78d5f-135">Read-only.</span></span>|
|<span data-ttu-id="78d5f-136">lastRefreshedDateTime</span><span class="sxs-lookup"><span data-stu-id="78d5f-136">lastRefreshedDateTime</span></span>|<span data-ttu-id="78d5f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78d5f-137">DateTimeOffset</span></span>|<span data-ttu-id="78d5f-138">实体上次在多租户管理平台中更新的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="78d5f-138">Date and time the entity was last updated in the multi-tenant management platform.</span></span> <span data-ttu-id="78d5f-139">必填。</span><span class="sxs-lookup"><span data-stu-id="78d5f-139">Required.</span></span> <span data-ttu-id="78d5f-140">只读。</span><span class="sxs-lookup"><span data-stu-id="78d5f-140">Read-only.</span></span>|
|<span data-ttu-id="78d5f-141">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="78d5f-141">managedDeviceId</span></span>|<span data-ttu-id="78d5f-142">String</span><span class="sxs-lookup"><span data-stu-id="78d5f-142">String</span></span>|<span data-ttu-id="78d5f-143">云电脑的托管设备标识符。</span><span class="sxs-lookup"><span data-stu-id="78d5f-143">The managed device identifier for the cloud PC.</span></span> <span data-ttu-id="78d5f-144">可选。</span><span class="sxs-lookup"><span data-stu-id="78d5f-144">Optional.</span></span> <span data-ttu-id="78d5f-145">只读。</span><span class="sxs-lookup"><span data-stu-id="78d5f-145">Read-only.</span></span>|
|<span data-ttu-id="78d5f-146">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="78d5f-146">managedDeviceName</span></span>|<span data-ttu-id="78d5f-147">String</span><span class="sxs-lookup"><span data-stu-id="78d5f-147">String</span></span>|<span data-ttu-id="78d5f-148">托管设备显示名称云电脑。</span><span class="sxs-lookup"><span data-stu-id="78d5f-148">The managed device display name for the cloud PC.</span></span> <span data-ttu-id="78d5f-149">可选。</span><span class="sxs-lookup"><span data-stu-id="78d5f-149">Optional.</span></span> <span data-ttu-id="78d5f-150">只读。</span><span class="sxs-lookup"><span data-stu-id="78d5f-150">Read-only.</span></span>|
|<span data-ttu-id="78d5f-151">provisioningPolicyId</span><span class="sxs-lookup"><span data-stu-id="78d5f-151">provisioningPolicyId</span></span>|<span data-ttu-id="78d5f-152">String</span><span class="sxs-lookup"><span data-stu-id="78d5f-152">String</span></span>|<span data-ttu-id="78d5f-153">云电脑的预配策略标识符。</span><span class="sxs-lookup"><span data-stu-id="78d5f-153">The provisioning policy identifier for the cloud PC.</span></span> <span data-ttu-id="78d5f-154">必填。</span><span class="sxs-lookup"><span data-stu-id="78d5f-154">Required.</span></span> <span data-ttu-id="78d5f-155">只读。</span><span class="sxs-lookup"><span data-stu-id="78d5f-155">Read-only.</span></span>|
|<span data-ttu-id="78d5f-156">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="78d5f-156">servicePlanName</span></span>|<span data-ttu-id="78d5f-157">String</span><span class="sxs-lookup"><span data-stu-id="78d5f-157">String</span></span>|<span data-ttu-id="78d5f-158">云电脑的服务计划名称。</span><span class="sxs-lookup"><span data-stu-id="78d5f-158">The service plan name for the cloud PC.</span></span> <span data-ttu-id="78d5f-159">必填。</span><span class="sxs-lookup"><span data-stu-id="78d5f-159">Required.</span></span> <span data-ttu-id="78d5f-160">只读。</span><span class="sxs-lookup"><span data-stu-id="78d5f-160">Read-only.</span></span>|
|<span data-ttu-id="78d5f-161">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="78d5f-161">tenantDisplayName</span></span>|<span data-ttu-id="78d5f-162">String</span><span class="sxs-lookup"><span data-stu-id="78d5f-162">String</span></span>|<span data-ttu-id="78d5f-163">托管显示名称租户的租户。</span><span class="sxs-lookup"><span data-stu-id="78d5f-163">The display name for the managed tenant.</span></span> <span data-ttu-id="78d5f-164">必填。</span><span class="sxs-lookup"><span data-stu-id="78d5f-164">Required.</span></span> <span data-ttu-id="78d5f-165">只读。</span><span class="sxs-lookup"><span data-stu-id="78d5f-165">Read-only.</span></span>|
|<span data-ttu-id="78d5f-166">tenantId</span><span class="sxs-lookup"><span data-stu-id="78d5f-166">tenantId</span></span>|<span data-ttu-id="78d5f-167">String</span><span class="sxs-lookup"><span data-stu-id="78d5f-167">String</span></span>|<span data-ttu-id="78d5f-168">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="78d5f-168">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="78d5f-169">必填。</span><span class="sxs-lookup"><span data-stu-id="78d5f-169">Required.</span></span> <span data-ttu-id="78d5f-170">只读。</span><span class="sxs-lookup"><span data-stu-id="78d5f-170">Read-only.</span></span>|
|<span data-ttu-id="78d5f-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="78d5f-171">userPrincipalName</span></span>|<span data-ttu-id="78d5f-172">String</span><span class="sxs-lookup"><span data-stu-id="78d5f-172">String</span></span>|<span data-ttu-id="78d5f-173">用户主体名称 (分配给) 电脑的用户的 UPN 名称。</span><span class="sxs-lookup"><span data-stu-id="78d5f-173">The user principal name (UPN) of the user assigned to the cloud PC.</span></span> <span data-ttu-id="78d5f-174">必填。</span><span class="sxs-lookup"><span data-stu-id="78d5f-174">Required.</span></span> <span data-ttu-id="78d5f-175">只读。</span><span class="sxs-lookup"><span data-stu-id="78d5f-175">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78d5f-176">关系</span><span class="sxs-lookup"><span data-stu-id="78d5f-176">Relationships</span></span>
<span data-ttu-id="78d5f-177">无。</span><span class="sxs-lookup"><span data-stu-id="78d5f-177">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="78d5f-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78d5f-178">JSON representation</span></span>
<span data-ttu-id="78d5f-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78d5f-179">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.cloudPcDevice",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcDevice",
  "id": "String (identifier)",
  "displayName": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "userPrincipalName": "String",
  "servicePlanName": "String",
  "cloudPcStatus": "String",
  "provisioningPolicyId": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
