---
title: androidManagedStoreAppConfigurationSchema 资源类型
description: 描述 Android 应用程序的自定义配置的架构。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a4dde22a1f2a59827639059269f566235bbf5fcb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702668"
---
# <a name="androidmanagedstoreappconfigurationschema-resource-type"></a>androidManagedStoreAppConfigurationSchema 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述 Android 应用程序的自定义配置的架构。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 androidManagedStoreAppConfigurationSchemas](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-list.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) 集合|列出 [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) 对象的属性和关系。|
|[获取 androidManagedStoreAppConfigurationSchema](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-get.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|读取 [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) 对象的属性和关系。|
|[创建 androidManagedStoreAppConfigurationSchema](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-create.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|创建新的 [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) 对象。|
|[删除 androidManagedStoreAppConfigurationSchema](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-delete.md)|无|删除 [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)。|
|[更新 androidManagedStoreAppConfigurationSchema](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-update.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|更新 [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|架构对应的应用程序的 Android 包名称的实体密钥|
|exampleJson|Binary|包含符合此架构的示例 JSON 字符串的 UTF8 编码的字节数组，它演示如何设置此应用的配置|
|schemaItems|[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) 集合|项集合，每个项表示架构中的命名配置选项。 它仅包含根级别的配置。|
|nestedSchemaItems|[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) 集合|项集合，每个项表示架构中的命名配置选项。 它包含所有配置的简单列表。|

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
      "index": 1024,
      "parentIndex": 1024,
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
  ],
  "nestedSchemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "index": 1024,
      "parentIndex": 1024,
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





