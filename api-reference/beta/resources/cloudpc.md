---
title: cloudPC 资源类型
description: 云托管虚拟桌面。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 1b026bccd18af0dcbc9c0a5128595399a0997474
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50033916"
---
# <a name="cloudpc-resource-type"></a><span data-ttu-id="ae62c-103">cloudPC 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae62c-103">cloudPC resource type</span></span>

<span data-ttu-id="ae62c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae62c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae62c-105">表示云托管虚拟桌面。</span><span class="sxs-lookup"><span data-stu-id="ae62c-105">Represents a cloud-managed virtual desktop.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="ae62c-106">方法</span><span class="sxs-lookup"><span data-stu-id="ae62c-106">Methods</span></span>

|<span data-ttu-id="ae62c-107">方法</span><span class="sxs-lookup"><span data-stu-id="ae62c-107">Method</span></span>|<span data-ttu-id="ae62c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ae62c-108">Return type</span></span>|<span data-ttu-id="ae62c-109">说明</span><span class="sxs-lookup"><span data-stu-id="ae62c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ae62c-110">列出 cloudPCs</span><span class="sxs-lookup"><span data-stu-id="ae62c-110">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="ae62c-111">[cloudPC](../resources/cloudpc.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ae62c-111">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="ae62c-112">列出 cloudPC 对象 [的属性和](../resources/cloudpc.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="ae62c-112">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="ae62c-113">获取 cloudPC</span><span class="sxs-lookup"><span data-stu-id="ae62c-113">Get cloudPC</span></span>](../api/cloudpc-get.md)|[<span data-ttu-id="ae62c-114">cloudPC</span><span class="sxs-lookup"><span data-stu-id="ae62c-114">cloudPC</span></span>](../resources/cloudpc.md)|<span data-ttu-id="ae62c-115">读取 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ae62c-115">Read the properties and relationships of a [cloudPC](../resources/cloudpc.md) object.</span></span>|
|[<span data-ttu-id="ae62c-116">重新设置</span><span class="sxs-lookup"><span data-stu-id="ae62c-116">Reprovision</span></span>](../api/cloudpc-reprovision.md)|<span data-ttu-id="ae62c-117">无</span><span class="sxs-lookup"><span data-stu-id="ae62c-117">None</span></span>|<span data-ttu-id="ae62c-118">重新设置 [cloudPC](../resources/cloudpc.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ae62c-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ae62c-119">属性</span><span class="sxs-lookup"><span data-stu-id="ae62c-119">Properties</span></span>

|<span data-ttu-id="ae62c-120">属性</span><span class="sxs-lookup"><span data-stu-id="ae62c-120">Property</span></span>|<span data-ttu-id="ae62c-121">类型</span><span class="sxs-lookup"><span data-stu-id="ae62c-121">Type</span></span>|<span data-ttu-id="ae62c-122">说明</span><span class="sxs-lookup"><span data-stu-id="ae62c-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae62c-123">id</span><span class="sxs-lookup"><span data-stu-id="ae62c-123">id</span></span>|<span data-ttu-id="ae62c-124">String</span><span class="sxs-lookup"><span data-stu-id="ae62c-124">String</span></span>|<span data-ttu-id="ae62c-125">云电脑的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ae62c-125">Unique identifier for the cloud PC.</span></span> <span data-ttu-id="ae62c-126">只读。</span><span class="sxs-lookup"><span data-stu-id="ae62c-126">Read-only.</span></span>|
|<span data-ttu-id="ae62c-127">displayName</span><span class="sxs-lookup"><span data-stu-id="ae62c-127">displayName</span></span>|<span data-ttu-id="ae62c-128">String</span><span class="sxs-lookup"><span data-stu-id="ae62c-128">String</span></span>|<span data-ttu-id="ae62c-129">云电脑显示名称。</span><span class="sxs-lookup"><span data-stu-id="ae62c-129">The cloud PC display name.</span></span>|
|<span data-ttu-id="ae62c-130">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="ae62c-130">imageDisplayName</span></span>|<span data-ttu-id="ae62c-131">String</span><span class="sxs-lookup"><span data-stu-id="ae62c-131">String</span></span>|<span data-ttu-id="ae62c-132">云电脑上的操作系统映像的名称。</span><span class="sxs-lookup"><span data-stu-id="ae62c-132">Name of the OS image that's on the cloud PC.</span></span>|
|<span data-ttu-id="ae62c-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="ae62c-133">managedDeviceId</span></span>|<span data-ttu-id="ae62c-134">String</span><span class="sxs-lookup"><span data-stu-id="ae62c-134">String</span></span>|<span data-ttu-id="ae62c-135">云电脑的 Intune 设备 ID。</span><span class="sxs-lookup"><span data-stu-id="ae62c-135">The cloud PC’s Intune device ID.</span></span>|
|<span data-ttu-id="ae62c-136">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="ae62c-136">managedDeviceName</span></span>|<span data-ttu-id="ae62c-137">String</span><span class="sxs-lookup"><span data-stu-id="ae62c-137">String</span></span>|<span data-ttu-id="ae62c-138">云电脑的 Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="ae62c-138">The cloud PC’s Intune device name.</span></span>|
|<span data-ttu-id="ae62c-139">provisioningPolicyId</span><span class="sxs-lookup"><span data-stu-id="ae62c-139">provisioningPolicyId</span></span>|<span data-ttu-id="ae62c-140">String</span><span class="sxs-lookup"><span data-stu-id="ae62c-140">String</span></span>|<span data-ttu-id="ae62c-141">云电脑的预配策略 ID。</span><span class="sxs-lookup"><span data-stu-id="ae62c-141">The cloud PC's provisioning policy ID.</span></span>|
|<span data-ttu-id="ae62c-142">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="ae62c-142">servicePlanId</span></span>|<span data-ttu-id="ae62c-143">String</span><span class="sxs-lookup"><span data-stu-id="ae62c-143">String</span></span>|<span data-ttu-id="ae62c-144">云电脑的服务计划 ID。</span><span class="sxs-lookup"><span data-stu-id="ae62c-144">The cloud PC's service plan ID.</span></span>|
|<span data-ttu-id="ae62c-145">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="ae62c-145">servicePlanName</span></span>|<span data-ttu-id="ae62c-146">String</span><span class="sxs-lookup"><span data-stu-id="ae62c-146">String</span></span>|<span data-ttu-id="ae62c-147">云电脑的服务计划名称。</span><span class="sxs-lookup"><span data-stu-id="ae62c-147">The cloud PC's service plan name.</span></span>|
|<span data-ttu-id="ae62c-148">状态</span><span class="sxs-lookup"><span data-stu-id="ae62c-148">status</span></span>|[<span data-ttu-id="ae62c-149">cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="ae62c-149">cloudPcStatus</span></span>](#cloudpcstatus-values)|<span data-ttu-id="ae62c-150">云电脑的状态。</span><span class="sxs-lookup"><span data-stu-id="ae62c-150">Status of the cloud PC.</span></span> <span data-ttu-id="ae62c-151">可取值为：`notProvisioned`、`provisioning`、`provisioned`、`upgrading`、`inGracePeriod`、`deprovisioning` 或 `failed`。</span><span class="sxs-lookup"><span data-stu-id="ae62c-151">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span></span>|
|<span data-ttu-id="ae62c-152">statusDetails</span><span class="sxs-lookup"><span data-stu-id="ae62c-152">statusDetails</span></span>|[<span data-ttu-id="ae62c-153">cloudPcStatusDetails</span><span class="sxs-lookup"><span data-stu-id="ae62c-153">cloudPcStatusDetails</span></span>](../resources/cloudpcstatusdetails.md)|<span data-ttu-id="ae62c-154">云电脑状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ae62c-154">The details of the cloud PC status.</span></span>|
|<span data-ttu-id="ae62c-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ae62c-155">userPrincipalName</span></span>|<span data-ttu-id="ae62c-156">String</span><span class="sxs-lookup"><span data-stu-id="ae62c-156">String</span></span>|<span data-ttu-id="ae62c-157">用户主体名称 (分配给) 电脑的用户的 UPN 名称。</span><span class="sxs-lookup"><span data-stu-id="ae62c-157">The user principal name (UPN) of the user assigned to the cloud PC.</span></span>|
|<span data-ttu-id="ae62c-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae62c-158">lastModifiedDateTime</span></span>|<span data-ttu-id="ae62c-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae62c-159">DateTimeOffset</span></span>|<span data-ttu-id="ae62c-160">云电脑上次修改的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ae62c-160">The cloud PC's last modified date and time.</span></span> <span data-ttu-id="ae62c-161">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ae62c-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ae62c-162">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="ae62c-162">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

### <a name="cloudpcstatus-values"></a><span data-ttu-id="ae62c-163">cloudPcStatus 值</span><span class="sxs-lookup"><span data-stu-id="ae62c-163">cloudPcStatus values</span></span>

|<span data-ttu-id="ae62c-164">成员</span><span class="sxs-lookup"><span data-stu-id="ae62c-164">Member</span></span>|<span data-ttu-id="ae62c-165">说明</span><span class="sxs-lookup"><span data-stu-id="ae62c-165">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ae62c-166">notProvisioned</span><span class="sxs-lookup"><span data-stu-id="ae62c-166">notProvisioned</span></span>|<span data-ttu-id="ae62c-167">尚未预配云电脑。</span><span class="sxs-lookup"><span data-stu-id="ae62c-167">The Cloud PC hasn’t been provisioned.</span></span>|
|<span data-ttu-id="ae62c-168">预配</span><span class="sxs-lookup"><span data-stu-id="ae62c-168">provisioning</span></span>|<span data-ttu-id="ae62c-169">云电脑预配正在进行中。</span><span class="sxs-lookup"><span data-stu-id="ae62c-169">Cloud PC provisioning is in progress.</span></span>|
|<span data-ttu-id="ae62c-170">已设置</span><span class="sxs-lookup"><span data-stu-id="ae62c-170">provisioned</span></span>|<span data-ttu-id="ae62c-171">云电脑已预配，最终用户可以访问它。</span><span class="sxs-lookup"><span data-stu-id="ae62c-171">The Cloud PC is provisioned and can be accessed by end users.</span></span>|
|<span data-ttu-id="ae62c-172">升级</span><span class="sxs-lookup"><span data-stu-id="ae62c-172">upgrading</span></span>|<span data-ttu-id="ae62c-173">云电脑调整大小正在进行中。</span><span class="sxs-lookup"><span data-stu-id="ae62c-173">Cloud PC resize is in progress.</span></span>|
|<span data-ttu-id="ae62c-174">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="ae62c-174">inGracePeriod</span></span>|<span data-ttu-id="ae62c-175">云电脑在取消设置前有一周的宽限期。</span><span class="sxs-lookup"><span data-stu-id="ae62c-175">The Cloud PC is in the one week grace period before it’s deprovisioned.</span></span>|
|<span data-ttu-id="ae62c-176">取消设置</span><span class="sxs-lookup"><span data-stu-id="ae62c-176">deprovisioning</span></span>|<span data-ttu-id="ae62c-177">云电脑正在取消设置。</span><span class="sxs-lookup"><span data-stu-id="ae62c-177">The Cloud PC is deprovisioning.</span></span>|
|<span data-ttu-id="ae62c-178">failed</span><span class="sxs-lookup"><span data-stu-id="ae62c-178">failed</span></span>|<span data-ttu-id="ae62c-179">云电脑上的操作失败。</span><span class="sxs-lookup"><span data-stu-id="ae62c-179">The operation on Cloud PC has failed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae62c-180">关系</span><span class="sxs-lookup"><span data-stu-id="ae62c-180">Relationships</span></span>

<span data-ttu-id="ae62c-181">无。</span><span class="sxs-lookup"><span data-stu-id="ae62c-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae62c-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae62c-182">JSON representation</span></span>

<span data-ttu-id="ae62c-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae62c-183">The following is a JSON representation of the resource.</span></span>
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
