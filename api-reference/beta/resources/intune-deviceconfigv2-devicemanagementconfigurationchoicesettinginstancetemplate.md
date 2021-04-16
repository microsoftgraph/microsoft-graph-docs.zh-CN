---
title: deviceManagementConfigurationChoiceSettingInstanceTemplate 资源类型
description: 选项设置实例模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b7c894e455d96f1fb7e8c2cd7a50beaff009858f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868443"
---
# <a name="devicemanagementconfigurationchoicesettinginstancetemplate-resource-type"></a><span data-ttu-id="3caeb-103">deviceManagementConfigurationChoiceSettingInstanceTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="3caeb-103">deviceManagementConfigurationChoiceSettingInstanceTemplate resource type</span></span>

<span data-ttu-id="3caeb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3caeb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3caeb-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3caeb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3caeb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3caeb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3caeb-107">选项设置实例模板</span><span class="sxs-lookup"><span data-stu-id="3caeb-107">Choice Setting Instance Template</span></span>


<span data-ttu-id="3caeb-108">继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="3caeb-108">Inherits from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3caeb-109">属性</span><span class="sxs-lookup"><span data-stu-id="3caeb-109">Properties</span></span>
|<span data-ttu-id="3caeb-110">属性</span><span class="sxs-lookup"><span data-stu-id="3caeb-110">Property</span></span>|<span data-ttu-id="3caeb-111">类型</span><span class="sxs-lookup"><span data-stu-id="3caeb-111">Type</span></span>|<span data-ttu-id="3caeb-112">说明</span><span class="sxs-lookup"><span data-stu-id="3caeb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3caeb-113">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="3caeb-113">settingInstanceTemplateId</span></span>|<span data-ttu-id="3caeb-114">String</span><span class="sxs-lookup"><span data-stu-id="3caeb-114">String</span></span>|<span data-ttu-id="3caeb-115">设置实例模板 ID 继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="3caeb-115">Setting Instance Template Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="3caeb-116">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="3caeb-116">settingDefinitionId</span></span>|<span data-ttu-id="3caeb-117">String</span><span class="sxs-lookup"><span data-stu-id="3caeb-117">String</span></span>|<span data-ttu-id="3caeb-118">设置定义 ID 继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="3caeb-118">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="3caeb-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="3caeb-119">isRequired</span></span>|<span data-ttu-id="3caeb-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="3caeb-120">Boolean</span></span>|<span data-ttu-id="3caeb-121">指示策略是否必须指定此设置。</span><span class="sxs-lookup"><span data-stu-id="3caeb-121">Indicates if a policy must specify this setting.</span></span> <span data-ttu-id="3caeb-122">继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="3caeb-122">Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="3caeb-123">choiceSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="3caeb-123">choiceSettingValueTemplate</span></span>|[<span data-ttu-id="3caeb-124">deviceManagementConfigurationChoiceSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="3caeb-124">deviceManagementConfigurationChoiceSettingValueTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluetemplate.md)|<span data-ttu-id="3caeb-125">选项设置值模板</span><span class="sxs-lookup"><span data-stu-id="3caeb-125">Choice Setting Value Template</span></span>|

## <a name="relationships"></a><span data-ttu-id="3caeb-126">关系</span><span class="sxs-lookup"><span data-stu-id="3caeb-126">Relationships</span></span>
<span data-ttu-id="3caeb-127">无</span><span class="sxs-lookup"><span data-stu-id="3caeb-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3caeb-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3caeb-128">JSON Representation</span></span>
<span data-ttu-id="3caeb-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3caeb-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "choiceSettingValueTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueTemplate",
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
}
```




