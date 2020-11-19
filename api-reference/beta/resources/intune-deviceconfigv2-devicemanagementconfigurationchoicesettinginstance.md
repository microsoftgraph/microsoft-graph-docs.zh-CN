---
title: deviceManagementConfigurationChoiceSettingInstance 资源类型
description: 策略内的设置实例
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 591c99a1089a9a01acb6b4ded72439f98d3afbb1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241454"
---
# <a name="devicemanagementconfigurationchoicesettinginstance-resource-type"></a><span data-ttu-id="22117-103">deviceManagementConfigurationChoiceSettingInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="22117-103">deviceManagementConfigurationChoiceSettingInstance resource type</span></span>

<span data-ttu-id="22117-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22117-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22117-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="22117-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22117-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22117-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22117-107">策略内的设置实例</span><span class="sxs-lookup"><span data-stu-id="22117-107">Setting instance within policy</span></span>


<span data-ttu-id="22117-108">继承自 [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="22117-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="22117-109">属性</span><span class="sxs-lookup"><span data-stu-id="22117-109">Properties</span></span>
|<span data-ttu-id="22117-110">属性</span><span class="sxs-lookup"><span data-stu-id="22117-110">Property</span></span>|<span data-ttu-id="22117-111">类型</span><span class="sxs-lookup"><span data-stu-id="22117-111">Type</span></span>|<span data-ttu-id="22117-112">说明</span><span class="sxs-lookup"><span data-stu-id="22117-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22117-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="22117-113">settingDefinitionId</span></span>|<span data-ttu-id="22117-114">String</span><span class="sxs-lookup"><span data-stu-id="22117-114">String</span></span>|<span data-ttu-id="22117-115">从[DeviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)继承的设置定义 Id</span><span class="sxs-lookup"><span data-stu-id="22117-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="22117-116">choiceSettingValue</span><span class="sxs-lookup"><span data-stu-id="22117-116">choiceSettingValue</span></span>|[<span data-ttu-id="22117-117">deviceManagementConfigurationChoiceSettingValue</span><span class="sxs-lookup"><span data-stu-id="22117-117">deviceManagementConfigurationChoiceSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvalue.md)|<span data-ttu-id="22117-118">选项设置值</span><span class="sxs-lookup"><span data-stu-id="22117-118">Choice setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="22117-119">关系</span><span class="sxs-lookup"><span data-stu-id="22117-119">Relationships</span></span>
<span data-ttu-id="22117-120">无</span><span class="sxs-lookup"><span data-stu-id="22117-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22117-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22117-121">JSON Representation</span></span>
<span data-ttu-id="22117-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22117-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
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
                                                                "children": [
                                                                  {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                    "settingDefinitionId": "String",
                                                                    "choiceSettingValue": null
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
}
```




