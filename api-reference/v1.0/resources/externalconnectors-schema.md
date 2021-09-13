---
title: 架构资源类型
description: 连接架构确定添加到连接的内容如何用于各种 Microsoft Graph体验。
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: dcfea02e76c97a8bd946a3c1aa5294b843b0b739
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036583"
---
# <a name="schema-resource-type"></a>架构资源类型

命名空间：microsoft.graph.externalConnectors

连接[架构](externalconnectors-externalconnection.md)确定外部内容如何用于各种 Microsoft Graph体验。 架构是计划添加到连接中的所有属性的简单列表及其属性、标签和别名。 向连接添加项目前，必须注册架构。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[创建架构](../api/externalconnectors-schema-create.md)|[schema](../resources/externalconnectors-schema.md)|创建新的 [架构](../resources/externalconnectors-schema.md) 对象。|
|[获取架构](../api/externalconnectors-schema-get.md)|[schema](../resources/externalconnectors-schema.md)|读取架构对象的属性 [和](../resources/externalconnectors-schema.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|baseType|String|必须设置为 `microsoft.graph.externalConnector.externalItem`。 必需。|
|properties|[property](../resources/externalconnectors-property.md) 集合|为连接中的项目定义的属性。 最小属性数为 1，最大值为 128。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.schema",
  "openType": false
}
-->
``` json
{
  "baseType": "String",
  "properties": [
    {
      "name": "String",
      "type": "String",
    }
  ]
}
```

