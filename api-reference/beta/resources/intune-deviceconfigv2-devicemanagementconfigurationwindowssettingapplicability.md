---
title: deviceManagementConfigurationWindowsSettingApplicability 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ca3b520a194a09d178790f5a82f3ca21c1e00d2d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301509"
---
# <a name="devicemanagementconfigurationwindowssettingapplicability-resource-type"></a><span data-ttu-id="8c862-103">deviceManagementConfigurationWindowsSettingApplicability 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c862-103">deviceManagementConfigurationWindowsSettingApplicability resource type</span></span>

<span data-ttu-id="8c862-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c862-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c862-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c862-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c862-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c862-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c862-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c862-107">Not yet documented</span></span>


<span data-ttu-id="8c862-108">继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span><span class="sxs-lookup"><span data-stu-id="8c862-108">Inherits from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8c862-109">属性</span><span class="sxs-lookup"><span data-stu-id="8c862-109">Properties</span></span>
|<span data-ttu-id="8c862-110">属性</span><span class="sxs-lookup"><span data-stu-id="8c862-110">Property</span></span>|<span data-ttu-id="8c862-111">类型</span><span class="sxs-lookup"><span data-stu-id="8c862-111">Type</span></span>|<span data-ttu-id="8c862-112">说明</span><span class="sxs-lookup"><span data-stu-id="8c862-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c862-113">说明</span><span class="sxs-lookup"><span data-stu-id="8c862-113">description</span></span>|<span data-ttu-id="8c862-114">String</span><span class="sxs-lookup"><span data-stu-id="8c862-114">String</span></span>|<span data-ttu-id="8c862-115">从[DeviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)继承的设置的说明</span><span class="sxs-lookup"><span data-stu-id="8c862-115">description of the setting Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span></span>|
|<span data-ttu-id="8c862-116">平台</span><span class="sxs-lookup"><span data-stu-id="8c862-116">platform</span></span>|[<span data-ttu-id="8c862-117">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="8c862-117">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="8c862-118">平台设置可应用于继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)。</span><span class="sxs-lookup"><span data-stu-id="8c862-118">Platform setting can be applied on Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span></span> <span data-ttu-id="8c862-119">可取值为：`none`、`macOS`、`windows10X`、`windows10`。</span><span class="sxs-lookup"><span data-stu-id="8c862-119">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="8c862-120">deviceMode</span><span class="sxs-lookup"><span data-stu-id="8c862-120">deviceMode</span></span>|[<span data-ttu-id="8c862-121">deviceManagementConfigurationDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8c862-121">deviceManagementConfigurationDeviceMode</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|<span data-ttu-id="8c862-122">可在继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)时应用设置的设备模式。</span><span class="sxs-lookup"><span data-stu-id="8c862-122">Device Mode that setting can be applied on Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span></span> <span data-ttu-id="8c862-123">可取值为：`none`、`kiosk`。</span><span class="sxs-lookup"><span data-stu-id="8c862-123">Possible values are: `none`, `kiosk`.</span></span>|
|<span data-ttu-id="8c862-124">技术</span><span class="sxs-lookup"><span data-stu-id="8c862-124">technologies</span></span>|[<span data-ttu-id="8c862-125">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="8c862-125">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="8c862-126">可以通过从 [DeviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)继承来部署此设置的技术通道。</span><span class="sxs-lookup"><span data-stu-id="8c862-126">Which technology channels this setting can be deployed through Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span></span> <span data-ttu-id="8c862-127">可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="8c862-127">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|
|<span data-ttu-id="8c862-128">configurationServiceProviderVersion</span><span class="sxs-lookup"><span data-stu-id="8c862-128">configurationServiceProviderVersion</span></span>|<span data-ttu-id="8c862-129">String</span><span class="sxs-lookup"><span data-stu-id="8c862-129">String</span></span>|<span data-ttu-id="8c862-130">CSP 的版本设置属于</span><span class="sxs-lookup"><span data-stu-id="8c862-130">Version of CSP setting is a part of</span></span>|
|<span data-ttu-id="8c862-131">maximumSupportedVersion</span><span class="sxs-lookup"><span data-stu-id="8c862-131">maximumSupportedVersion</span></span>|<span data-ttu-id="8c862-132">String</span><span class="sxs-lookup"><span data-stu-id="8c862-132">String</span></span>|<span data-ttu-id="8c862-133">最大支持的 Windows 版本</span><span class="sxs-lookup"><span data-stu-id="8c862-133">Maximum supported version of Windows</span></span>|
|<span data-ttu-id="8c862-134">minimumSupportedVersion</span><span class="sxs-lookup"><span data-stu-id="8c862-134">minimumSupportedVersion</span></span>|<span data-ttu-id="8c862-135">String</span><span class="sxs-lookup"><span data-stu-id="8c862-135">String</span></span>|<span data-ttu-id="8c862-136">支持的最低版本的 Windows</span><span class="sxs-lookup"><span data-stu-id="8c862-136">Minimum supported version of Windows</span></span>|
|<span data-ttu-id="8c862-137">windowsSkus</span><span class="sxs-lookup"><span data-stu-id="8c862-137">windowsSkus</span></span>|<span data-ttu-id="8c862-138">[deviceManagementConfigurationWindowsSkus](../resources/intune-deviceconfigv2-devicemanagementconfigurationwindowsskus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8c862-138">[deviceManagementConfigurationWindowsSkus](../resources/intune-deviceconfigv2-devicemanagementconfigurationwindowsskus.md) collection</span></span>|<span data-ttu-id="8c862-139">该设置适用于的 Windows Sku 列表</span><span class="sxs-lookup"><span data-stu-id="8c862-139">List of Windows SKUs that the setting is applicable for</span></span>|
|<span data-ttu-id="8c862-140">requiresAzureAd</span><span class="sxs-lookup"><span data-stu-id="8c862-140">requiresAzureAd</span></span>|<span data-ttu-id="8c862-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c862-141">Boolean</span></span>|<span data-ttu-id="8c862-142">AzureAD 设置要求</span><span class="sxs-lookup"><span data-stu-id="8c862-142">AzureAD setting requirement</span></span>|
|<span data-ttu-id="8c862-143">requiredAzureAdTrustType</span><span class="sxs-lookup"><span data-stu-id="8c862-143">requiredAzureAdTrustType</span></span>|[<span data-ttu-id="8c862-144">deviceManagementConfigurationAzureAdTrustType</span><span class="sxs-lookup"><span data-stu-id="8c862-144">deviceManagementConfigurationAzureAdTrustType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationazureadtrusttype.md)|<span data-ttu-id="8c862-145">必需的 AzureAD 信任类型。</span><span class="sxs-lookup"><span data-stu-id="8c862-145">Required AzureAD trust type.</span></span> <span data-ttu-id="8c862-146">可取值为：`none`、`azureAdJoined`、`addWorkAccount`、`mdmOnly`。</span><span class="sxs-lookup"><span data-stu-id="8c862-146">Possible values are: `none`, `azureAdJoined`, `addWorkAccount`, `mdmOnly`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c862-147">关系</span><span class="sxs-lookup"><span data-stu-id="8c862-147">Relationships</span></span>
<span data-ttu-id="8c862-148">无</span><span class="sxs-lookup"><span data-stu-id="8c862-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c862-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c862-149">JSON Representation</span></span>
<span data-ttu-id="8c862-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c862-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationWindowsSettingApplicability"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationWindowsSettingApplicability",
  "description": "String",
  "platform": "String",
  "deviceMode": "String",
  "technologies": "String",
  "configurationServiceProviderVersion": "String",
  "maximumSupportedVersion": "String",
  "minimumSupportedVersion": "String",
  "windowsSkus": [
    "String"
  ],
  "requiresAzureAd": true,
  "requiredAzureAdTrustType": "String"
}
```




