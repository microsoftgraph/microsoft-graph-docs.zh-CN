---
title: deviceManagementConfigurationOptionDefinition 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cffbb4ccf98637b4fe65b5b593e947fb1dab5c06
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666518"
---
# <a name="devicemanagementconfigurationoptiondefinition-resource-type"></a><span data-ttu-id="1cd7e-103">deviceManagementConfigurationOptionDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="1cd7e-103">deviceManagementConfigurationOptionDefinition resource type</span></span>

<span data-ttu-id="1cd7e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cd7e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1cd7e-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1cd7e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cd7e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1cd7e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cd7e-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1cd7e-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1cd7e-108">属性</span><span class="sxs-lookup"><span data-stu-id="1cd7e-108">Properties</span></span>
|<span data-ttu-id="1cd7e-109">属性</span><span class="sxs-lookup"><span data-stu-id="1cd7e-109">Property</span></span>|<span data-ttu-id="1cd7e-110">类型</span><span class="sxs-lookup"><span data-stu-id="1cd7e-110">Type</span></span>|<span data-ttu-id="1cd7e-111">说明</span><span class="sxs-lookup"><span data-stu-id="1cd7e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cd7e-112">optionValue</span><span class="sxs-lookup"><span data-stu-id="1cd7e-112">optionValue</span></span>|[<span data-ttu-id="1cd7e-113">deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="1cd7e-113">deviceManagementConfigurationSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|<span data-ttu-id="1cd7e-114">选项的值</span><span class="sxs-lookup"><span data-stu-id="1cd7e-114">Value of the option</span></span>|
|<span data-ttu-id="1cd7e-115">dependentOn</span><span class="sxs-lookup"><span data-stu-id="1cd7e-115">dependentOn</span></span>|<span data-ttu-id="1cd7e-116">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1cd7e-116">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="1cd7e-117">此选项的依赖设置列表</span><span class="sxs-lookup"><span data-stu-id="1cd7e-117">List of dependent settings for this option</span></span>|
|<span data-ttu-id="1cd7e-118">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="1cd7e-118">dependedOnBy</span></span>|<span data-ttu-id="1cd7e-119">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1cd7e-119">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="1cd7e-120">依赖于设置的列表</span><span class="sxs-lookup"><span data-stu-id="1cd7e-120">List of Settings that depends on this option</span></span>|
|<span data-ttu-id="1cd7e-121">itemId</span><span class="sxs-lookup"><span data-stu-id="1cd7e-121">itemId</span></span>|<span data-ttu-id="1cd7e-122">String</span><span class="sxs-lookup"><span data-stu-id="1cd7e-122">String</span></span>|<span data-ttu-id="1cd7e-123">选项的标识符</span><span class="sxs-lookup"><span data-stu-id="1cd7e-123">Identifier of option</span></span>|
|<span data-ttu-id="1cd7e-124">说明</span><span class="sxs-lookup"><span data-stu-id="1cd7e-124">description</span></span>|<span data-ttu-id="1cd7e-125">String</span><span class="sxs-lookup"><span data-stu-id="1cd7e-125">String</span></span>|<span data-ttu-id="1cd7e-126">选项的说明</span><span class="sxs-lookup"><span data-stu-id="1cd7e-126">Description of the option</span></span>|
|<span data-ttu-id="1cd7e-127">helpText</span><span class="sxs-lookup"><span data-stu-id="1cd7e-127">helpText</span></span>|<span data-ttu-id="1cd7e-128">String</span><span class="sxs-lookup"><span data-stu-id="1cd7e-128">String</span></span>|<span data-ttu-id="1cd7e-129">选项的帮助文本</span><span class="sxs-lookup"><span data-stu-id="1cd7e-129">Help text of the option</span></span>|
|<span data-ttu-id="1cd7e-130">name</span><span class="sxs-lookup"><span data-stu-id="1cd7e-130">name</span></span>|<span data-ttu-id="1cd7e-131">String</span><span class="sxs-lookup"><span data-stu-id="1cd7e-131">String</span></span>|<span data-ttu-id="1cd7e-132">选项的名称</span><span class="sxs-lookup"><span data-stu-id="1cd7e-132">Name of the option</span></span>|
|<span data-ttu-id="1cd7e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1cd7e-133">displayName</span></span>|<span data-ttu-id="1cd7e-134">String</span><span class="sxs-lookup"><span data-stu-id="1cd7e-134">String</span></span>|<span data-ttu-id="1cd7e-135">选项的友好名称</span><span class="sxs-lookup"><span data-stu-id="1cd7e-135">Friendly name of the option</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cd7e-136">关系</span><span class="sxs-lookup"><span data-stu-id="1cd7e-136">Relationships</span></span>
<span data-ttu-id="1cd7e-137">无</span><span class="sxs-lookup"><span data-stu-id="1cd7e-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1cd7e-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1cd7e-138">JSON Representation</span></span>
<span data-ttu-id="1cd7e-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1cd7e-139">Here is a JSON representation of the resource.</span></span>
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
    "settingValueTemplateReference": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
      "settingValueTemplateId": "String",
      "useTemplateDefault": true
    },
    "children": [
      {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
        "settingDefinitionId": "String",
        "settingInstanceTemplateReference": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
          "settingInstanceTemplateId": "String"
        },
        "choiceSettingValue": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
          "settingValueTemplateReference": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
            "settingValueTemplateId": "String",
            "useTemplateDefault": true
          },
          "value": "String",
          "children": [
            {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
              "settingDefinitionId": "String",
              "settingInstanceTemplateReference": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                "settingInstanceTemplateId": "String"
              },
              "choiceSettingValue": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                "settingValueTemplateReference": {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                  "settingValueTemplateId": "String",
                  "useTemplateDefault": true
                },
                "value": "String",
                "children": [
                  {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                    "settingDefinitionId": "String",
                    "settingInstanceTemplateReference": {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                      "settingInstanceTemplateId": "String"
                    },
                    "choiceSettingValue": {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                      "settingValueTemplateReference": {
                        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                        "settingValueTemplateId": "String",
                        "useTemplateDefault": true
                      },
                      "value": "String",
                      "children": [
                        {
                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                          "settingDefinitionId": "String",
                          "settingInstanceTemplateReference": {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                            "settingInstanceTemplateId": "String"
                          },
                          "choiceSettingValue": {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                            "settingValueTemplateReference": {
                              "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                              "settingValueTemplateId": "String",
                              "useTemplateDefault": true
                            },
                            "value": "String",
                            "children": [
                              {
                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                "settingDefinitionId": "String",
                                "settingInstanceTemplateReference": {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                  "settingInstanceTemplateId": "String"
                                },
                                "choiceSettingValue": {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                  "settingValueTemplateReference": {
                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                    "settingValueTemplateId": "String",
                                    "useTemplateDefault": true
                                  },
                                  "value": "String",
                                  "children": [
                                    {
                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                      "settingDefinitionId": "String",
                                      "settingInstanceTemplateReference": {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                        "settingInstanceTemplateId": "String"
                                      },
                                      "choiceSettingValue": {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                        "settingValueTemplateReference": {
                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                          "settingValueTemplateId": "String",
                                          "useTemplateDefault": true
                                        },
                                        "value": "String",
                                        "children": [
                                          {
                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                            "settingDefinitionId": "String",
                                            "settingInstanceTemplateReference": {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                              "settingInstanceTemplateId": "String"
                                            },
                                            "choiceSettingValue": {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                              "settingValueTemplateReference": {
                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                "settingValueTemplateId": "String",
                                                "useTemplateDefault": true
                                              },
                                              "value": "String",
                                              "children": [
                                                {
                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                  "settingDefinitionId": "String",
                                                  "settingInstanceTemplateReference": {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                    "settingInstanceTemplateId": "String"
                                                  },
                                                  "choiceSettingValue": {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                    "settingValueTemplateReference": {
                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                      "settingValueTemplateId": "String",
                                                      "useTemplateDefault": true
                                                    },
                                                    "value": "String",
                                                    "children": [
                                                      {
                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                        "settingDefinitionId": "String",
                                                        "settingInstanceTemplateReference": {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                          "settingInstanceTemplateId": "String"
                                                        },
                                                        "choiceSettingValue": {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                          "settingValueTemplateReference": {
                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                            "settingValueTemplateId": "String",
                                                            "useTemplateDefault": true
                                                          },
                                                          "value": "String",
                                                          "children": [
                                                            {
                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                              "settingDefinitionId": "String",
                                                              "settingInstanceTemplateReference": {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                                "settingInstanceTemplateId": "String"
                                                              },
                                                              "choiceSettingValue": {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                "settingValueTemplateReference": {
                                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                                  "settingValueTemplateId": "String",
                                                                  "useTemplateDefault": true
                                                                },
                                                                "value": "String",
                                                                "children": [
                                                                  {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                    "settingDefinitionId": "String",
                                                                    "settingInstanceTemplateReference": {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                                      "settingInstanceTemplateId": "String"
                                                                    },
                                                                    "choiceSettingValue": {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                      "settingValueTemplateReference": null,
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




