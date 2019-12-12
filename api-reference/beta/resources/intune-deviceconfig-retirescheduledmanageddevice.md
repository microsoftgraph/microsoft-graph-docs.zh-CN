---
title: retireScheduledManagedDevice 资源类型
description: 计划停用的 ManagedDevices
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8b79f0541450f4d3c00e4f89f02405cd74545b49
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955516"
---
# <a name="retirescheduledmanageddevice-resource-type"></a><span data-ttu-id="9d480-103">retireScheduledManagedDevice 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d480-103">retireScheduledManagedDevice resource type</span></span>

> <span data-ttu-id="9d480-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9d480-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d480-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9d480-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d480-106">计划停用的 ManagedDevices</span><span class="sxs-lookup"><span data-stu-id="9d480-106">ManagedDevices that are scheduled for retire</span></span>

## <a name="properties"></a><span data-ttu-id="9d480-107">属性</span><span class="sxs-lookup"><span data-stu-id="9d480-107">Properties</span></span>
|<span data-ttu-id="9d480-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d480-108">Property</span></span>|<span data-ttu-id="9d480-109">类型</span><span class="sxs-lookup"><span data-stu-id="9d480-109">Type</span></span>|<span data-ttu-id="9d480-110">说明</span><span class="sxs-lookup"><span data-stu-id="9d480-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d480-111">id</span><span class="sxs-lookup"><span data-stu-id="9d480-111">id</span></span>|<span data-ttu-id="9d480-112">字符串</span><span class="sxs-lookup"><span data-stu-id="9d480-112">String</span></span>|<span data-ttu-id="9d480-113">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9d480-113">Key of the entity.</span></span>|
|<span data-ttu-id="9d480-114">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="9d480-114">managedDeviceId</span></span>|<span data-ttu-id="9d480-115">字符串</span><span class="sxs-lookup"><span data-stu-id="9d480-115">String</span></span>|<span data-ttu-id="9d480-116">托管 DeviceId</span><span class="sxs-lookup"><span data-stu-id="9d480-116">Managed DeviceId</span></span>|
|<span data-ttu-id="9d480-117">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="9d480-117">managedDeviceName</span></span>|<span data-ttu-id="9d480-118">String</span><span class="sxs-lookup"><span data-stu-id="9d480-118">String</span></span>|<span data-ttu-id="9d480-119">托管设备名称</span><span class="sxs-lookup"><span data-stu-id="9d480-119">Managed Device Name</span></span>|
|<span data-ttu-id="9d480-120">deviceType</span><span class="sxs-lookup"><span data-stu-id="9d480-120">deviceType</span></span>|[<span data-ttu-id="9d480-121">deviceType</span><span class="sxs-lookup"><span data-stu-id="9d480-121">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="9d480-122">托管设备设备类型。</span><span class="sxs-lookup"><span data-stu-id="9d480-122">Managed Device Device Type.</span></span> <span data-ttu-id="9d480-123">可能的值为`desktop`： `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `palm` `unknown`、、、、、、、、、、、、、、、、、、、。 `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry`</span><span class="sxs-lookup"><span data-stu-id="9d480-123">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="9d480-124">complianceState</span><span class="sxs-lookup"><span data-stu-id="9d480-124">complianceState</span></span>|[<span data-ttu-id="9d480-125">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="9d480-125">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="9d480-126">托管设备 ComplianceStatus。</span><span class="sxs-lookup"><span data-stu-id="9d480-126">Managed Device ComplianceStatus.</span></span> <span data-ttu-id="9d480-127">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="9d480-127">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="9d480-128">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="9d480-128">retireAfterDateTime</span></span>|<span data-ttu-id="9d480-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d480-129">DateTimeOffset</span></span>|<span data-ttu-id="9d480-130">托管设备在 DateTime 之后停用</span><span class="sxs-lookup"><span data-stu-id="9d480-130">Managed Device Retire After DateTime</span></span>|
|<span data-ttu-id="9d480-131">managementAgent</span><span class="sxs-lookup"><span data-stu-id="9d480-131">managementAgent</span></span>|[<span data-ttu-id="9d480-132">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="9d480-132">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="9d480-133">托管设备 ManagementAgentType。</span><span class="sxs-lookup"><span data-stu-id="9d480-133">Managed Device ManagementAgentType.</span></span> <span data-ttu-id="9d480-134">可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`。</span><span class="sxs-lookup"><span data-stu-id="9d480-134">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="9d480-135">所有者</span><span class="sxs-lookup"><span data-stu-id="9d480-135">ownerType</span></span>|[<span data-ttu-id="9d480-136">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="9d480-136">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="9d480-137">托管设备 ManagedDeviceOwnerType。</span><span class="sxs-lookup"><span data-stu-id="9d480-137">Managed Device ManagedDeviceOwnerType.</span></span> <span data-ttu-id="9d480-138">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="9d480-138">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="9d480-139">deviceCompliancePolicyName</span><span class="sxs-lookup"><span data-stu-id="9d480-139">deviceCompliancePolicyName</span></span>|<span data-ttu-id="9d480-140">字符串</span><span class="sxs-lookup"><span data-stu-id="9d480-140">String</span></span>|<span data-ttu-id="9d480-141">设备合规性策略名称</span><span class="sxs-lookup"><span data-stu-id="9d480-141">Device Compliance Policy Name</span></span>|
|<span data-ttu-id="9d480-142">deviceCompliancePolicyId</span><span class="sxs-lookup"><span data-stu-id="9d480-142">deviceCompliancePolicyId</span></span>|<span data-ttu-id="9d480-143">字符串</span><span class="sxs-lookup"><span data-stu-id="9d480-143">String</span></span>|<span data-ttu-id="9d480-144">设备合规性 PolicyId</span><span class="sxs-lookup"><span data-stu-id="9d480-144">Device Compliance PolicyId</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d480-145">关系</span><span class="sxs-lookup"><span data-stu-id="9d480-145">Relationships</span></span>
<span data-ttu-id="9d480-146">无</span><span class="sxs-lookup"><span data-stu-id="9d480-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d480-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d480-147">JSON Representation</span></span>
<span data-ttu-id="9d480-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d480-148">Here is a JSON representation of the resource.</span></span>
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
  "deviceCompliancePolicyId": "String"
}
```



