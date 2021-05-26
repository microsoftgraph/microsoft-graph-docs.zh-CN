---
title: deviceManagementConfigurationWindowsSettingApplicability 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2302bcbae4af684efc159f269d639c50aeb99191
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666679"
---
# <a name="devicemanagementconfigurationwindowssettingapplicability-resource-type"></a><span data-ttu-id="48b7d-103">deviceManagementConfigurationWindowsSettingApplicability 资源类型</span><span class="sxs-lookup"><span data-stu-id="48b7d-103">deviceManagementConfigurationWindowsSettingApplicability resource type</span></span>

<span data-ttu-id="48b7d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48b7d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48b7d-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="48b7d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48b7d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="48b7d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48b7d-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="48b7d-107">Not yet documented</span></span>


<span data-ttu-id="48b7d-108">继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span><span class="sxs-lookup"><span data-stu-id="48b7d-108">Inherits from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span></span>

## <a name="properties"></a><span data-ttu-id="48b7d-109">属性</span><span class="sxs-lookup"><span data-stu-id="48b7d-109">Properties</span></span>
|<span data-ttu-id="48b7d-110">属性</span><span class="sxs-lookup"><span data-stu-id="48b7d-110">Property</span></span>|<span data-ttu-id="48b7d-111">类型</span><span class="sxs-lookup"><span data-stu-id="48b7d-111">Type</span></span>|<span data-ttu-id="48b7d-112">说明</span><span class="sxs-lookup"><span data-stu-id="48b7d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48b7d-113">说明</span><span class="sxs-lookup"><span data-stu-id="48b7d-113">description</span></span>|<span data-ttu-id="48b7d-114">String</span><span class="sxs-lookup"><span data-stu-id="48b7d-114">String</span></span>|<span data-ttu-id="48b7d-115">设置说明 继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span><span class="sxs-lookup"><span data-stu-id="48b7d-115">description of the setting Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span></span>|
|<span data-ttu-id="48b7d-116">平台</span><span class="sxs-lookup"><span data-stu-id="48b7d-116">platform</span></span>|[<span data-ttu-id="48b7d-117">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="48b7d-117">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="48b7d-118">可以在继承自 [deviceManagementConfigurationSettingApplicability 上应用平台设置](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)。</span><span class="sxs-lookup"><span data-stu-id="48b7d-118">Platform setting can be applied on Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span></span> <span data-ttu-id="48b7d-119">可取值为：`none`、`macOS`、`windows10X`、`windows10`。</span><span class="sxs-lookup"><span data-stu-id="48b7d-119">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="48b7d-120">deviceMode</span><span class="sxs-lookup"><span data-stu-id="48b7d-120">deviceMode</span></span>|[<span data-ttu-id="48b7d-121">deviceManagementConfigurationDeviceMode</span><span class="sxs-lookup"><span data-stu-id="48b7d-121">deviceManagementConfigurationDeviceMode</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|<span data-ttu-id="48b7d-122">可以在继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)上应用设置的设备模式。</span><span class="sxs-lookup"><span data-stu-id="48b7d-122">Device Mode that setting can be applied on Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span></span> <span data-ttu-id="48b7d-123">可取值为：`none`、`kiosk`。</span><span class="sxs-lookup"><span data-stu-id="48b7d-123">Possible values are: `none`, `kiosk`.</span></span>|
|<span data-ttu-id="48b7d-124">technologies</span><span class="sxs-lookup"><span data-stu-id="48b7d-124">technologies</span></span>|[<span data-ttu-id="48b7d-125">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="48b7d-125">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="48b7d-126">可通过继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)部署此设置的技术通道。</span><span class="sxs-lookup"><span data-stu-id="48b7d-126">Which technology channels this setting can be deployed through Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span></span> <span data-ttu-id="48b7d-127">可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`、`microsoftSense`。</span><span class="sxs-lookup"><span data-stu-id="48b7d-127">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span></span>|
|<span data-ttu-id="48b7d-128">configurationServiceProviderVersion</span><span class="sxs-lookup"><span data-stu-id="48b7d-128">configurationServiceProviderVersion</span></span>|<span data-ttu-id="48b7d-129">String</span><span class="sxs-lookup"><span data-stu-id="48b7d-129">String</span></span>|<span data-ttu-id="48b7d-130">云解决方案提供商设置的版本是其中一部分</span><span class="sxs-lookup"><span data-stu-id="48b7d-130">Version of CSP setting is a part of</span></span>|
|<span data-ttu-id="48b7d-131">maximumSupportedVersion</span><span class="sxs-lookup"><span data-stu-id="48b7d-131">maximumSupportedVersion</span></span>|<span data-ttu-id="48b7d-132">String</span><span class="sxs-lookup"><span data-stu-id="48b7d-132">String</span></span>|<span data-ttu-id="48b7d-133">支持的最大版本Windows</span><span class="sxs-lookup"><span data-stu-id="48b7d-133">Maximum supported version of Windows</span></span>|
|<span data-ttu-id="48b7d-134">minimumSupportedVersion</span><span class="sxs-lookup"><span data-stu-id="48b7d-134">minimumSupportedVersion</span></span>|<span data-ttu-id="48b7d-135">String</span><span class="sxs-lookup"><span data-stu-id="48b7d-135">String</span></span>|<span data-ttu-id="48b7d-136">支持的最低版本Windows</span><span class="sxs-lookup"><span data-stu-id="48b7d-136">Minimum supported version of Windows</span></span>|
|<span data-ttu-id="48b7d-137">windowsSkus</span><span class="sxs-lookup"><span data-stu-id="48b7d-137">windowsSkus</span></span>|<span data-ttu-id="48b7d-138">[deviceManagementConfigurationWindowsSkus](../resources/intune-deviceconfigv2-devicemanagementconfigurationwindowsskus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="48b7d-138">[deviceManagementConfigurationWindowsSkus](../resources/intune-deviceconfigv2-devicemanagementconfigurationwindowsskus.md) collection</span></span>|<span data-ttu-id="48b7d-139">设置Windows的 SKUS 列表</span><span class="sxs-lookup"><span data-stu-id="48b7d-139">List of Windows SKUs that the setting is applicable for</span></span>|
|<span data-ttu-id="48b7d-140">requiresAzureAd</span><span class="sxs-lookup"><span data-stu-id="48b7d-140">requiresAzureAd</span></span>|<span data-ttu-id="48b7d-141">布尔值</span><span class="sxs-lookup"><span data-stu-id="48b7d-141">Boolean</span></span>|<span data-ttu-id="48b7d-142">AzureAD 设置要求</span><span class="sxs-lookup"><span data-stu-id="48b7d-142">AzureAD setting requirement</span></span>|
|<span data-ttu-id="48b7d-143">requiredAzureAdTrustType</span><span class="sxs-lookup"><span data-stu-id="48b7d-143">requiredAzureAdTrustType</span></span>|[<span data-ttu-id="48b7d-144">deviceManagementConfigurationAzureAdTrustType</span><span class="sxs-lookup"><span data-stu-id="48b7d-144">deviceManagementConfigurationAzureAdTrustType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationazureadtrusttype.md)|<span data-ttu-id="48b7d-145">必需属性，类型为 AzureAD 信任。</span><span class="sxs-lookup"><span data-stu-id="48b7d-145">Required AzureAD trust type.</span></span> <span data-ttu-id="48b7d-146">可取值为：`none`、`azureAdJoined`、`addWorkAccount`、`mdmOnly`。</span><span class="sxs-lookup"><span data-stu-id="48b7d-146">Possible values are: `none`, `azureAdJoined`, `addWorkAccount`, `mdmOnly`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48b7d-147">关系</span><span class="sxs-lookup"><span data-stu-id="48b7d-147">Relationships</span></span>
<span data-ttu-id="48b7d-148">无</span><span class="sxs-lookup"><span data-stu-id="48b7d-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48b7d-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48b7d-149">JSON Representation</span></span>
<span data-ttu-id="48b7d-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48b7d-150">Here is a JSON representation of the resource.</span></span>
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




