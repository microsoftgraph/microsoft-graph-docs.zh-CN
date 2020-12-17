---
title: cloudPC 资源类型
description: 云托管虚拟桌面。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 481bcae691632685cafab00a4b7e44addb1ad0cd
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706079"
---
# <a name="cloudpc-resource-type"></a><span data-ttu-id="8ab8f-103">cloudPC 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ab8f-103">cloudPC resource type</span></span>

<span data-ttu-id="8ab8f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ab8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ab8f-105">表示云托管虚拟桌面。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-105">Represents a cloud-managed virtual desktop.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="8ab8f-106">方法</span><span class="sxs-lookup"><span data-stu-id="8ab8f-106">Methods</span></span>

|<span data-ttu-id="8ab8f-107">方法</span><span class="sxs-lookup"><span data-stu-id="8ab8f-107">Method</span></span>|<span data-ttu-id="8ab8f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8ab8f-108">Return type</span></span>|<span data-ttu-id="8ab8f-109">说明</span><span class="sxs-lookup"><span data-stu-id="8ab8f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8ab8f-110">列出 cloudPCs</span><span class="sxs-lookup"><span data-stu-id="8ab8f-110">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="8ab8f-111">[cloudPC](../resources/cloudpc.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ab8f-111">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="8ab8f-112">列出 cloudPC 对象 [的属性和](../resources/cloudpc.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-112">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="8ab8f-113">获取 cloudPC</span><span class="sxs-lookup"><span data-stu-id="8ab8f-113">Get cloudPC</span></span>](../api/cloudpc-get.md)|[<span data-ttu-id="8ab8f-114">cloudPC</span><span class="sxs-lookup"><span data-stu-id="8ab8f-114">cloudPC</span></span>](../resources/cloudpc.md)|<span data-ttu-id="8ab8f-115">读取 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-115">Read the properties and relationships of a [cloudPC](../resources/cloudpc.md) object.</span></span>|
|[<span data-ttu-id="8ab8f-116">重新设置</span><span class="sxs-lookup"><span data-stu-id="8ab8f-116">Reprovision</span></span>](../api/cloudpc-reprovision.md)|<span data-ttu-id="8ab8f-117">无</span><span class="sxs-lookup"><span data-stu-id="8ab8f-117">None</span></span>|<span data-ttu-id="8ab8f-118">重新设置 [cloudPC](../resources/cloudpc.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8ab8f-119">属性</span><span class="sxs-lookup"><span data-stu-id="8ab8f-119">Properties</span></span>

|<span data-ttu-id="8ab8f-120">属性</span><span class="sxs-lookup"><span data-stu-id="8ab8f-120">Property</span></span>|<span data-ttu-id="8ab8f-121">类型</span><span class="sxs-lookup"><span data-stu-id="8ab8f-121">Type</span></span>|<span data-ttu-id="8ab8f-122">说明</span><span class="sxs-lookup"><span data-stu-id="8ab8f-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ab8f-123">id</span><span class="sxs-lookup"><span data-stu-id="8ab8f-123">id</span></span>|<span data-ttu-id="8ab8f-124">字符串</span><span class="sxs-lookup"><span data-stu-id="8ab8f-124">String</span></span>|<span data-ttu-id="8ab8f-125">云电脑的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-125">Unique identifier for the cloud PC.</span></span> <span data-ttu-id="8ab8f-126">只读。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-126">Read-only.</span></span>|
|<span data-ttu-id="8ab8f-127">displayName</span><span class="sxs-lookup"><span data-stu-id="8ab8f-127">displayName</span></span>|<span data-ttu-id="8ab8f-128">字符串</span><span class="sxs-lookup"><span data-stu-id="8ab8f-128">String</span></span>|<span data-ttu-id="8ab8f-129">云电脑显示名称。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-129">The cloud PC display name.</span></span>|
|<span data-ttu-id="8ab8f-130">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="8ab8f-130">imageDisplayName</span></span>|<span data-ttu-id="8ab8f-131">字符串</span><span class="sxs-lookup"><span data-stu-id="8ab8f-131">String</span></span>|<span data-ttu-id="8ab8f-132">云电脑上的操作系统映像的名称。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-132">Name of the OS image that's on the cloud PC.</span></span>|
|<span data-ttu-id="8ab8f-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="8ab8f-133">managedDeviceId</span></span>|<span data-ttu-id="8ab8f-134">字符串</span><span class="sxs-lookup"><span data-stu-id="8ab8f-134">String</span></span>|<span data-ttu-id="8ab8f-135">云电脑的 Intune 设备 ID。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-135">The cloud PC’s Intune device ID.</span></span>|
|<span data-ttu-id="8ab8f-136">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="8ab8f-136">managedDeviceName</span></span>|<span data-ttu-id="8ab8f-137">String</span><span class="sxs-lookup"><span data-stu-id="8ab8f-137">String</span></span>|<span data-ttu-id="8ab8f-138">云电脑的 Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-138">The cloud PC’s Intune device name.</span></span>|
|<span data-ttu-id="8ab8f-139">provisioningPolicyId</span><span class="sxs-lookup"><span data-stu-id="8ab8f-139">provisioningPolicyId</span></span>|<span data-ttu-id="8ab8f-140">字符串</span><span class="sxs-lookup"><span data-stu-id="8ab8f-140">String</span></span>|<span data-ttu-id="8ab8f-141">云电脑的预配策略 ID。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-141">The cloud PC's provisioning policy ID.</span></span>|
|<span data-ttu-id="8ab8f-142">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="8ab8f-142">servicePlanId</span></span>|<span data-ttu-id="8ab8f-143">字符串</span><span class="sxs-lookup"><span data-stu-id="8ab8f-143">String</span></span>|<span data-ttu-id="8ab8f-144">云电脑的服务计划 ID。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-144">The cloud PC's service plan ID.</span></span>|
|<span data-ttu-id="8ab8f-145">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="8ab8f-145">servicePlanName</span></span>|<span data-ttu-id="8ab8f-146">String</span><span class="sxs-lookup"><span data-stu-id="8ab8f-146">String</span></span>|<span data-ttu-id="8ab8f-147">云电脑的服务计划名称。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-147">The cloud PC's service plan name.</span></span>|
|<span data-ttu-id="8ab8f-148">status</span><span class="sxs-lookup"><span data-stu-id="8ab8f-148">status</span></span>|<span data-ttu-id="8ab8f-149">cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="8ab8f-149">cloudPcStatus</span></span>|<span data-ttu-id="8ab8f-150">云电脑的状态。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-150">Status of the cloud PC.</span></span> <span data-ttu-id="8ab8f-151">可取值为：`notProvisioned`、`provisioning`、`provisioned`、`upgrading`、`inGracePeriod`、`deprovisioning` 或 `failed`。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-151">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span></span>|
|<span data-ttu-id="8ab8f-152">statusDetails</span><span class="sxs-lookup"><span data-stu-id="8ab8f-152">statusDetails</span></span>|[<span data-ttu-id="8ab8f-153">cloudPcStatusDetails</span><span class="sxs-lookup"><span data-stu-id="8ab8f-153">cloudPcStatusDetails</span></span>](../resources/cloudpcstatusdetails.md)|<span data-ttu-id="8ab8f-154">云电脑状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-154">The details of the cloud PC status.</span></span>|
|<span data-ttu-id="8ab8f-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8ab8f-155">userPrincipalName</span></span>|<span data-ttu-id="8ab8f-156">字符串</span><span class="sxs-lookup"><span data-stu-id="8ab8f-156">String</span></span>|<span data-ttu-id="8ab8f-157">用户主体名称 (分配给) 电脑的用户的 UPN 名称。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-157">The user principal name (UPN) of the user assigned to the cloud PC.</span></span>|
|<span data-ttu-id="8ab8f-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ab8f-158">lastModifiedDateTime</span></span>|<span data-ttu-id="8ab8f-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ab8f-159">DateTimeOffset</span></span>|<span data-ttu-id="8ab8f-160">云电脑上次修改的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-160">The cloud PC's last modified date and time.</span></span> <span data-ttu-id="8ab8f-161">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8ab8f-162">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-162">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ab8f-163">关系</span><span class="sxs-lookup"><span data-stu-id="8ab8f-163">Relationships</span></span>

<span data-ttu-id="8ab8f-164">无。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-164">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ab8f-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ab8f-165">JSON representation</span></span>

<span data-ttu-id="8ab8f-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ab8f-166">The following is a JSON representation of the resource.</span></span>
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
