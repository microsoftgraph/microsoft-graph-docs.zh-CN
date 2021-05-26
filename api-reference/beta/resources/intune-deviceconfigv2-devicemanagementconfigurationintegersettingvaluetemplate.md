---
title: deviceManagementConfigurationIntegerSettingValueTemplate 资源类型
description: 整数设置值模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1a196cf31bbb1a7063b6d937e797d602e7481ff4
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666842"
---
# <a name="devicemanagementconfigurationintegersettingvaluetemplate-resource-type"></a><span data-ttu-id="33573-103">deviceManagementConfigurationIntegerSettingValueTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="33573-103">deviceManagementConfigurationIntegerSettingValueTemplate resource type</span></span>

<span data-ttu-id="33573-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33573-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33573-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="33573-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33573-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="33573-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33573-107">整数设置值模板</span><span class="sxs-lookup"><span data-stu-id="33573-107">Integer Setting Value Template</span></span>


<span data-ttu-id="33573-108">继承自 [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="33573-108">Inherits from [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="33573-109">属性</span><span class="sxs-lookup"><span data-stu-id="33573-109">Properties</span></span>
|<span data-ttu-id="33573-110">属性</span><span class="sxs-lookup"><span data-stu-id="33573-110">Property</span></span>|<span data-ttu-id="33573-111">类型</span><span class="sxs-lookup"><span data-stu-id="33573-111">Type</span></span>|<span data-ttu-id="33573-112">说明</span><span class="sxs-lookup"><span data-stu-id="33573-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33573-113">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="33573-113">settingValueTemplateId</span></span>|<span data-ttu-id="33573-114">String</span><span class="sxs-lookup"><span data-stu-id="33573-114">String</span></span>|<span data-ttu-id="33573-115">设置值模板 ID 继承自 [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="33573-115">Setting Value Template Id Inherited from [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span></span>|
|<span data-ttu-id="33573-116">defaultValue</span><span class="sxs-lookup"><span data-stu-id="33573-116">defaultValue</span></span>|[<span data-ttu-id="33573-117">deviceManagementConfigurationIntegerSettingValueDefaultTemplate</span><span class="sxs-lookup"><span data-stu-id="33573-117">deviceManagementConfigurationIntegerSettingValueDefaultTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefaulttemplate.md)|<span data-ttu-id="33573-118">整数设置值默认模板。</span><span class="sxs-lookup"><span data-stu-id="33573-118">Integer Setting Value Default Template.</span></span>|
|<span data-ttu-id="33573-119">recommendedValueDefinition</span><span class="sxs-lookup"><span data-stu-id="33573-119">recommendedValueDefinition</span></span>|[<span data-ttu-id="33573-120">deviceManagementConfigurationIntegerSettingValueDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="33573-120">deviceManagementConfigurationIntegerSettingValueDefinitionTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefinitiontemplate.md)|<span data-ttu-id="33573-121">建议的值定义。</span><span class="sxs-lookup"><span data-stu-id="33573-121">Recommended value definition.</span></span>|
|<span data-ttu-id="33573-122">requiredValueDefinition</span><span class="sxs-lookup"><span data-stu-id="33573-122">requiredValueDefinition</span></span>|[<span data-ttu-id="33573-123">deviceManagementConfigurationIntegerSettingValueDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="33573-123">deviceManagementConfigurationIntegerSettingValueDefinitionTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefinitiontemplate.md)|<span data-ttu-id="33573-124">必需的值定义。</span><span class="sxs-lookup"><span data-stu-id="33573-124">Required value definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33573-125">关系</span><span class="sxs-lookup"><span data-stu-id="33573-125">Relationships</span></span>
<span data-ttu-id="33573-126">无</span><span class="sxs-lookup"><span data-stu-id="33573-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="33573-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33573-127">JSON Representation</span></span>
<span data-ttu-id="33573-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33573-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValueTemplate",
  "settingValueTemplateId": "String",
  "defaultValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate",
    "constantValue": 1024
  },
  "recommendedValueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate",
    "minValue": 1024,
    "maxValue": 1024
  },
  "requiredValueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate",
    "minValue": 1024,
    "maxValue": 1024
  }
}
```




