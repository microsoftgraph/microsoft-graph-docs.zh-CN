---
title: deviceManagementConfigurationChoiceSettingValueTemplate 资源类型
description: 选项设置值模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cffa6a685053194b8ff554d101fecd98f6c6456a
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868432"
---
# <a name="devicemanagementconfigurationchoicesettingvaluetemplate-resource-type"></a><span data-ttu-id="3d003-103">deviceManagementConfigurationChoiceSettingValueTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d003-103">deviceManagementConfigurationChoiceSettingValueTemplate resource type</span></span>

<span data-ttu-id="3d003-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d003-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d003-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3d003-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d003-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d003-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d003-107">选项设置值模板</span><span class="sxs-lookup"><span data-stu-id="3d003-107">Choice Setting Value Template</span></span>

## <a name="properties"></a><span data-ttu-id="3d003-108">属性</span><span class="sxs-lookup"><span data-stu-id="3d003-108">Properties</span></span>
|<span data-ttu-id="3d003-109">属性</span><span class="sxs-lookup"><span data-stu-id="3d003-109">Property</span></span>|<span data-ttu-id="3d003-110">类型</span><span class="sxs-lookup"><span data-stu-id="3d003-110">Type</span></span>|<span data-ttu-id="3d003-111">说明</span><span class="sxs-lookup"><span data-stu-id="3d003-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d003-112">defaultValue</span><span class="sxs-lookup"><span data-stu-id="3d003-112">defaultValue</span></span>|[<span data-ttu-id="3d003-113">deviceManagementConfigurationChoiceSettingValueDefaultTemplate</span><span class="sxs-lookup"><span data-stu-id="3d003-113">deviceManagementConfigurationChoiceSettingValueDefaultTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefaulttemplate.md)|<span data-ttu-id="3d003-114">选项设置值默认模板。</span><span class="sxs-lookup"><span data-stu-id="3d003-114">Choice Setting Value Default Template.</span></span>|
|<span data-ttu-id="3d003-115">recommendedValueDefinition</span><span class="sxs-lookup"><span data-stu-id="3d003-115">recommendedValueDefinition</span></span>|[<span data-ttu-id="3d003-116">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="3d003-116">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefinitiontemplate.md)|<span data-ttu-id="3d003-117">建议的定义替代。</span><span class="sxs-lookup"><span data-stu-id="3d003-117">Recommended definition override.</span></span>|
|<span data-ttu-id="3d003-118">requiredValueDefinition</span><span class="sxs-lookup"><span data-stu-id="3d003-118">requiredValueDefinition</span></span>|[<span data-ttu-id="3d003-119">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="3d003-119">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefinitiontemplate.md)|<span data-ttu-id="3d003-120">必需的定义重写。</span><span class="sxs-lookup"><span data-stu-id="3d003-120">Required definition override.</span></span>|
|<span data-ttu-id="3d003-121">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="3d003-121">settingValueTemplateId</span></span>|<span data-ttu-id="3d003-122">String</span><span class="sxs-lookup"><span data-stu-id="3d003-122">String</span></span>|<span data-ttu-id="3d003-123">设置值模板 ID</span><span class="sxs-lookup"><span data-stu-id="3d003-123">Setting Value Template Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d003-124">关系</span><span class="sxs-lookup"><span data-stu-id="3d003-124">Relationships</span></span>
<span data-ttu-id="3d003-125">无</span><span class="sxs-lookup"><span data-stu-id="3d003-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d003-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d003-126">JSON Representation</span></span>
<span data-ttu-id="3d003-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d003-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingValueTemplate",
  "defaultValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate",
    "settingDefinitionOptionId": "String",
    "children": [
      {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
        "settingInstanceTemplateId": "String",
        "settingDefinitionId": "String",
        "isRequired": true,
        "simpleSettingValueTemplate": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
          "settingValueTemplateId": "String"
        }
      }
    ]
  },
  "recommendedValueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
    "allowedOptions": [
      {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
        "itemId": "String",
        "children": [
          {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
            "settingInstanceTemplateId": "String",
            "settingDefinitionId": "String",
            "isRequired": true,
            "simpleSettingValueTemplate": {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
              "settingValueTemplateId": "String"
            }
          }
        ]
      }
    ]
  },
  "requiredValueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
    "allowedOptions": [
      {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
        "itemId": "String",
        "children": [
          {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
            "settingInstanceTemplateId": "String",
            "settingDefinitionId": "String",
            "isRequired": true,
            "simpleSettingValueTemplate": {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
              "settingValueTemplateId": "String"
            }
          }
        ]
      }
    ]
  },
  "settingValueTemplateId": "String"
}
```




