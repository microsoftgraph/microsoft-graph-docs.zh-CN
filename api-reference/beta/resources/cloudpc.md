---
title: cloudPC 资源类型
description: 云托管虚拟桌面。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c5fc858e29abf7d649b32991d9e30ce64cc0b632
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721612"
---
# <a name="cloudpc-resource-type"></a><span data-ttu-id="5bb16-103">cloudPC 资源类型</span><span class="sxs-lookup"><span data-stu-id="5bb16-103">cloudPC resource type</span></span>

<span data-ttu-id="5bb16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bb16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bb16-105">表示云托管虚拟桌面。</span><span class="sxs-lookup"><span data-stu-id="5bb16-105">Represents a cloud-managed virtual desktop.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="5bb16-106">方法</span><span class="sxs-lookup"><span data-stu-id="5bb16-106">Methods</span></span>

|<span data-ttu-id="5bb16-107">方法</span><span class="sxs-lookup"><span data-stu-id="5bb16-107">Method</span></span>|<span data-ttu-id="5bb16-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="5bb16-108">Return type</span></span>|<span data-ttu-id="5bb16-109">说明</span><span class="sxs-lookup"><span data-stu-id="5bb16-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5bb16-110">列出 cloudPCs</span><span class="sxs-lookup"><span data-stu-id="5bb16-110">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="5bb16-111">[cloudPC](../resources/cloudpc.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5bb16-111">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="5bb16-112">列出 cloudPC 对象 [的属性和](../resources/cloudpc.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="5bb16-112">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="5bb16-113">获取 cloudPC</span><span class="sxs-lookup"><span data-stu-id="5bb16-113">Get cloudPC</span></span>](../api/cloudpc-get.md)|[<span data-ttu-id="5bb16-114">cloudPC</span><span class="sxs-lookup"><span data-stu-id="5bb16-114">cloudPC</span></span>](../resources/cloudpc.md)|<span data-ttu-id="5bb16-115">读取 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5bb16-115">Read the properties and relationships of a [cloudPC](../resources/cloudpc.md) object.</span></span>|
|[<span data-ttu-id="5bb16-116">重新设置</span><span class="sxs-lookup"><span data-stu-id="5bb16-116">Reprovision</span></span>](../api/cloudpc-reprovision.md)|<span data-ttu-id="5bb16-117">无</span><span class="sxs-lookup"><span data-stu-id="5bb16-117">None</span></span>|<span data-ttu-id="5bb16-118">重新设置 [cloudPC](../resources/cloudpc.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5bb16-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5bb16-119">属性</span><span class="sxs-lookup"><span data-stu-id="5bb16-119">Properties</span></span>

|<span data-ttu-id="5bb16-120">属性</span><span class="sxs-lookup"><span data-stu-id="5bb16-120">Property</span></span>|<span data-ttu-id="5bb16-121">类型</span><span class="sxs-lookup"><span data-stu-id="5bb16-121">Type</span></span>|<span data-ttu-id="5bb16-122">说明</span><span class="sxs-lookup"><span data-stu-id="5bb16-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bb16-123">id</span><span class="sxs-lookup"><span data-stu-id="5bb16-123">id</span></span>|<span data-ttu-id="5bb16-124">String</span><span class="sxs-lookup"><span data-stu-id="5bb16-124">String</span></span>|<span data-ttu-id="5bb16-125">云电脑的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5bb16-125">Unique identifier for the cloud PC.</span></span> <span data-ttu-id="5bb16-126">只读。</span><span class="sxs-lookup"><span data-stu-id="5bb16-126">Read-only.</span></span>|
|<span data-ttu-id="5bb16-127">displayName</span><span class="sxs-lookup"><span data-stu-id="5bb16-127">displayName</span></span>|<span data-ttu-id="5bb16-128">String</span><span class="sxs-lookup"><span data-stu-id="5bb16-128">String</span></span>|<span data-ttu-id="5bb16-129">云电脑显示名称。</span><span class="sxs-lookup"><span data-stu-id="5bb16-129">The cloud PC display name.</span></span>|
|<span data-ttu-id="5bb16-130">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="5bb16-130">imageDisplayName</span></span>|<span data-ttu-id="5bb16-131">String</span><span class="sxs-lookup"><span data-stu-id="5bb16-131">String</span></span>|<span data-ttu-id="5bb16-132">云电脑上的操作系统映像的名称。</span><span class="sxs-lookup"><span data-stu-id="5bb16-132">Name of the OS image that's on the cloud PC.</span></span>|
|<span data-ttu-id="5bb16-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="5bb16-133">managedDeviceId</span></span>|<span data-ttu-id="5bb16-134">String</span><span class="sxs-lookup"><span data-stu-id="5bb16-134">String</span></span>|<span data-ttu-id="5bb16-135">云电脑的 Intune 设备 ID。</span><span class="sxs-lookup"><span data-stu-id="5bb16-135">The cloud PC’s Intune device ID.</span></span>|
|<span data-ttu-id="5bb16-136">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="5bb16-136">managedDeviceName</span></span>|<span data-ttu-id="5bb16-137">String</span><span class="sxs-lookup"><span data-stu-id="5bb16-137">String</span></span>|<span data-ttu-id="5bb16-138">云电脑的 Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="5bb16-138">The cloud PC’s Intune device name.</span></span>|
|<span data-ttu-id="5bb16-139">provisioningPolicyId</span><span class="sxs-lookup"><span data-stu-id="5bb16-139">provisioningPolicyId</span></span>|<span data-ttu-id="5bb16-140">String</span><span class="sxs-lookup"><span data-stu-id="5bb16-140">String</span></span>|<span data-ttu-id="5bb16-141">云电脑的预配策略 ID。</span><span class="sxs-lookup"><span data-stu-id="5bb16-141">The cloud PC's provisioning policy ID.</span></span>|
|<span data-ttu-id="5bb16-142">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="5bb16-142">servicePlanId</span></span>|<span data-ttu-id="5bb16-143">String</span><span class="sxs-lookup"><span data-stu-id="5bb16-143">String</span></span>|<span data-ttu-id="5bb16-144">云电脑的服务计划 ID。</span><span class="sxs-lookup"><span data-stu-id="5bb16-144">The cloud PC's service plan ID.</span></span>|
|<span data-ttu-id="5bb16-145">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="5bb16-145">servicePlanName</span></span>|<span data-ttu-id="5bb16-146">String</span><span class="sxs-lookup"><span data-stu-id="5bb16-146">String</span></span>|<span data-ttu-id="5bb16-147">云电脑的服务计划名称。</span><span class="sxs-lookup"><span data-stu-id="5bb16-147">The cloud PC's service plan name.</span></span>|
|<span data-ttu-id="5bb16-148">状态</span><span class="sxs-lookup"><span data-stu-id="5bb16-148">status</span></span>|[<span data-ttu-id="5bb16-149">cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="5bb16-149">cloudPcStatus</span></span>](#cloudpcstatus-values)|<span data-ttu-id="5bb16-150">云电脑的状态。</span><span class="sxs-lookup"><span data-stu-id="5bb16-150">Status of the cloud PC.</span></span> <span data-ttu-id="5bb16-151">可取值为：`notProvisioned`、`provisioning`、`provisioned`、`upgrading`、`inGracePeriod`、`deprovisioning` 或 `failed`。</span><span class="sxs-lookup"><span data-stu-id="5bb16-151">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span></span>|
|<span data-ttu-id="5bb16-152">statusDetails</span><span class="sxs-lookup"><span data-stu-id="5bb16-152">statusDetails</span></span>|[<span data-ttu-id="5bb16-153">cloudPcStatusDetails</span><span class="sxs-lookup"><span data-stu-id="5bb16-153">cloudPcStatusDetails</span></span>](../resources/cloudpcstatusdetails.md)|<span data-ttu-id="5bb16-154">云电脑状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5bb16-154">The details of the cloud PC status.</span></span>|
|<span data-ttu-id="5bb16-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5bb16-155">userPrincipalName</span></span>|<span data-ttu-id="5bb16-156">String</span><span class="sxs-lookup"><span data-stu-id="5bb16-156">String</span></span>|<span data-ttu-id="5bb16-157">用户主体名称 (分配给) 电脑的用户的 UPN 名称。</span><span class="sxs-lookup"><span data-stu-id="5bb16-157">The user principal name (UPN) of the user assigned to the cloud PC.</span></span>|
|<span data-ttu-id="5bb16-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5bb16-158">lastModifiedDateTime</span></span>|<span data-ttu-id="5bb16-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bb16-159">DateTimeOffset</span></span>|<span data-ttu-id="5bb16-160">云电脑上次修改的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5bb16-160">The cloud PC's last modified date and time.</span></span> <span data-ttu-id="5bb16-161">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="5bb16-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5bb16-162">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="5bb16-162">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|

### <a name="cloudpcstatus-values"></a><span data-ttu-id="5bb16-163">cloudPcStatus 值</span><span class="sxs-lookup"><span data-stu-id="5bb16-163">cloudPcStatus values</span></span>

|<span data-ttu-id="5bb16-164">成员</span><span class="sxs-lookup"><span data-stu-id="5bb16-164">Member</span></span>|<span data-ttu-id="5bb16-165">说明</span><span class="sxs-lookup"><span data-stu-id="5bb16-165">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5bb16-166">notProvisioned</span><span class="sxs-lookup"><span data-stu-id="5bb16-166">notProvisioned</span></span>|<span data-ttu-id="5bb16-167">尚未预配云电脑。</span><span class="sxs-lookup"><span data-stu-id="5bb16-167">The Cloud PC hasn’t been provisioned.</span></span>|
|<span data-ttu-id="5bb16-168">预配</span><span class="sxs-lookup"><span data-stu-id="5bb16-168">provisioning</span></span>|<span data-ttu-id="5bb16-169">云电脑预配正在进行中。</span><span class="sxs-lookup"><span data-stu-id="5bb16-169">Cloud PC provisioning is in progress.</span></span>|
|<span data-ttu-id="5bb16-170">已设置</span><span class="sxs-lookup"><span data-stu-id="5bb16-170">provisioned</span></span>|<span data-ttu-id="5bb16-171">云电脑已预配，最终用户可以访问它。</span><span class="sxs-lookup"><span data-stu-id="5bb16-171">The Cloud PC is provisioned and can be accessed by end users.</span></span>|
|<span data-ttu-id="5bb16-172">升级</span><span class="sxs-lookup"><span data-stu-id="5bb16-172">upgrading</span></span>|<span data-ttu-id="5bb16-173">云电脑大小调整正在进行中。</span><span class="sxs-lookup"><span data-stu-id="5bb16-173">Cloud PC resize is in progress.</span></span>|
|<span data-ttu-id="5bb16-174">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="5bb16-174">inGracePeriod</span></span>|<span data-ttu-id="5bb16-175">云电脑在取消预配前的一周宽限期内。</span><span class="sxs-lookup"><span data-stu-id="5bb16-175">The Cloud PC is in the one week grace period before it’s deprovisioned.</span></span>|
|<span data-ttu-id="5bb16-176">取消设置</span><span class="sxs-lookup"><span data-stu-id="5bb16-176">deprovisioning</span></span>|<span data-ttu-id="5bb16-177">云电脑正在取消预配。</span><span class="sxs-lookup"><span data-stu-id="5bb16-177">The Cloud PC is deprovisioning.</span></span>|
|<span data-ttu-id="5bb16-178">failed</span><span class="sxs-lookup"><span data-stu-id="5bb16-178">failed</span></span>|<span data-ttu-id="5bb16-179">云电脑上的操作失败。</span><span class="sxs-lookup"><span data-stu-id="5bb16-179">The operation on Cloud PC has failed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5bb16-180">关系</span><span class="sxs-lookup"><span data-stu-id="5bb16-180">Relationships</span></span>

<span data-ttu-id="5bb16-181">无。</span><span class="sxs-lookup"><span data-stu-id="5bb16-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5bb16-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5bb16-182">JSON representation</span></span>

<span data-ttu-id="5bb16-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5bb16-183">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPC",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPC",
  "id": "String (identifier)",
  "displayName": "String",
  "imageDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "provisioningPolicyId": "String",
  "servicePlanId": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```
