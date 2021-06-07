---
title: deviceManagement 资源类型
description: 充当所有设备管理功能的容器的单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ba60fc551a3f9de8b795b6521814d7899a1c3706
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755281"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="e3570-103">deviceManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="e3570-103">deviceManagement resource type</span></span>

<span data-ttu-id="e3570-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3570-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3570-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e3570-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3570-106">充当所有设备管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="e3570-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="e3570-107">方法</span><span class="sxs-lookup"><span data-stu-id="e3570-107">Methods</span></span>
|<span data-ttu-id="e3570-108">方法</span><span class="sxs-lookup"><span data-stu-id="e3570-108">Method</span></span>|<span data-ttu-id="e3570-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e3570-109">Return Type</span></span>|<span data-ttu-id="e3570-110">说明</span><span class="sxs-lookup"><span data-stu-id="e3570-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e3570-111">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e3570-111">Get deviceManagement</span></span>](../api/intune-deviceconfig-devicemanagement-get.md)|[<span data-ttu-id="e3570-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e3570-112">deviceManagement</span></span>](../resources/intune-deviceconfig-devicemanagement.md)|<span data-ttu-id="e3570-113">读取 [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e3570-113">Read properties and relationships of the [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="e3570-114">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e3570-114">Update deviceManagement</span></span>](../api/intune-deviceconfig-devicemanagement-update.md)|[<span data-ttu-id="e3570-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e3570-115">deviceManagement</span></span>](../resources/intune-deviceconfig-devicemanagement.md)|<span data-ttu-id="e3570-116">更新 [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e3570-116">Update the properties of a [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e3570-117">属性</span><span class="sxs-lookup"><span data-stu-id="e3570-117">Properties</span></span>
|<span data-ttu-id="e3570-118">属性</span><span class="sxs-lookup"><span data-stu-id="e3570-118">Property</span></span>|<span data-ttu-id="e3570-119">类型</span><span class="sxs-lookup"><span data-stu-id="e3570-119">Type</span></span>|<span data-ttu-id="e3570-120">说明</span><span class="sxs-lookup"><span data-stu-id="e3570-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3570-121">id</span><span class="sxs-lookup"><span data-stu-id="e3570-121">id</span></span>|<span data-ttu-id="e3570-122">String</span><span class="sxs-lookup"><span data-stu-id="e3570-122">String</span></span>|<span data-ttu-id="e3570-123">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="e3570-123">Unique Identifier</span></span>|
|<span data-ttu-id="e3570-124">settings</span><span class="sxs-lookup"><span data-stu-id="e3570-124">settings</span></span>|[<span data-ttu-id="e3570-125">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="e3570-125">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="e3570-126">帐户级别设置。</span><span class="sxs-lookup"><span data-stu-id="e3570-126">Account level settings.</span></span>|
|<span data-ttu-id="e3570-127">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="e3570-127">intuneAccountId</span></span>|<span data-ttu-id="e3570-128">Guid</span><span class="sxs-lookup"><span data-stu-id="e3570-128">Guid</span></span>|<span data-ttu-id="e3570-129">给定租户的 Intune 帐户 ID</span><span class="sxs-lookup"><span data-stu-id="e3570-129">Intune Account Id for given tenant</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3570-130">关系</span><span class="sxs-lookup"><span data-stu-id="e3570-130">Relationships</span></span>
|<span data-ttu-id="e3570-131">关系</span><span class="sxs-lookup"><span data-stu-id="e3570-131">Relationship</span></span>|<span data-ttu-id="e3570-132">类型</span><span class="sxs-lookup"><span data-stu-id="e3570-132">Type</span></span>|<span data-ttu-id="e3570-133">说明</span><span class="sxs-lookup"><span data-stu-id="e3570-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3570-134">deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="e3570-134">deviceConfigurations</span></span>|<span data-ttu-id="e3570-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e3570-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="e3570-136">设备配置。</span><span class="sxs-lookup"><span data-stu-id="e3570-136">The device configurations.</span></span>|
|<span data-ttu-id="e3570-137">deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="e3570-137">deviceCompliancePolicies</span></span>|<span data-ttu-id="e3570-138">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e3570-138">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="e3570-139">设备符合性策略。</span><span class="sxs-lookup"><span data-stu-id="e3570-139">The device compliance policies.</span></span>|
|<span data-ttu-id="e3570-140">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="e3570-140">softwareUpdateStatusSummary</span></span>|[<span data-ttu-id="e3570-141">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="e3570-141">softwareUpdateStatusSummary</span></span>](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|<span data-ttu-id="e3570-142">软件更新状态摘要。</span><span class="sxs-lookup"><span data-stu-id="e3570-142">The software update status summary.</span></span>|
|<span data-ttu-id="e3570-143">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e3570-143">deviceCompliancePolicyDeviceStateSummary</span></span>|[<span data-ttu-id="e3570-144">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e3570-144">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="e3570-145">此帐户的设备符合性状态摘要。</span><span class="sxs-lookup"><span data-stu-id="e3570-145">The device compliance state summary for this account.</span></span>|
|<span data-ttu-id="e3570-146">deviceCompliancePolicySettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="e3570-146">deviceCompliancePolicySettingStateSummaries</span></span>|<span data-ttu-id="e3570-147">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e3570-147">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) collection</span></span>|<span data-ttu-id="e3570-148">此帐户的符合性设置的摘要状态。</span><span class="sxs-lookup"><span data-stu-id="e3570-148">The summary states of compliance policy settings for this account.</span></span>|
|<span data-ttu-id="e3570-149">deviceConfigurationDeviceStateSummaries</span><span class="sxs-lookup"><span data-stu-id="e3570-149">deviceConfigurationDeviceStateSummaries</span></span>|[<span data-ttu-id="e3570-150">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e3570-150">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="e3570-151">此帐户的设备配置设备状态摘要。</span><span class="sxs-lookup"><span data-stu-id="e3570-151">The device configuration device state summary for this account.</span></span>|
|<span data-ttu-id="e3570-152">iosUpdateStatuses</span><span class="sxs-lookup"><span data-stu-id="e3570-152">iosUpdateStatuses</span></span>|<span data-ttu-id="e3570-153">[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e3570-153">[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) collection</span></span>|<span data-ttu-id="e3570-154">此帐户的 IOS 软件更新安装状态。</span><span class="sxs-lookup"><span data-stu-id="e3570-154">The IOS software update installation statuses for this account.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3570-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3570-155">JSON Representation</span></span>
<span data-ttu-id="e3570-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3570-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 1024,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  },
  "intuneAccountId": "Guid"
}
```




