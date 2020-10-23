---
title: 创建 deviceManagementCollectionSettingDefinition
description: 创建新的 deviceManagementCollectionSettingDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cefd92913ddb79ee8de42d2524db992b8ecb64c5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735580"
---
# <a name="create-devicemanagementcollectionsettingdefinition"></a>创建 deviceManagementCollectionSettingDefinition

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
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
POST /deviceManagement/settingDefinitions
POST /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 deviceManagementCollectionSettingDefinition 对象的 JSON 表示形式。

下表显示创建 deviceManagementCollectionSettingDefinition 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的设置定义的 ID|
|valueType|[deviceManangementIntentValueType](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的值的数据类型。 可取值为：`integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。|
|displayName|String|设置的显示名称继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|isTopLevel|布尔|如果设置是顶级的，则可以对其进行配置，而无需将其包装在从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的集合或复杂设置中。|
|说明|String|该设置的说明继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|placeholderText|String|占位符文本作为从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的有效输入的示例|
|documentationUrl|String|设置从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的文档的 Url|
|headerTitle|String|设置标头的标题代表从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的设置/设置的类别/部分|
|headerSubtitle|String|设置标头的副标题有关从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的类别/部分的更多详细信息|
|keywords|String collection|与继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的设置关联的关键字|
|施加|[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) 集合|继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的设置值的约束集合|
|依|[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) 集合|继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的其他设置的依赖项集合|
|elementDefinitionId|String|描述集合的每个元素外观的设置定义 ID|



## <a name="response"></a>响应
如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
Content-type: application/json
Content-length: 1081

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "placeholderText": "Placeholder Text value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "headerTitle": "Header Title value",
  "headerSubtitle": "Header Subtitle value",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "Supported Types value"
      ]
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
          "supportedTypes": [
            "Supported Types value"
          ]
        }
      ]
    }
  ],
  "elementDefinitionId": "Element Definition Id value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1130

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
  "id": "0419c4a7-c4a7-0419-a7c4-1904a7c41904",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "placeholderText": "Placeholder Text value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "headerTitle": "Header Title value",
  "headerSubtitle": "Header Subtitle value",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "Supported Types value"
      ]
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
          "supportedTypes": [
            "Supported Types value"
          ]
        }
      ]
    }
  ],
  "elementDefinitionId": "Element Definition Id value"
}
```





