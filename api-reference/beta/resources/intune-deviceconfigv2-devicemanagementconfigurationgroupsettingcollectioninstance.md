---
title: deviceManagementConfigurationGroupSettingCollectionInstance 资源类型
description: GroupSettingCollection 的实例
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 40542c7358838f60bfeb30d8e938062fbbc2c7b0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241442"
---
# <a name="devicemanagementconfigurationgroupsettingcollectioninstance-resource-type"></a><span data-ttu-id="2912a-103">deviceManagementConfigurationGroupSettingCollectionInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="2912a-103">deviceManagementConfigurationGroupSettingCollectionInstance resource type</span></span>

<span data-ttu-id="2912a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2912a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2912a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2912a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2912a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2912a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2912a-107">GroupSettingCollection 的实例</span><span class="sxs-lookup"><span data-stu-id="2912a-107">Instance of a GroupSettingCollection</span></span>


<span data-ttu-id="2912a-108">继承自 [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="2912a-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2912a-109">属性</span><span class="sxs-lookup"><span data-stu-id="2912a-109">Properties</span></span>
|<span data-ttu-id="2912a-110">属性</span><span class="sxs-lookup"><span data-stu-id="2912a-110">Property</span></span>|<span data-ttu-id="2912a-111">类型</span><span class="sxs-lookup"><span data-stu-id="2912a-111">Type</span></span>|<span data-ttu-id="2912a-112">说明</span><span class="sxs-lookup"><span data-stu-id="2912a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2912a-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2912a-113">settingDefinitionId</span></span>|<span data-ttu-id="2912a-114">String</span><span class="sxs-lookup"><span data-stu-id="2912a-114">String</span></span>|<span data-ttu-id="2912a-115">从[DeviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)继承的设置定义 Id</span><span class="sxs-lookup"><span data-stu-id="2912a-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="2912a-116">groupSettingCollectionValue</span><span class="sxs-lookup"><span data-stu-id="2912a-116">groupSettingCollectionValue</span></span>|<span data-ttu-id="2912a-117">[deviceManagementConfigurationGroupSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationgroupsettingvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2912a-117">[deviceManagementConfigurationGroupSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationgroupsettingvalue.md) collection</span></span>|<span data-ttu-id="2912a-118">GroupSetting 值的集合</span><span class="sxs-lookup"><span data-stu-id="2912a-118">A collection of GroupSetting values</span></span>|

## <a name="relationships"></a><span data-ttu-id="2912a-119">关系</span><span class="sxs-lookup"><span data-stu-id="2912a-119">Relationships</span></span>
<span data-ttu-id="2912a-120">无</span><span class="sxs-lookup"><span data-stu-id="2912a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2912a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2912a-121">JSON Representation</span></span>
<span data-ttu-id="2912a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2912a-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationGroupSettingCollectionInstance",
  "settingDefinitionId": "String",
  "groupSettingCollectionValue": [
    {
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
    }
  ]
}
```




