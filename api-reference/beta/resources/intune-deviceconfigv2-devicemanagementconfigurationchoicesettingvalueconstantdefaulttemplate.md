---
title: deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate 资源类型
description: 选项设置值常量默认模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f55e885448e7fe131a1eb4151196d5a200a8d300
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666588"
---
# <a name="devicemanagementconfigurationchoicesettingvalueconstantdefaulttemplate-resource-type"></a><span data-ttu-id="2899b-103">deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="2899b-103">deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate resource type</span></span>

<span data-ttu-id="2899b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2899b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2899b-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2899b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2899b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2899b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2899b-107">选项设置值常量默认模板</span><span class="sxs-lookup"><span data-stu-id="2899b-107">Choice Setting Value Constant Default Template</span></span>


<span data-ttu-id="2899b-108">继承自 [deviceManagementConfigurationChoiceSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefaulttemplate.md)</span><span class="sxs-lookup"><span data-stu-id="2899b-108">Inherits from [deviceManagementConfigurationChoiceSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefaulttemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2899b-109">属性</span><span class="sxs-lookup"><span data-stu-id="2899b-109">Properties</span></span>
|<span data-ttu-id="2899b-110">属性</span><span class="sxs-lookup"><span data-stu-id="2899b-110">Property</span></span>|<span data-ttu-id="2899b-111">类型</span><span class="sxs-lookup"><span data-stu-id="2899b-111">Type</span></span>|<span data-ttu-id="2899b-112">说明</span><span class="sxs-lookup"><span data-stu-id="2899b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2899b-113">settingDefinitionOptionId</span><span class="sxs-lookup"><span data-stu-id="2899b-113">settingDefinitionOptionId</span></span>|<span data-ttu-id="2899b-114">String</span><span class="sxs-lookup"><span data-stu-id="2899b-114">String</span></span>|<span data-ttu-id="2899b-115">默认常量值</span><span class="sxs-lookup"><span data-stu-id="2899b-115">Default Constant Value</span></span>|
|<span data-ttu-id="2899b-116">children</span><span class="sxs-lookup"><span data-stu-id="2899b-116">children</span></span>|<span data-ttu-id="2899b-117">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2899b-117">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) collection</span></span>|<span data-ttu-id="2899b-118">选项子项</span><span class="sxs-lookup"><span data-stu-id="2899b-118">Option Children</span></span>|

## <a name="relationships"></a><span data-ttu-id="2899b-119">关系</span><span class="sxs-lookup"><span data-stu-id="2899b-119">Relationships</span></span>
<span data-ttu-id="2899b-120">无</span><span class="sxs-lookup"><span data-stu-id="2899b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2899b-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2899b-121">JSON Representation</span></span>
<span data-ttu-id="2899b-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2899b-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate",
  "settingDefinitionOptionId": "String",
  "children": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
      "settingInstanceTemplateId": "String",
      "settingDefinitionId": "String",
      "isRequired": true,
      "simpleSettingValueTemplate": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
        "settingValueTemplateId": "String",
        "defaultValue": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
          "constantValue": "String"
        }
      }
    }
  ]
}
```




