---
title: deviceManagementConfigurationChoiceSettingCollectionInstance 资源类型
description: 策略内的设置实例
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c184daa530de199afc5240b42cbcb1d8204f96df
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241458"
---
# <a name="devicemanagementconfigurationchoicesettingcollectioninstance-resource-type"></a><span data-ttu-id="7e730-103">deviceManagementConfigurationChoiceSettingCollectionInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e730-103">deviceManagementConfigurationChoiceSettingCollectionInstance resource type</span></span>

<span data-ttu-id="7e730-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e730-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e730-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7e730-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e730-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7e730-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e730-107">策略内的设置实例</span><span class="sxs-lookup"><span data-stu-id="7e730-107">Setting instance within policy</span></span>


<span data-ttu-id="7e730-108">继承自 [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="7e730-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7e730-109">属性</span><span class="sxs-lookup"><span data-stu-id="7e730-109">Properties</span></span>
|<span data-ttu-id="7e730-110">属性</span><span class="sxs-lookup"><span data-stu-id="7e730-110">Property</span></span>|<span data-ttu-id="7e730-111">类型</span><span class="sxs-lookup"><span data-stu-id="7e730-111">Type</span></span>|<span data-ttu-id="7e730-112">说明</span><span class="sxs-lookup"><span data-stu-id="7e730-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e730-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7e730-113">settingDefinitionId</span></span>|<span data-ttu-id="7e730-114">String</span><span class="sxs-lookup"><span data-stu-id="7e730-114">String</span></span>|<span data-ttu-id="7e730-115">从[DeviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)继承的设置定义 Id</span><span class="sxs-lookup"><span data-stu-id="7e730-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="7e730-116">choiceSettingCollectionValue</span><span class="sxs-lookup"><span data-stu-id="7e730-116">choiceSettingCollectionValue</span></span>|<span data-ttu-id="7e730-117">[deviceManagementConfigurationChoiceSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e730-117">[deviceManagementConfigurationChoiceSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvalue.md) collection</span></span>|<span data-ttu-id="7e730-118">选项设置集合值</span><span class="sxs-lookup"><span data-stu-id="7e730-118">Choice setting collection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e730-119">关系</span><span class="sxs-lookup"><span data-stu-id="7e730-119">Relationships</span></span>
<span data-ttu-id="7e730-120">无</span><span class="sxs-lookup"><span data-stu-id="7e730-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e730-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e730-121">JSON Representation</span></span>
<span data-ttu-id="7e730-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e730-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionInstance",
  "settingDefinitionId": "String",
  "choiceSettingCollectionValue": [
    {
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
                                                                  "children": [
                                                                    {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                      "settingDefinitionId": "String",
                                                                      "choiceSettingValue": {
                                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                        "value": null,
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
  ]
}
```




