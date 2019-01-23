---
title: androidManagedStoreAppConfigurationSchema 资源类型
description: 描述 Android 应用程序的自定义配置的模式。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9e520957ddcdba6c713b5564fdf1a85ce6ad8b08
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414947"
---
# <a name="androidmanagedstoreappconfigurationschema-resource-type"></a>androidManagedStoreAppConfigurationSchema 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述 Android 应用程序的自定义配置的模式。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 androidManagedStoreAppConfigurationSchemas](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-list.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)集合|列出属性和[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象之间的关系。|
|[获取 androidManagedStoreAppConfigurationSchema](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-get.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|读取属性和[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象的关系。|
|[创建 androidManagedStoreAppConfigurationSchema](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-create.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|创建新的[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象。|
|[删除 androidManagedStoreAppConfigurationSchema](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-delete.md)|无|删除[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)。|
|[更新 androidManagedStoreAppConfigurationSchema](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-update.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|更新[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|架构对应的应用程序的 Android 包名称的实体密钥|
|exampleJson|Binary|包含符合此架构的示例 JSON 字符串的 UTF8 编码的字节数组，它演示如何设置此应用的配置|
|schemaItems|[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)集合|项集合，每个项表示架构中命名的配置选项|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchema"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "id": "String (identifier)",
  "exampleJson": "binary",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "schemaItemKey": "String",
      "displayName": "String",
      "description": "String",
      "defaultBoolValue": true,
      "defaultIntValue": 1024,
      "defaultStringValue": "String",
      "defaultStringArrayValue": [
        "String"
      ],
      "dataType": "String",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "String",
          "value": "String"
        }
      ]
    }
  ]
}
```




