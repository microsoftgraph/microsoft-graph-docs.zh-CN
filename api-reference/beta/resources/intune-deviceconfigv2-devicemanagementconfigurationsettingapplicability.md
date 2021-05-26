---
title: deviceManagementConfigurationSettingApplicability 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b95e92c7ee9d6e520a326cb8918dcbfe05f83725
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665075"
---
# <a name="devicemanagementconfigurationsettingapplicability-resource-type"></a><span data-ttu-id="47d72-103">deviceManagementConfigurationSettingApplicability 资源类型</span><span class="sxs-lookup"><span data-stu-id="47d72-103">deviceManagementConfigurationSettingApplicability resource type</span></span>

<span data-ttu-id="47d72-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47d72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47d72-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="47d72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47d72-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="47d72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47d72-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="47d72-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="47d72-108">属性</span><span class="sxs-lookup"><span data-stu-id="47d72-108">Properties</span></span>
|<span data-ttu-id="47d72-109">属性</span><span class="sxs-lookup"><span data-stu-id="47d72-109">Property</span></span>|<span data-ttu-id="47d72-110">类型</span><span class="sxs-lookup"><span data-stu-id="47d72-110">Type</span></span>|<span data-ttu-id="47d72-111">说明</span><span class="sxs-lookup"><span data-stu-id="47d72-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47d72-112">说明</span><span class="sxs-lookup"><span data-stu-id="47d72-112">description</span></span>|<span data-ttu-id="47d72-113">String</span><span class="sxs-lookup"><span data-stu-id="47d72-113">String</span></span>|<span data-ttu-id="47d72-114">设置说明</span><span class="sxs-lookup"><span data-stu-id="47d72-114">description of the setting</span></span>|
|<span data-ttu-id="47d72-115">平台</span><span class="sxs-lookup"><span data-stu-id="47d72-115">platform</span></span>|[<span data-ttu-id="47d72-116">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="47d72-116">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="47d72-117">可以应用平台设置。</span><span class="sxs-lookup"><span data-stu-id="47d72-117">Platform setting can be applied on.</span></span> <span data-ttu-id="47d72-118">可取值为：`none`、`macOS`、`windows10X`、`windows10`。</span><span class="sxs-lookup"><span data-stu-id="47d72-118">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="47d72-119">deviceMode</span><span class="sxs-lookup"><span data-stu-id="47d72-119">deviceMode</span></span>|[<span data-ttu-id="47d72-120">deviceManagementConfigurationDeviceMode</span><span class="sxs-lookup"><span data-stu-id="47d72-120">deviceManagementConfigurationDeviceMode</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|<span data-ttu-id="47d72-121">可应用设置的设备模式。</span><span class="sxs-lookup"><span data-stu-id="47d72-121">Device Mode that setting can be applied on.</span></span> <span data-ttu-id="47d72-122">可取值为：`none`、`kiosk`。</span><span class="sxs-lookup"><span data-stu-id="47d72-122">Possible values are: `none`, `kiosk`.</span></span>|
|<span data-ttu-id="47d72-123">technologies</span><span class="sxs-lookup"><span data-stu-id="47d72-123">technologies</span></span>|[<span data-ttu-id="47d72-124">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="47d72-124">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="47d72-125">可通过哪些技术渠道部署此设置。</span><span class="sxs-lookup"><span data-stu-id="47d72-125">Which technology channels this setting can be deployed through.</span></span> <span data-ttu-id="47d72-126">可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`、`microsoftSense`。</span><span class="sxs-lookup"><span data-stu-id="47d72-126">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47d72-127">关系</span><span class="sxs-lookup"><span data-stu-id="47d72-127">Relationships</span></span>
<span data-ttu-id="47d72-128">无</span><span class="sxs-lookup"><span data-stu-id="47d72-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47d72-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47d72-129">JSON Representation</span></span>
<span data-ttu-id="47d72-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47d72-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingApplicability",
  "description": "String",
  "platform": "String",
  "deviceMode": "String",
  "technologies": "String"
}
```




