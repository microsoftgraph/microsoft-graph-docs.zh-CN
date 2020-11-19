---
title: deviceManagementConfigurationOptionDefinition 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5c8ccb388a8feb43b6be96402d45a5b7a0ae62ed
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241418"
---
# <a name="devicemanagementconfigurationoptiondefinition-resource-type"></a><span data-ttu-id="5c005-103">deviceManagementConfigurationOptionDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c005-103">deviceManagementConfigurationOptionDefinition resource type</span></span>

<span data-ttu-id="5c005-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c005-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c005-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5c005-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c005-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5c005-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c005-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5c005-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5c005-108">属性</span><span class="sxs-lookup"><span data-stu-id="5c005-108">Properties</span></span>
|<span data-ttu-id="5c005-109">属性</span><span class="sxs-lookup"><span data-stu-id="5c005-109">Property</span></span>|<span data-ttu-id="5c005-110">类型</span><span class="sxs-lookup"><span data-stu-id="5c005-110">Type</span></span>|<span data-ttu-id="5c005-111">说明</span><span class="sxs-lookup"><span data-stu-id="5c005-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c005-112">optionValue</span><span class="sxs-lookup"><span data-stu-id="5c005-112">optionValue</span></span>|[<span data-ttu-id="5c005-113">deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="5c005-113">deviceManagementConfigurationSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|<span data-ttu-id="5c005-114">选项的值</span><span class="sxs-lookup"><span data-stu-id="5c005-114">Value of the option</span></span>|
|<span data-ttu-id="5c005-115">dependentOn</span><span class="sxs-lookup"><span data-stu-id="5c005-115">dependentOn</span></span>|<span data-ttu-id="5c005-116">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5c005-116">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="5c005-117">此选项的相关设置列表</span><span class="sxs-lookup"><span data-stu-id="5c005-117">List of dependent settings for this option</span></span>|
|<span data-ttu-id="5c005-118">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="5c005-118">dependedOnBy</span></span>|<span data-ttu-id="5c005-119">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5c005-119">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="5c005-120">取决于此选项的设置列表</span><span class="sxs-lookup"><span data-stu-id="5c005-120">List of Settings that depends on this option</span></span>|
|<span data-ttu-id="5c005-121">itemId</span><span class="sxs-lookup"><span data-stu-id="5c005-121">itemId</span></span>|<span data-ttu-id="5c005-122">String</span><span class="sxs-lookup"><span data-stu-id="5c005-122">String</span></span>|<span data-ttu-id="5c005-123">选项的标识符</span><span class="sxs-lookup"><span data-stu-id="5c005-123">Identifier of option</span></span>|
|<span data-ttu-id="5c005-124">description</span><span class="sxs-lookup"><span data-stu-id="5c005-124">description</span></span>|<span data-ttu-id="5c005-125">String</span><span class="sxs-lookup"><span data-stu-id="5c005-125">String</span></span>|<span data-ttu-id="5c005-126">选项的说明</span><span class="sxs-lookup"><span data-stu-id="5c005-126">Description of the option</span></span>|
|<span data-ttu-id="5c005-127">helpText</span><span class="sxs-lookup"><span data-stu-id="5c005-127">helpText</span></span>|<span data-ttu-id="5c005-128">String</span><span class="sxs-lookup"><span data-stu-id="5c005-128">String</span></span>|<span data-ttu-id="5c005-129">选项的帮助文本</span><span class="sxs-lookup"><span data-stu-id="5c005-129">Help text of the option</span></span>|
|<span data-ttu-id="5c005-130">name</span><span class="sxs-lookup"><span data-stu-id="5c005-130">name</span></span>|<span data-ttu-id="5c005-131">String</span><span class="sxs-lookup"><span data-stu-id="5c005-131">String</span></span>|<span data-ttu-id="5c005-132">选项的名称</span><span class="sxs-lookup"><span data-stu-id="5c005-132">Name of the option</span></span>|
|<span data-ttu-id="5c005-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5c005-133">displayName</span></span>|<span data-ttu-id="5c005-134">String</span><span class="sxs-lookup"><span data-stu-id="5c005-134">String</span></span>|<span data-ttu-id="5c005-135">选项的友好名称</span><span class="sxs-lookup"><span data-stu-id="5c005-135">Friendly name of the option</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c005-136">关系</span><span class="sxs-lookup"><span data-stu-id="5c005-136">Relationships</span></span>
<span data-ttu-id="5c005-137">无</span><span class="sxs-lookup"><span data-stu-id="5c005-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c005-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c005-138">JSON Representation</span></span>
<span data-ttu-id="5c005-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c005-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationOptionDefinition",
  "optionValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValue",
    "children": [
      {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
        "settingDefinitionId": "String",
        "choiceSettingValue": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
          "value": "String",
          "children": [
            {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
              "settingDefinitionId": "String",
              "choiceSettingValue": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                "value": "String",
                "children": [
                  {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                    "settingDefinitionId": "String",
                    "choiceSettingValue": {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                      "value": "String",
                      "children": [
                        {
                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                          "settingDefinitionId": "String",
                          "choiceSettingValue": {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                            "value": "String",
                            "children": [
                              {
                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                "settingDefinitionId": "String",
                                "choiceSettingValue": {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                  "value": "String",
                                  "children": [
                                    {
                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                      "settingDefinitionId": "String",
                                      "choiceSettingValue": {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                        "value": "String",
                                        "children": [
                                          {
                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                            "settingDefinitionId": "String",
                                            "choiceSettingValue": {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                              "value": "String",
                                              "children": [
                                                {
                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                  "settingDefinitionId": "String",
                                                  "choiceSettingValue": {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                    "value": "String",
                                                    "children": [
                                                      {
                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                        "settingDefinitionId": "String",
                                                        "choiceSettingValue": {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                          "value": "String",
                                                          "children": [
                                                            {
                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                              "settingDefinitionId": "String",
                                                              "choiceSettingValue": {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                "value": "String",
                                                                "children": [
                                                                  {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                    "settingDefinitionId": "String",
                                                                    "choiceSettingValue": {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                      "value": "String",
                                                                      "children": null
                                                                    }
                                                                  }
                                                                ]
                                                              }
                                                            }
                                                          ]
                                                        }
                                                      }
                                                    ]
                                                  }
                                                }
                                              ]
                                            }
                                          }
                                        ]
                                      }
                                    }
                                  ]
                                }
                              }
                            ]
                          }
                        }
                      ]
                    }
                  }
                ]
              }
            }
          ]
        }
      }
    ]
  },
  "dependentOn": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn",
      "dependentOn": "String",
      "parentSettingId": "String"
    }
  ],
  "dependedOnBy": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
      "dependedOnBy": "String",
      "required": true
    }
  ],
  "itemId": "String",
  "description": "String",
  "helpText": "String",
  "name": "String",
  "displayName": "String"
}
```




