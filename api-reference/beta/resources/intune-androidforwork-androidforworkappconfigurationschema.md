---
title: androidForWorkAppConfigurationSchema 资源类型
description: 描述 Android for Work 应用程序的自定义配置的架构。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c8278aca6c91675658d0e3939a4acef525d3f017
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806276"
---
# <a name="androidforworkappconfigurationschema-resource-type"></a>androidForWorkAppConfigurationSchema 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述 Android for Work 应用程序的自定义配置的架构。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 androidForWorkAppConfigurationSchemas](../api/intune-androidforwork-androidforworkappconfigurationschema-list.md)|[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 集合|列出 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的属性和关系。|
|[获取 androidForWorkAppConfigurationSchema](../api/intune-androidforwork-androidforworkappconfigurationschema-get.md)|[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|读取 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的属性和关系。|
|[创建 androidForWorkAppConfigurationSchema](../api/intune-androidforwork-androidforworkappconfigurationschema-create.md)|[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|创建新的 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象。|
|[删除 androidForWorkAppConfigurationSchema](../api/intune-androidforwork-androidforworkappconfigurationschema-delete.md)|无|删除 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)。|
|[更新 androidForWorkAppConfigurationSchema](../api/intune-androidforwork-androidforworkappconfigurationschema-update.md)|[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|更新 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|架构对应的应用程序的 Android 包名称的实体密钥|
|exampleJson|Binary|包含符合此架构的示例 JSON 字符串的 UTF8 编码的字节数组，它演示如何设置此应用的配置|
|schemaItems|[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) 集合|项集合，每个项表示架构中命名的配置选项|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchema"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "String (identifier)",
  "exampleJson": "binary",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
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



