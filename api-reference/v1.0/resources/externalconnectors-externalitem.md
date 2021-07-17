---
title: externalItem 资源类型
description: 添加到 Microsoft Graph项。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6c9fc66f33c2dc089bbdffe3987959d56670332a
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467254"
---
# <a name="externalitem-resource-type"></a>externalItem 资源类型

命名空间：microsoft.graph.externalConnectors

添加到 Microsoft Graph[项](externalconnectors-externalconnection.md)。 

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[创建 externalItem](../api/externalconnectors-externalitem-create.md)|[externalItem](../resources/externalconnectors-externalitem.md)|创建新的 [externalItem](../resources/externalconnectors-externalitem.md) 对象。|
|[获取 externalItem](../api/externalconnectors-externalitem-get.md)|[externalItem](../resources/externalconnectors-externalitem.md)|读取 [externalItem 对象的属性和](../resources/externalconnectors-externalitem.md) 关系。|
|[更新 externalItem](../api/externalconnectors-externalitem-update.md)|[externalItem](../resources/externalconnectors-externalitem.md)|更新 [externalItem 对象](../resources/externalconnectors-externalitem.md) 的属性。|
|[删除 externalItem](../api/externalconnectors-externalitem-delete.md)|无|删除 [externalItem](../resources/externalconnectors-externalitem.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|acl|[microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md) 集合|访问控制项数组。 每个条目指定授予用户或组的访问权限。 必需项。|
|content|[microsoft.graph.externalConnectors.externalItemContent](../resources/externalconnectors-externalitemcontent.md)|项目内容的纯文本表示形式。 此属性中的文本已编制全文索引。 可选。|
|id|String|开发人员提供的项目在包含[externalConnection 中的唯一 ID。](externalconnectors-externalconnection.md) 必须为字母数字，最多为 128 个字符。 必需项。|
|properties|[microsoft.graph.externalConnectors.properties](../resources/externalconnectors-properties.md)|具有项目属性的属性包。 属性必须符合为[externalConnection](externalconnectors-externalconnection.md)定义的架构。 [](externalconnectors-schema.md) 必填。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalItem",
  "openType": false
}
-->
```json
{
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant"
    }
  ],
  "id": "String (identifier)",
  "properties": {
    "@odata.type": "microsoft.graph.externalConnectors.properties"
  },
  "content": {
    "@odata.type": "microsoft.graph.externalConnectors.externalItemContent"
  }
}
```

