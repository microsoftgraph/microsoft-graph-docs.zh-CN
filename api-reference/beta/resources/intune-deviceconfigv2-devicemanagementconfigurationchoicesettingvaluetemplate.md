---
title: deviceManagementConfigurationChoiceSettingValueTemplate 资源类型
description: 选项设置值模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 10d446532e0664c6d83d16d223c0a8e0d966aeb4
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666574"
---
# <a name="devicemanagementconfigurationchoicesettingvaluetemplate-resource-type"></a><span data-ttu-id="23e0e-103">deviceManagementConfigurationChoiceSettingValueTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="23e0e-103">deviceManagementConfigurationChoiceSettingValueTemplate resource type</span></span>

<span data-ttu-id="23e0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23e0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23e0e-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="23e0e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23e0e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23e0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23e0e-107">选项设置值模板</span><span class="sxs-lookup"><span data-stu-id="23e0e-107">Choice Setting Value Template</span></span>

## <a name="properties"></a><span data-ttu-id="23e0e-108">属性</span><span class="sxs-lookup"><span data-stu-id="23e0e-108">Properties</span></span>
|<span data-ttu-id="23e0e-109">属性</span><span class="sxs-lookup"><span data-stu-id="23e0e-109">Property</span></span>|<span data-ttu-id="23e0e-110">类型</span><span class="sxs-lookup"><span data-stu-id="23e0e-110">Type</span></span>|<span data-ttu-id="23e0e-111">说明</span><span class="sxs-lookup"><span data-stu-id="23e0e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23e0e-112">defaultValue</span><span class="sxs-lookup"><span data-stu-id="23e0e-112">defaultValue</span></span>|[<span data-ttu-id="23e0e-113">deviceManagementConfigurationChoiceSettingValueDefaultTemplate</span><span class="sxs-lookup"><span data-stu-id="23e0e-113">deviceManagementConfigurationChoiceSettingValueDefaultTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefaulttemplate.md)|<span data-ttu-id="23e0e-114">选项设置值默认模板。</span><span class="sxs-lookup"><span data-stu-id="23e0e-114">Choice Setting Value Default Template.</span></span>|
|<span data-ttu-id="23e0e-115">recommendedValueDefinition</span><span class="sxs-lookup"><span data-stu-id="23e0e-115">recommendedValueDefinition</span></span>|[<span data-ttu-id="23e0e-116">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="23e0e-116">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefinitiontemplate.md)|<span data-ttu-id="23e0e-117">建议的定义替代。</span><span class="sxs-lookup"><span data-stu-id="23e0e-117">Recommended definition override.</span></span>|
|<span data-ttu-id="23e0e-118">requiredValueDefinition</span><span class="sxs-lookup"><span data-stu-id="23e0e-118">requiredValueDefinition</span></span>|[<span data-ttu-id="23e0e-119">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="23e0e-119">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefinitiontemplate.md)|<span data-ttu-id="23e0e-120">必需的定义重写。</span><span class="sxs-lookup"><span data-stu-id="23e0e-120">Required definition override.</span></span>|
|<span data-ttu-id="23e0e-121">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="23e0e-121">settingValueTemplateId</span></span>|<span data-ttu-id="23e0e-122">String</span><span class="sxs-lookup"><span data-stu-id="23e0e-122">String</span></span>|<span data-ttu-id="23e0e-123">设置值模板 ID</span><span class="sxs-lookup"><span data-stu-id="23e0e-123">Setting Value Template Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="23e0e-124">关系</span><span class="sxs-lookup"><span data-stu-id="23e0e-124">Relationships</span></span>
<span data-ttu-id="23e0e-125">无</span><span class="sxs-lookup"><span data-stu-id="23e0e-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23e0e-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23e0e-126">JSON Representation</span></span>
<span data-ttu-id="23e0e-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23e0e-127">Here is a JSON representation of the resource.</span></span>
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
          "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
          "settingValueTemplateId": "String",
          "defaultValue": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
            "constantValue": "String"
          }
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
    ]
  },
  "settingValueTemplateId": "String"
}
```




