---
title: deviceManagementConfigurationSettingApplicability 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f94bfffd8dd3149d11e7ada38a4c238f4ce618a4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241272"
---
# <a name="devicemanagementconfigurationsettingapplicability-resource-type"></a><span data-ttu-id="81e51-103">deviceManagementConfigurationSettingApplicability 资源类型</span><span class="sxs-lookup"><span data-stu-id="81e51-103">deviceManagementConfigurationSettingApplicability resource type</span></span>

<span data-ttu-id="81e51-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81e51-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81e51-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="81e51-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81e51-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81e51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81e51-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="81e51-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="81e51-108">属性</span><span class="sxs-lookup"><span data-stu-id="81e51-108">Properties</span></span>
|<span data-ttu-id="81e51-109">属性</span><span class="sxs-lookup"><span data-stu-id="81e51-109">Property</span></span>|<span data-ttu-id="81e51-110">类型</span><span class="sxs-lookup"><span data-stu-id="81e51-110">Type</span></span>|<span data-ttu-id="81e51-111">说明</span><span class="sxs-lookup"><span data-stu-id="81e51-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81e51-112">说明</span><span class="sxs-lookup"><span data-stu-id="81e51-112">description</span></span>|<span data-ttu-id="81e51-113">String</span><span class="sxs-lookup"><span data-stu-id="81e51-113">String</span></span>|<span data-ttu-id="81e51-114">设置的说明</span><span class="sxs-lookup"><span data-stu-id="81e51-114">description of the setting</span></span>|
|<span data-ttu-id="81e51-115">平台</span><span class="sxs-lookup"><span data-stu-id="81e51-115">platform</span></span>|[<span data-ttu-id="81e51-116">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="81e51-116">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="81e51-117">可以在上应用平台设置。</span><span class="sxs-lookup"><span data-stu-id="81e51-117">Platform setting can be applied on.</span></span> <span data-ttu-id="81e51-118">可取值为：`none`、`macOS`、`windows10X`、`windows10`。</span><span class="sxs-lookup"><span data-stu-id="81e51-118">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="81e51-119">deviceMode</span><span class="sxs-lookup"><span data-stu-id="81e51-119">deviceMode</span></span>|[<span data-ttu-id="81e51-120">deviceManagementConfigurationDeviceMode</span><span class="sxs-lookup"><span data-stu-id="81e51-120">deviceManagementConfigurationDeviceMode</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|<span data-ttu-id="81e51-121">可在上应用设置的设备模式。</span><span class="sxs-lookup"><span data-stu-id="81e51-121">Device Mode that setting can be applied on.</span></span> <span data-ttu-id="81e51-122">可取值为：`none`、`kiosk`。</span><span class="sxs-lookup"><span data-stu-id="81e51-122">Possible values are: `none`, `kiosk`.</span></span>|
|<span data-ttu-id="81e51-123">技术</span><span class="sxs-lookup"><span data-stu-id="81e51-123">technologies</span></span>|[<span data-ttu-id="81e51-124">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="81e51-124">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="81e51-125">可以通过哪些技术通道来部署此设置。</span><span class="sxs-lookup"><span data-stu-id="81e51-125">Which technology channels this setting can be deployed through.</span></span> <span data-ttu-id="81e51-126">可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="81e51-126">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81e51-127">关系</span><span class="sxs-lookup"><span data-stu-id="81e51-127">Relationships</span></span>
<span data-ttu-id="81e51-128">无</span><span class="sxs-lookup"><span data-stu-id="81e51-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81e51-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81e51-129">JSON Representation</span></span>
<span data-ttu-id="81e51-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81e51-130">Here is a JSON representation of the resource.</span></span>
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




