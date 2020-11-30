---
title: cloudPC 资源类型
description: 云托管虚拟桌面。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 95758299f87ac463bac6fdc30f7d70fb59eb6c92
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378317"
---
# <a name="cloudpc-resource-type"></a><span data-ttu-id="3e97d-103">cloudPC 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e97d-103">cloudPC resource type</span></span>

<span data-ttu-id="3e97d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e97d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e97d-105">表示云管理的虚拟桌面。</span><span class="sxs-lookup"><span data-stu-id="3e97d-105">Represents a cloud-managed virtual desktop.</span></span>

## <a name="methods"></a><span data-ttu-id="3e97d-106">Methods</span><span class="sxs-lookup"><span data-stu-id="3e97d-106">Methods</span></span>

|<span data-ttu-id="3e97d-107">方法</span><span class="sxs-lookup"><span data-stu-id="3e97d-107">Method</span></span>|<span data-ttu-id="3e97d-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3e97d-108">Return type</span></span>|<span data-ttu-id="3e97d-109">说明</span><span class="sxs-lookup"><span data-stu-id="3e97d-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3e97d-110">列出 cloudPCs</span><span class="sxs-lookup"><span data-stu-id="3e97d-110">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="3e97d-111">[cloudPC](../resources/cloudpc.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3e97d-111">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="3e97d-112">列出 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3e97d-112">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="3e97d-113">获取 cloudPC</span><span class="sxs-lookup"><span data-stu-id="3e97d-113">Get cloudPC</span></span>](../api/cloudpc-get.md)|[<span data-ttu-id="3e97d-114">cloudPC</span><span class="sxs-lookup"><span data-stu-id="3e97d-114">cloudPC</span></span>](../resources/cloudpc.md)|<span data-ttu-id="3e97d-115">读取 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3e97d-115">Read the properties and relationships of a [cloudPC](../resources/cloudpc.md) object.</span></span>|
|[<span data-ttu-id="3e97d-116">重新设置</span><span class="sxs-lookup"><span data-stu-id="3e97d-116">Reprovision</span></span>](../api/cloudpc-reprovision.md)|<span data-ttu-id="3e97d-117">无</span><span class="sxs-lookup"><span data-stu-id="3e97d-117">None</span></span>|<span data-ttu-id="3e97d-118">重新设置一个 [cloudPC](../resources/cloudpc.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3e97d-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3e97d-119">属性</span><span class="sxs-lookup"><span data-stu-id="3e97d-119">Properties</span></span>

|<span data-ttu-id="3e97d-120">属性</span><span class="sxs-lookup"><span data-stu-id="3e97d-120">Property</span></span>|<span data-ttu-id="3e97d-121">类型</span><span class="sxs-lookup"><span data-stu-id="3e97d-121">Type</span></span>|<span data-ttu-id="3e97d-122">说明</span><span class="sxs-lookup"><span data-stu-id="3e97d-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e97d-123">id</span><span class="sxs-lookup"><span data-stu-id="3e97d-123">id</span></span>|<span data-ttu-id="3e97d-124">字符串</span><span class="sxs-lookup"><span data-stu-id="3e97d-124">String</span></span>|<span data-ttu-id="3e97d-125">云电脑的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3e97d-125">Unique identifier for the cloud PC.</span></span> <span data-ttu-id="3e97d-126">只读。</span><span class="sxs-lookup"><span data-stu-id="3e97d-126">Read-only.</span></span>|
|<span data-ttu-id="3e97d-127">displayName</span><span class="sxs-lookup"><span data-stu-id="3e97d-127">displayName</span></span>|<span data-ttu-id="3e97d-128">字符串</span><span class="sxs-lookup"><span data-stu-id="3e97d-128">String</span></span>|<span data-ttu-id="3e97d-129">云电脑显示名称。</span><span class="sxs-lookup"><span data-stu-id="3e97d-129">The cloud PC display name.</span></span>|
|<span data-ttu-id="3e97d-130">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="3e97d-130">imageDisplayName</span></span>|<span data-ttu-id="3e97d-131">字符串</span><span class="sxs-lookup"><span data-stu-id="3e97d-131">String</span></span>|<span data-ttu-id="3e97d-132">云电脑上的 OS 映像的名称。</span><span class="sxs-lookup"><span data-stu-id="3e97d-132">Name of the OS image that's on the cloud PC.</span></span>|
|<span data-ttu-id="3e97d-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="3e97d-133">managedDeviceId</span></span>|<span data-ttu-id="3e97d-134">字符串</span><span class="sxs-lookup"><span data-stu-id="3e97d-134">String</span></span>|<span data-ttu-id="3e97d-135">云电脑的 Intune 设备 ID。</span><span class="sxs-lookup"><span data-stu-id="3e97d-135">The cloud PC’s Intune device ID.</span></span>|
|<span data-ttu-id="3e97d-136">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="3e97d-136">managedDeviceName</span></span>|<span data-ttu-id="3e97d-137">String</span><span class="sxs-lookup"><span data-stu-id="3e97d-137">String</span></span>|<span data-ttu-id="3e97d-138">云电脑的 Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="3e97d-138">The cloud PC’s Intune device name.</span></span>|
|<span data-ttu-id="3e97d-139">provisioningPolicyId</span><span class="sxs-lookup"><span data-stu-id="3e97d-139">provisioningPolicyId</span></span>|<span data-ttu-id="3e97d-140">字符串</span><span class="sxs-lookup"><span data-stu-id="3e97d-140">String</span></span>|<span data-ttu-id="3e97d-141">云电脑的设置策略 ID。</span><span class="sxs-lookup"><span data-stu-id="3e97d-141">The cloud PC's provisioning policy ID.</span></span>|
|<span data-ttu-id="3e97d-142">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="3e97d-142">servicePlanId</span></span>|<span data-ttu-id="3e97d-143">字符串</span><span class="sxs-lookup"><span data-stu-id="3e97d-143">String</span></span>|<span data-ttu-id="3e97d-144">云电脑的服务计划 ID。</span><span class="sxs-lookup"><span data-stu-id="3e97d-144">The cloud PC's service plan ID.</span></span>|
|<span data-ttu-id="3e97d-145">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="3e97d-145">servicePlanName</span></span>|<span data-ttu-id="3e97d-146">String</span><span class="sxs-lookup"><span data-stu-id="3e97d-146">String</span></span>|<span data-ttu-id="3e97d-147">云电脑的服务计划名称。</span><span class="sxs-lookup"><span data-stu-id="3e97d-147">The cloud PC's service plan name.</span></span>|
|<span data-ttu-id="3e97d-148">status</span><span class="sxs-lookup"><span data-stu-id="3e97d-148">status</span></span>|<span data-ttu-id="3e97d-149">cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="3e97d-149">cloudPcStatus</span></span>|<span data-ttu-id="3e97d-150">云电脑的状态。</span><span class="sxs-lookup"><span data-stu-id="3e97d-150">Status of the cloud PC.</span></span> <span data-ttu-id="3e97d-151">可取值为：`notProvisioned`、`provisioning`、`provisioned`、`upgrading`、`inGracePeriod`、`deprovisioning`、`upgradeFailed`、`provisionFailed`、`deprovisionFailed`、`reprovisionFailed`。</span><span class="sxs-lookup"><span data-stu-id="3e97d-151">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `upgradeFailed`, `provisionFailed`, `deprovisionFailed`, `reprovisionFailed`.</span></span>|
|<span data-ttu-id="3e97d-152">statusDetails</span><span class="sxs-lookup"><span data-stu-id="3e97d-152">statusDetails</span></span>|[<span data-ttu-id="3e97d-153">cloudPcStatusDetails</span><span class="sxs-lookup"><span data-stu-id="3e97d-153">cloudPcStatusDetails</span></span>](../resources/cloudpcstatusdetails.md)|<span data-ttu-id="3e97d-154">云电脑状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3e97d-154">The details of the cloud PC status.</span></span>|
|<span data-ttu-id="3e97d-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3e97d-155">userPrincipalName</span></span>|<span data-ttu-id="3e97d-156">字符串</span><span class="sxs-lookup"><span data-stu-id="3e97d-156">String</span></span>|<span data-ttu-id="3e97d-157">为云电脑分配的用户的用户主体名称 (UPN) 。</span><span class="sxs-lookup"><span data-stu-id="3e97d-157">The user principal name (UPN) of the user assigned to the cloud PC.</span></span>|
|<span data-ttu-id="3e97d-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e97d-158">lastModifiedDateTime</span></span>|<span data-ttu-id="3e97d-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e97d-159">DateTimeOffset</span></span>|<span data-ttu-id="3e97d-160">云电脑的上次修改日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3e97d-160">The cloud PC's last modified date and time.</span></span> <span data-ttu-id="3e97d-161">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="3e97d-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3e97d-162">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="3e97d-162">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e97d-163">关系</span><span class="sxs-lookup"><span data-stu-id="3e97d-163">Relationships</span></span>

<span data-ttu-id="3e97d-164">无。</span><span class="sxs-lookup"><span data-stu-id="3e97d-164">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e97d-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e97d-165">JSON representation</span></span>

<span data-ttu-id="3e97d-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e97d-166">The following is a JSON representation of the resource.</span></span>
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
