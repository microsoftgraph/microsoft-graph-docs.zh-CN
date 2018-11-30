---
title: androidForWorkAppConfigurationSchema 资源类型
description: 描述 Android for Work 应用程序的自定义配置的架构。
ms.openlocfilehash: f555c7e1b9c62024531f4c4fc57a3fd3df3336fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042106"
---
# <a name="androidforworkappconfigurationschema-resource-type"></a>androidForWorkAppConfigurationSchema 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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





