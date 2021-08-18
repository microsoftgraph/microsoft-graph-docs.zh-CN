---
title: deviceManagementReusablePolicySetting 资源类型
description: Graph可重用设置的模型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d9139d11d35ab76bfcec96e0b0b04f8a947873e826ecb4678ff5d82b1333352d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54248444"
---
# <a name="devicemanagementreusablepolicysetting-resource-type"></a>deviceManagementReusablePolicySetting 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Graph可重用设置的模型

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementReusablePolicySettings](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-list.md)|[deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) 集合|列出 [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) 对象的属性和关系。|
|[获取 deviceManagementReusablePolicySetting](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-get.md)|[deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)|读取 [deviceManagementReusablePolicySetting 对象的属性和](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) 关系。|
|[创建 deviceManagementReusablePolicySetting](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-create.md)|[deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)|创建新的 [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) 对象。|
|[删除 deviceManagementReusablePolicySetting](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-delete.md)|无|删除 [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)。|
|[更新 deviceManagementReusablePolicySetting](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-update.md)|[deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)|更新 [deviceManagementReusablePolicySetting 对象](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) 的属性。|
|[clone 操作](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-clone.md)|[deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|系统生成的可重用设置 ID。|
|displayName|String|用户可显示名称可重用设置。|
|description|String|由用户提供的可重用设置说明。|
|settingDefinitionId|String|与此可重用设置关联的设置定义 ID。|
|settingInstance|[deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|可重用的设置配置实例|
|createdDateTime|DateTimeOffset|可重用设置创建日期和时间。 此属性是只读的。|
|lastModifiedDateTime|DateTimeOffset|上次修改可重用设置的日期和时间。 此属性是只读的。|
|version|Int32|可重复使用设置的版本号。 有效值为 0 到 2147483647。 此属性是只读的。|
|referencingConfigurationPolicyCount|Int32|引用当前可重用设置的配置策略计数。 有效值为 0 到 2147483647。 此属性是只读的。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|referencingConfigurationPolicies|[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 集合|引用当前可重用设置的配置策略|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReusablePolicySetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReusablePolicySetting",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "settingDefinitionId": "String",
  "settingInstance": {
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
                                                                  "settingValueTemplateReference": {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                                    "settingValueTemplateId": "String",
                                                                    "useTemplateDefault": true
                                                                  },
                                                                  "value": "String",
                                                                  "children": [
                                                                    {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                      "settingDefinitionId": null,
                                                                      "settingInstanceTemplateReference": null,
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
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "referencingConfigurationPolicyCount": 1024
}
```




