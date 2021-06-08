---
title: cloudPC 资源类型
description: 云托管虚拟桌面。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 232ad6a8de6634f028ec59080114110c902ce184
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787497"
---
# <a name="cloudpc-resource-type"></a><span data-ttu-id="b6bc7-103">cloudPC 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6bc7-103">cloudPC resource type</span></span>

<span data-ttu-id="b6bc7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6bc7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6bc7-105">表示云托管虚拟桌面。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-105">Represents a cloud-managed virtual desktop.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="b6bc7-106">方法</span><span class="sxs-lookup"><span data-stu-id="b6bc7-106">Methods</span></span>

|<span data-ttu-id="b6bc7-107">方法</span><span class="sxs-lookup"><span data-stu-id="b6bc7-107">Method</span></span>|<span data-ttu-id="b6bc7-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b6bc7-108">Return type</span></span>|<span data-ttu-id="b6bc7-109">说明</span><span class="sxs-lookup"><span data-stu-id="b6bc7-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b6bc7-110">列出 cloudPCs</span><span class="sxs-lookup"><span data-stu-id="b6bc7-110">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="b6bc7-111">[cloudPC](../resources/cloudpc.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b6bc7-111">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="b6bc7-112">列出 [cloudPC 对象的属性和](../resources/cloudpc.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-112">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="b6bc7-113">获取 cloudPC</span><span class="sxs-lookup"><span data-stu-id="b6bc7-113">Get cloudPC</span></span>](../api/cloudpc-get.md)|[<span data-ttu-id="b6bc7-114">cloudPC</span><span class="sxs-lookup"><span data-stu-id="b6bc7-114">cloudPC</span></span>](../resources/cloudpc.md)|<span data-ttu-id="b6bc7-115">读取 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-115">Read the properties and relationships of a [cloudPC](../resources/cloudpc.md) object.</span></span>|
|[<span data-ttu-id="b6bc7-116">重新设置</span><span class="sxs-lookup"><span data-stu-id="b6bc7-116">Reprovision</span></span>](../api/cloudpc-reprovision.md)|<span data-ttu-id="b6bc7-117">无</span><span class="sxs-lookup"><span data-stu-id="b6bc7-117">None</span></span>|<span data-ttu-id="b6bc7-118">重新设置 [cloudPC](../resources/cloudpc.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b6bc7-119">属性</span><span class="sxs-lookup"><span data-stu-id="b6bc7-119">Properties</span></span>

|<span data-ttu-id="b6bc7-120">属性</span><span class="sxs-lookup"><span data-stu-id="b6bc7-120">Property</span></span>|<span data-ttu-id="b6bc7-121">类型</span><span class="sxs-lookup"><span data-stu-id="b6bc7-121">Type</span></span>|<span data-ttu-id="b6bc7-122">说明</span><span class="sxs-lookup"><span data-stu-id="b6bc7-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6bc7-123">id</span><span class="sxs-lookup"><span data-stu-id="b6bc7-123">id</span></span>|<span data-ttu-id="b6bc7-124">String</span><span class="sxs-lookup"><span data-stu-id="b6bc7-124">String</span></span>|<span data-ttu-id="b6bc7-125">云电脑的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-125">Unique identifier for the cloud PC.</span></span> <span data-ttu-id="b6bc7-126">只读。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-126">Read-only.</span></span>|
|<span data-ttu-id="b6bc7-127">displayName</span><span class="sxs-lookup"><span data-stu-id="b6bc7-127">displayName</span></span>|<span data-ttu-id="b6bc7-128">String</span><span class="sxs-lookup"><span data-stu-id="b6bc7-128">String</span></span>|<span data-ttu-id="b6bc7-129">云电脑显示名称。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-129">The cloud PC display name.</span></span>|
|<span data-ttu-id="b6bc7-130">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="b6bc7-130">imageDisplayName</span></span>|<span data-ttu-id="b6bc7-131">String</span><span class="sxs-lookup"><span data-stu-id="b6bc7-131">String</span></span>|<span data-ttu-id="b6bc7-132">云电脑上的操作系统映像的名称。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-132">Name of the OS image that's on the cloud PC.</span></span>|
|<span data-ttu-id="b6bc7-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="b6bc7-133">managedDeviceId</span></span>|<span data-ttu-id="b6bc7-134">String</span><span class="sxs-lookup"><span data-stu-id="b6bc7-134">String</span></span>|<span data-ttu-id="b6bc7-135">云电脑的 Intune 设备 ID。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-135">The cloud PC’s Intune device ID.</span></span>|
|<span data-ttu-id="b6bc7-136">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="b6bc7-136">managedDeviceName</span></span>|<span data-ttu-id="b6bc7-137">String</span><span class="sxs-lookup"><span data-stu-id="b6bc7-137">String</span></span>|<span data-ttu-id="b6bc7-138">云电脑的 Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-138">The cloud PC’s Intune device name.</span></span>|
|<span data-ttu-id="b6bc7-139">provisioningPolicyId</span><span class="sxs-lookup"><span data-stu-id="b6bc7-139">provisioningPolicyId</span></span>|<span data-ttu-id="b6bc7-140">String</span><span class="sxs-lookup"><span data-stu-id="b6bc7-140">String</span></span>|<span data-ttu-id="b6bc7-141">云电脑的预配策略 ID。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-141">The cloud PC's provisioning policy ID.</span></span>|
|<span data-ttu-id="b6bc7-142">provisioningPolicyName</span><span class="sxs-lookup"><span data-stu-id="b6bc7-142">provisioningPolicyName</span></span>|<span data-ttu-id="b6bc7-143">String</span><span class="sxs-lookup"><span data-stu-id="b6bc7-143">String</span></span>|<span data-ttu-id="b6bc7-144">预配云电脑期间应用的预配策略。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-144">The provisioning policy that is applied during provisioning of cloud PCs.</span></span>|
|<span data-ttu-id="b6bc7-145">onPremisesConnectionName</span><span class="sxs-lookup"><span data-stu-id="b6bc7-145">onPremisesConnectionName</span></span>|<span data-ttu-id="b6bc7-146">String</span><span class="sxs-lookup"><span data-stu-id="b6bc7-146">String</span></span>|<span data-ttu-id="b6bc7-147">预配云电脑期间应用本地连接。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-147">The on-premises connection that is applied during provisioning of cloud PCs.</span></span>|
|<span data-ttu-id="b6bc7-148">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="b6bc7-148">servicePlanId</span></span>|<span data-ttu-id="b6bc7-149">String</span><span class="sxs-lookup"><span data-stu-id="b6bc7-149">String</span></span>|<span data-ttu-id="b6bc7-150">云电脑的服务计划 ID。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-150">The cloud PC's service plan ID.</span></span>|
|<span data-ttu-id="b6bc7-151">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="b6bc7-151">servicePlanName</span></span>|<span data-ttu-id="b6bc7-152">String</span><span class="sxs-lookup"><span data-stu-id="b6bc7-152">String</span></span>|<span data-ttu-id="b6bc7-153">云电脑的服务计划名称。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-153">The cloud PC's service plan name.</span></span>|
|<span data-ttu-id="b6bc7-154">状态</span><span class="sxs-lookup"><span data-stu-id="b6bc7-154">status</span></span>|[<span data-ttu-id="b6bc7-155">cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="b6bc7-155">cloudPcStatus</span></span>](#cloudpcstatus-values)|<span data-ttu-id="b6bc7-156">云电脑的状态。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-156">Status of the cloud PC.</span></span> <span data-ttu-id="b6bc7-157">可取值为：`notProvisioned`、`provisioning`、`provisioned`、`upgrading`、`inGracePeriod`、`deprovisioning` 或 `failed`。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-157">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span></span>|
|<span data-ttu-id="b6bc7-158">statusDetails</span><span class="sxs-lookup"><span data-stu-id="b6bc7-158">statusDetails</span></span>|[<span data-ttu-id="b6bc7-159">cloudPcStatusDetails</span><span class="sxs-lookup"><span data-stu-id="b6bc7-159">cloudPcStatusDetails</span></span>](../resources/cloudpcstatusdetails.md)|<span data-ttu-id="b6bc7-160">云电脑状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-160">The details of the cloud PC status.</span></span>|
|<span data-ttu-id="b6bc7-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b6bc7-161">userPrincipalName</span></span>|<span data-ttu-id="b6bc7-162">String</span><span class="sxs-lookup"><span data-stu-id="b6bc7-162">String</span></span>|<span data-ttu-id="b6bc7-163">用户主体名称 (分配给) 电脑的用户的 UPN 名称。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-163">The user principal name (UPN) of the user assigned to the cloud PC.</span></span>|
|<span data-ttu-id="b6bc7-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6bc7-164">lastModifiedDateTime</span></span>|<span data-ttu-id="b6bc7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6bc7-165">DateTimeOffset</span></span>|<span data-ttu-id="b6bc7-166">云电脑上次修改的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-166">The cloud PC's last modified date and time.</span></span> <span data-ttu-id="b6bc7-167">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-167">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b6bc7-168">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-168">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="b6bc7-169">gracePeriodEndDateTime</span><span class="sxs-lookup"><span data-stu-id="b6bc7-169">gracePeriodEndDateTime</span></span>|<span data-ttu-id="b6bc7-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6bc7-170">DateTimeOffset</span></span>|<span data-ttu-id="b6bc7-171">宽限期结束和重新设置/取消设置发生的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-171">The date and time when the grace period ends and reprovisioning/deprovisioning happens.</span></span> <span data-ttu-id="b6bc7-172">仅在 status 为 时是必需的 `inGracePeriod` 。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-172">Required only if status is `inGracePeriod`.</span></span> <span data-ttu-id="b6bc7-173">时间戳以 ISO 8601 格式和 UTC 协调世界时 (显示) 。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-173">The timestamp is shown in ISO 8601 format and Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="b6bc7-174">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-174">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|

### <a name="cloudpcstatus-values"></a><span data-ttu-id="b6bc7-175">cloudPcStatus 值</span><span class="sxs-lookup"><span data-stu-id="b6bc7-175">cloudPcStatus values</span></span>

|<span data-ttu-id="b6bc7-176">成员</span><span class="sxs-lookup"><span data-stu-id="b6bc7-176">Member</span></span>|<span data-ttu-id="b6bc7-177">说明</span><span class="sxs-lookup"><span data-stu-id="b6bc7-177">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b6bc7-178">notProvisioned</span><span class="sxs-lookup"><span data-stu-id="b6bc7-178">notProvisioned</span></span>|<span data-ttu-id="b6bc7-179">尚未Cloud PC设置该设置。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-179">The Cloud PC hasn’t been provisioned.</span></span>|
|<span data-ttu-id="b6bc7-180">预配</span><span class="sxs-lookup"><span data-stu-id="b6bc7-180">provisioning</span></span>|<span data-ttu-id="b6bc7-181">Cloud PC设置正在进行中。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-181">Cloud PC provisioning is in progress.</span></span>|
|<span data-ttu-id="b6bc7-182">已设置</span><span class="sxs-lookup"><span data-stu-id="b6bc7-182">provisioned</span></span>|<span data-ttu-id="b6bc7-183">此Cloud PC设置，最终用户可以访问它。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-183">The Cloud PC is provisioned and can be accessed by end users.</span></span>|
|<span data-ttu-id="b6bc7-184">升级</span><span class="sxs-lookup"><span data-stu-id="b6bc7-184">upgrading</span></span>|<span data-ttu-id="b6bc7-185">Cloud PC调整大小。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-185">Cloud PC resize is in progress.</span></span>|
|<span data-ttu-id="b6bc7-186">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="b6bc7-186">inGracePeriod</span></span>|<span data-ttu-id="b6bc7-187">该Cloud PC在取消设置前的一周宽限期内。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-187">The Cloud PC is in the one week grace period before it’s deprovisioned.</span></span>|
|<span data-ttu-id="b6bc7-188">取消设置</span><span class="sxs-lookup"><span data-stu-id="b6bc7-188">deprovisioning</span></span>|<span data-ttu-id="b6bc7-189">取消Cloud PC设置。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-189">The Cloud PC is deprovisioning.</span></span>|
|<span data-ttu-id="b6bc7-190">failed</span><span class="sxs-lookup"><span data-stu-id="b6bc7-190">failed</span></span>|<span data-ttu-id="b6bc7-191">对项目Cloud PC失败。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-191">The operation on Cloud PC has failed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6bc7-192">关系</span><span class="sxs-lookup"><span data-stu-id="b6bc7-192">Relationships</span></span>

<span data-ttu-id="b6bc7-193">无。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-193">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6bc7-194">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6bc7-194">JSON representation</span></span>

<span data-ttu-id="b6bc7-195">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6bc7-195">The following is a JSON representation of the resource.</span></span>
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
  "provisioningPolicyName": "String",
  "onPremisesConnectionName": "String",
  "servicePlanId": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "gracePeriodEndDateTime": "String (timestamp)"
}
```
