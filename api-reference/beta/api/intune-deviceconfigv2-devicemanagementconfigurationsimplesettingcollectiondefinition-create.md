---
title: 创建 deviceManagementConfigurationSimpleSettingCollectionDefinition
description: 创建新的 deviceManagementConfigurationSimpleSettingCollectionDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e8f1028ea726218f30fe4f4499d60cead5f4472d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129179"
---
# <a name="create-devicemanagementconfigurationsimplesettingcollectiondefinition"></a>创建 deviceManagementConfigurationSimpleSettingCollectionDefinition

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 deviceManagementConfigurationSimpleSettingCollectionDefinition 对象的 JSON 表示形式。

下表显示创建 deviceManagementConfigurationSimpleSettingCollectionDefinition 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|适用性|[deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|有关哪些设备设置适用于从[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的详细信息|
|accessTypes|[deviceManagementConfigurationSettingAccessTypes](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|读取/写入访问模式的设置 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。 可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。|
|keywords|String collection|要搜索上设置的令牌 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|infoUrls|String collection|有关设置详细信息的链接列表，可在 Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)找到|
|occurrence|[deviceManagementConfigurationSettingOccurrence](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|指示设置是否必需。继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|baseUri|String|基本云解决方案提供商路径 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|offsetUri|String|从基本位置偏移 CSP 路径 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|rootDefinitionId|String|根设置定义（如果该设置是子设置）。 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|categoryId|String|指定在 CSP (CSP) 指定的配置服务提供程序中配置设置的区域组。继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|settingUsage|[deviceManagementConfigurationSettingUsage](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|设置类型，例如，配置和合规性 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。 可取值为：`none`、`configuration`。|
|uxBehavior|[deviceManagementConfigurationControlType](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|设置 UX 中的控件类型表示形式 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。 可取值为：`default`、`dropdown`、`smallTextBox`、`largeTextBox`、`toggle`、`multiheaderGrid` 或 `contextPane`。|
|visibility|[deviceManagementConfigurationSettingVisibility](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|将可见性范围设置为 UX 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。 可取值为：`none`、`settingsCatalog`、`template`。|
|id|String|项目的标识符 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|说明|String|项目说明 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|helpText|String|项目的帮助文本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|name|String|项目名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|displayName|String|项目的显示名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|version|String|项目版本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|valueDefinition|[deviceManagementConfigurationSettingValueDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)|此设置的值定义 继承自 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)|
|defaultValue|[deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|此设置的默认设置值 继承自 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)|
|dependentOn|[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) 集合|此设置依赖于父设置列表 继承自 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)|
|dependedOnBy|[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) 集合|依赖于此设置的子设置列表 继承自 [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)|
|maximumCount|Int32|集合中简单设置的最大数目。 有效值为 1 到 100|
|minimumCount|Int32|集合中的最小简单设置数。 有效值为 1 到 100|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 9248

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionDefinition",
  "applicability": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
    "description": "Description value",
    "platform": "macOS",
    "deviceMode": "kiosk",
    "technologies": "mdm"
  },
  "accessTypes": "add",
  "keywords": [
    "Keywords value"
  ],
  "infoUrls": [
    "Info Urls value"
  ],
  "occurrence": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
    "minDeviceOccurrence": 3,
    "maxDeviceOccurrence": 3
  },
  "baseUri": "Base Uri value",
  "offsetUri": "Offset Uri value",
  "rootDefinitionId": "Root Definition Id value",
  "categoryId": "Category Id value",
  "settingUsage": "configuration",
  "uxBehavior": "dropdown",
  "visibility": "settingsCatalog",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value",
  "valueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueDefinition"
  },
  "defaultValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValue",
    "children": [
      {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
        "settingDefinitionId": "Setting Definition Id value",
        "choiceSettingValue": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
          "value": "Value value",
          "children": [
            {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
              "settingDefinitionId": "Setting Definition Id value",
              "choiceSettingValue": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                "value": "Value value",
                "children": [
                  {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                    "settingDefinitionId": "Setting Definition Id value",
                    "choiceSettingValue": {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                      "value": "Value value",
                      "children": [
                        {
                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                          "settingDefinitionId": "Setting Definition Id value",
                          "choiceSettingValue": {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                            "value": "Value value",
                            "children": [
                              {
                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                "settingDefinitionId": "Setting Definition Id value",
                                "choiceSettingValue": {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                  "value": "Value value",
                                  "children": [
                                    {
                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                      "settingDefinitionId": "Setting Definition Id value",
                                      "choiceSettingValue": {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                        "value": "Value value",
                                        "children": [
                                          {
                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                            "settingDefinitionId": "Setting Definition Id value",
                                            "choiceSettingValue": {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                              "value": "Value value",
                                              "children": [
                                                {
                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                  "settingDefinitionId": "Setting Definition Id value",
                                                  "choiceSettingValue": {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                    "value": "Value value",
                                                    "children": [
                                                      {
                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                        "settingDefinitionId": "Setting Definition Id value",
                                                        "choiceSettingValue": {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                          "value": "Value value",
                                                          "children": [
                                                            {
                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                              "settingDefinitionId": "Setting Definition Id value",
                                                              "choiceSettingValue": {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                "value": "Value value",
                                                                "children": [
                                                                  {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                    "settingDefinitionId": "Setting Definition Id value",
                                                                    "choiceSettingValue": {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                      "value": "Value value",
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
      "dependentOn": "Dependent On value",
      "parentSettingId": "Parent Setting Id value"
    }
  ],
  "dependedOnBy": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
      "dependedOnBy": "Depended On By value",
      "required": true
    }
  ],
  "maximumCount": 12,
  "minimumCount": 12
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9297

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionDefinition",
  "applicability": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
    "description": "Description value",
    "platform": "macOS",
    "deviceMode": "kiosk",
    "technologies": "mdm"
  },
  "accessTypes": "add",
  "keywords": [
    "Keywords value"
  ],
  "infoUrls": [
    "Info Urls value"
  ],
  "occurrence": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
    "minDeviceOccurrence": 3,
    "maxDeviceOccurrence": 3
  },
  "baseUri": "Base Uri value",
  "offsetUri": "Offset Uri value",
  "rootDefinitionId": "Root Definition Id value",
  "categoryId": "Category Id value",
  "settingUsage": "configuration",
  "uxBehavior": "dropdown",
  "visibility": "settingsCatalog",
  "id": "cb4abda1-bda1-cb4a-a1bd-4acba1bd4acb",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value",
  "valueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueDefinition"
  },
  "defaultValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValue",
    "children": [
      {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
        "settingDefinitionId": "Setting Definition Id value",
        "choiceSettingValue": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
          "value": "Value value",
          "children": [
            {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
              "settingDefinitionId": "Setting Definition Id value",
              "choiceSettingValue": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                "value": "Value value",
                "children": [
                  {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                    "settingDefinitionId": "Setting Definition Id value",
                    "choiceSettingValue": {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                      "value": "Value value",
                      "children": [
                        {
                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                          "settingDefinitionId": "Setting Definition Id value",
                          "choiceSettingValue": {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                            "value": "Value value",
                            "children": [
                              {
                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                "settingDefinitionId": "Setting Definition Id value",
                                "choiceSettingValue": {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                  "value": "Value value",
                                  "children": [
                                    {
                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                      "settingDefinitionId": "Setting Definition Id value",
                                      "choiceSettingValue": {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                        "value": "Value value",
                                        "children": [
                                          {
                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                            "settingDefinitionId": "Setting Definition Id value",
                                            "choiceSettingValue": {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                              "value": "Value value",
                                              "children": [
                                                {
                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                  "settingDefinitionId": "Setting Definition Id value",
                                                  "choiceSettingValue": {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                    "value": "Value value",
                                                    "children": [
                                                      {
                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                        "settingDefinitionId": "Setting Definition Id value",
                                                        "choiceSettingValue": {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                          "value": "Value value",
                                                          "children": [
                                                            {
                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                              "settingDefinitionId": "Setting Definition Id value",
                                                              "choiceSettingValue": {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                "value": "Value value",
                                                                "children": [
                                                                  {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                    "settingDefinitionId": "Setting Definition Id value",
                                                                    "choiceSettingValue": {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                      "value": "Value value",
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
      "dependentOn": "Dependent On value",
      "parentSettingId": "Parent Setting Id value"
    }
  ],
  "dependedOnBy": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
      "dependedOnBy": "Depended On By value",
      "required": true
    }
  ],
  "maximumCount": 12,
  "minimumCount": 12
}
```




