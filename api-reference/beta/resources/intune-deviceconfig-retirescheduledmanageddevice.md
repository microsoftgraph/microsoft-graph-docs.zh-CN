---
title: retireScheduledManagedDevice 资源类型
description: 计划停用的 ManagedDevices
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2939da221a47e878414c5a24f2ed44fdd9c5e238
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729662"
---
# <a name="retirescheduledmanageddevice-resource-type"></a><span data-ttu-id="2360a-103">retireScheduledManagedDevice 资源类型</span><span class="sxs-lookup"><span data-stu-id="2360a-103">retireScheduledManagedDevice resource type</span></span>

<span data-ttu-id="2360a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2360a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2360a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2360a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2360a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2360a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2360a-107">计划停用的 ManagedDevices</span><span class="sxs-lookup"><span data-stu-id="2360a-107">ManagedDevices that are scheduled for retire</span></span>

## <a name="properties"></a><span data-ttu-id="2360a-108">属性</span><span class="sxs-lookup"><span data-stu-id="2360a-108">Properties</span></span>
|<span data-ttu-id="2360a-109">属性</span><span class="sxs-lookup"><span data-stu-id="2360a-109">Property</span></span>|<span data-ttu-id="2360a-110">类型</span><span class="sxs-lookup"><span data-stu-id="2360a-110">Type</span></span>|<span data-ttu-id="2360a-111">说明</span><span class="sxs-lookup"><span data-stu-id="2360a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2360a-112">id</span><span class="sxs-lookup"><span data-stu-id="2360a-112">id</span></span>|<span data-ttu-id="2360a-113">String</span><span class="sxs-lookup"><span data-stu-id="2360a-113">String</span></span>|<span data-ttu-id="2360a-114">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2360a-114">Key of the entity.</span></span>|
|<span data-ttu-id="2360a-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="2360a-115">managedDeviceId</span></span>|<span data-ttu-id="2360a-116">String</span><span class="sxs-lookup"><span data-stu-id="2360a-116">String</span></span>|<span data-ttu-id="2360a-117">托管 DeviceId</span><span class="sxs-lookup"><span data-stu-id="2360a-117">Managed DeviceId</span></span>|
|<span data-ttu-id="2360a-118">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="2360a-118">managedDeviceName</span></span>|<span data-ttu-id="2360a-119">String</span><span class="sxs-lookup"><span data-stu-id="2360a-119">String</span></span>|<span data-ttu-id="2360a-120">托管设备名称</span><span class="sxs-lookup"><span data-stu-id="2360a-120">Managed Device Name</span></span>|
|<span data-ttu-id="2360a-121">deviceType</span><span class="sxs-lookup"><span data-stu-id="2360a-121">deviceType</span></span>|[<span data-ttu-id="2360a-122">deviceType</span><span class="sxs-lookup"><span data-stu-id="2360a-122">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="2360a-123">托管设备设备类型。</span><span class="sxs-lookup"><span data-stu-id="2360a-123">Managed Device Device Type.</span></span> <span data-ttu-id="2360a-124">可能的值为：、、、、、、、、、、、、、、、、、、、、、、、 `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `blackberry` `palm` `unknown` 。</span><span class="sxs-lookup"><span data-stu-id="2360a-124">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="2360a-125">complianceState</span><span class="sxs-lookup"><span data-stu-id="2360a-125">complianceState</span></span>|[<span data-ttu-id="2360a-126">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2360a-126">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2360a-127">托管设备 ComplianceStatus。</span><span class="sxs-lookup"><span data-stu-id="2360a-127">Managed Device ComplianceStatus.</span></span> <span data-ttu-id="2360a-128">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="2360a-128">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2360a-129">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="2360a-129">retireAfterDateTime</span></span>|<span data-ttu-id="2360a-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2360a-130">DateTimeOffset</span></span>|<span data-ttu-id="2360a-131">托管设备在 DateTime 之后停用</span><span class="sxs-lookup"><span data-stu-id="2360a-131">Managed Device Retire After DateTime</span></span>|
|<span data-ttu-id="2360a-132">managementAgent</span><span class="sxs-lookup"><span data-stu-id="2360a-132">managementAgent</span></span>|[<span data-ttu-id="2360a-133">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="2360a-133">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="2360a-134">托管设备 ManagementAgentType。</span><span class="sxs-lookup"><span data-stu-id="2360a-134">Managed Device ManagementAgentType.</span></span> <span data-ttu-id="2360a-135">可能的值是：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`、`windowsManagementCloudApi`。</span><span class="sxs-lookup"><span data-stu-id="2360a-135">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="2360a-136">所有者</span><span class="sxs-lookup"><span data-stu-id="2360a-136">ownerType</span></span>|[<span data-ttu-id="2360a-137">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="2360a-137">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="2360a-138">托管设备 ManagedDeviceOwnerType。</span><span class="sxs-lookup"><span data-stu-id="2360a-138">Managed Device ManagedDeviceOwnerType.</span></span> <span data-ttu-id="2360a-139">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="2360a-139">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="2360a-140">deviceCompliancePolicyName</span><span class="sxs-lookup"><span data-stu-id="2360a-140">deviceCompliancePolicyName</span></span>|<span data-ttu-id="2360a-141">String</span><span class="sxs-lookup"><span data-stu-id="2360a-141">String</span></span>|<span data-ttu-id="2360a-142">设备合规性策略名称</span><span class="sxs-lookup"><span data-stu-id="2360a-142">Device Compliance Policy Name</span></span>|
|<span data-ttu-id="2360a-143">deviceCompliancePolicyId</span><span class="sxs-lookup"><span data-stu-id="2360a-143">deviceCompliancePolicyId</span></span>|<span data-ttu-id="2360a-144">String</span><span class="sxs-lookup"><span data-stu-id="2360a-144">String</span></span>|<span data-ttu-id="2360a-145">设备合规性 PolicyId</span><span class="sxs-lookup"><span data-stu-id="2360a-145">Device Compliance PolicyId</span></span>|
|<span data-ttu-id="2360a-146">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2360a-146">roleScopeTagIds</span></span>|<span data-ttu-id="2360a-147">String collection</span><span class="sxs-lookup"><span data-stu-id="2360a-147">String collection</span></span>|<span data-ttu-id="2360a-148">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2360a-148">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2360a-149">关系</span><span class="sxs-lookup"><span data-stu-id="2360a-149">Relationships</span></span>
<span data-ttu-id="2360a-150">无</span><span class="sxs-lookup"><span data-stu-id="2360a-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2360a-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2360a-151">JSON Representation</span></span>
<span data-ttu-id="2360a-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2360a-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.retireScheduledManagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.retireScheduledManagedDevice",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "deviceType": "String",
  "complianceState": "String",
  "retireAfterDateTime": "String (timestamp)",
  "managementAgent": "String",
  "ownerType": "String",
  "deviceCompliancePolicyName": "String",
  "deviceCompliancePolicyId": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```





