---
title: deviceManagementConfigurationSimpleSettingDefinition 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5f4d0b1c0aa12dc9f4335d12028c584a2c62b952
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668669"
---
# <a name="devicemanagementconfigurationsimplesettingdefinition-resource-type"></a>deviceManagementConfigurationSimpleSettingDefinition 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录


继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementConfigurationSimpleSettingDefinitions](../api/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition-list.md)|[deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) 集合|列出 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) 对象的属性和关系。|
|[获取 deviceManagementConfigurationSimpleSettingDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition-get.md)|[deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)|读取 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) 对象的属性和关系。|
|[创建 deviceManagementConfigurationSimpleSettingDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition-create.md)|[deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)|创建新的 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) 对象。|
|[删除 deviceManagementConfigurationSimpleSettingDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition-delete.md)|None|删除 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)。|
|[更新 deviceManagementConfigurationSimpleSettingDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition-update.md)|[deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)|更新 [deviceManagementConfigurationSimpleSettingDefinition 对象的](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) 属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|适用性|[deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|详细信息：从 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 继承的设备设置适用|
|accessTypes|[deviceManagementConfigurationSettingAccessTypes](../resources/intune-shared-devicemanagementconfigurationsettingaccesstypes.md)|从 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 继承的设置的读/写访问模式。 可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。|
|keywords|字符串集合|要在从 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 上搜索设置的令牌|
|infoUrls|字符串集合|可在从 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 继承处找到有关设置的链接的详细信息列表|
|发生|[deviceManagementConfigurationSettingOccurrence](../resources/intune-shared-devicemanagementconfigurationsettingoccurrence.md)|指示是否需要设置从 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 继承|
|baseUri|String|从 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 继承的基本 CSP 路径|
|offsetUri|String|从 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 继承的基础的偏移 CSP 路径|
|rootDefinitionId|String|根设置定义（如果设置是子设置）。 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|categoryId|字符串|指定在指定的配置服务提供程序中配置设置的区域组 (CSP) 从 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 继承|
|settingUsage|[deviceManagementConfigurationSettingUsage](../resources/intune-shared-devicemanagementconfigurationsettingusage.md)|设置类型，例如，从 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 继承的配置和符合性。 可取值为：`none`、`configuration`、`compliance`。|
|uxBehavior|[deviceManagementConfigurationControlType](../resources/intune-shared-devicemanagementconfigurationcontroltype.md)|在从 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 继承的 UX 中设置控件类型表示形式。 可取值为：`default`、`dropdown`、`smallTextBox`、`largeTextBox`、`toggle`、`multiheaderGrid` 或 `contextPane`。|
|visibility|[deviceManagementConfigurationSettingVisibility](../resources/intune-shared-devicemanagementconfigurationsettingvisibility.md)|将可见性范围设置为从 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 继承的 UX。 可取值为：`none`、`settingsCatalog`、`template`。|
|referredSettingInformationList|[deviceManagementConfigurationReferredSettingInformation](../resources/intune-shared-devicemanagementconfigurationreferredsettinginformation.md) 集合|引用的设置信息列表。 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|id|String|从 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 继承的项的标识符|
|说明|字符串|从 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 继承的项目说明|
|helpText|字符串|从 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 继承的项目帮助文本|
|name|String|从 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 继承的项目名称|
|displayName|String|从 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 继承的项的显示名称|
|version|String|从 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 继承的项目版本|
|valueDefinition|[deviceManagementConfigurationSettingValueDefinition](../resources/intune-shared-devicemanagementconfigurationsettingvaluedefinition.md)|此设置的值定义|
|defaultValue|[deviceManagementConfigurationSettingValue](../resources/intune-shared-devicemanagementconfigurationsettingvalue.md)|此设置的默认设置值|
|dependentOn|[deviceManagementConfigurationDependentOn](../resources/intune-shared-devicemanagementconfigurationdependenton.md) 集合|此设置所依赖的父设置列表|
|dependedOnBy|[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-shared-devicemanagementconfigurationsettingdependedonby.md) 集合|依赖于此设置的子设置列表|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingDefinition",
  "applicability": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
    "description": "String",
    "platform": "String",
    "deviceMode": "String",
    "technologies": "String"
  },
  "accessTypes": "String",
  "keywords": [
    "String"
  ],
  "infoUrls": [
    "String"
  ],
  "occurrence": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
    "minDeviceOccurrence": 1024,
    "maxDeviceOccurrence": 1024
  },
  "baseUri": "String",
  "offsetUri": "String",
  "rootDefinitionId": "String",
  "categoryId": "String",
  "settingUsage": "String",
  "uxBehavior": "String",
  "visibility": "String",
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "String"
    }
  ],
  "id": "String (identifier)",
  "description": "String",
  "helpText": "String",
  "name": "String",
  "displayName": "String",
  "version": "String",
  "valueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueDefinition"
  },
  "defaultValue": {
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
  ]
}
```




