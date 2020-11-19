---
title: deviceManagementConfigurationChoiceSettingValue 资源类型
description: 设置值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d7b57e1cb62feb48073207275c249796a2474294
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241453"
---
# <a name="devicemanagementconfigurationchoicesettingvalue-resource-type"></a><span data-ttu-id="264ba-103">deviceManagementConfigurationChoiceSettingValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="264ba-103">deviceManagementConfigurationChoiceSettingValue resource type</span></span>

<span data-ttu-id="264ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="264ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="264ba-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="264ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="264ba-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="264ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="264ba-107">设置值</span><span class="sxs-lookup"><span data-stu-id="264ba-107">Setting value</span></span>


<span data-ttu-id="264ba-108">继承自 [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="264ba-108">Inherits from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="264ba-109">属性</span><span class="sxs-lookup"><span data-stu-id="264ba-109">Properties</span></span>
|<span data-ttu-id="264ba-110">属性</span><span class="sxs-lookup"><span data-stu-id="264ba-110">Property</span></span>|<span data-ttu-id="264ba-111">类型</span><span class="sxs-lookup"><span data-stu-id="264ba-111">Type</span></span>|<span data-ttu-id="264ba-112">说明</span><span class="sxs-lookup"><span data-stu-id="264ba-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="264ba-113">值</span><span class="sxs-lookup"><span data-stu-id="264ba-113">value</span></span>|<span data-ttu-id="264ba-114">String</span><span class="sxs-lookup"><span data-stu-id="264ba-114">String</span></span>|<span data-ttu-id="264ba-115">Choice 设置值： OptionDefinition ItemId。</span><span class="sxs-lookup"><span data-stu-id="264ba-115">Choice setting value: an OptionDefinition ItemId.</span></span>|
|<span data-ttu-id="264ba-116">children</span><span class="sxs-lookup"><span data-stu-id="264ba-116">children</span></span>|<span data-ttu-id="264ba-117">[deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md) 集合</span><span class="sxs-lookup"><span data-stu-id="264ba-117">[deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md) collection</span></span>|<span data-ttu-id="264ba-118">子设置。</span><span class="sxs-lookup"><span data-stu-id="264ba-118">Child settings.</span></span>|

## <a name="relationships"></a><span data-ttu-id="264ba-119">关系</span><span class="sxs-lookup"><span data-stu-id="264ba-119">Relationships</span></span>
<span data-ttu-id="264ba-120">无</span><span class="sxs-lookup"><span data-stu-id="264ba-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="264ba-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="264ba-121">JSON Representation</span></span>
<span data-ttu-id="264ba-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="264ba-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
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
}
```




