---
title: externalGroup 资源类型
description: 代表非Azure Active Directory组。
author: sacampbe-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: ad3718fec3a255348fc808ac7a87df96bbe8f4ec
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123473"
---
# <a name="externalgroup-resource-type"></a>externalGroup 资源类型

命名空间：microsoft.graph.externalConnectors

代表非Azure Active Directory组。

外部组确定对外部数据源中内容的权限。 这些外部组可在 externalItem 的 [acl](../resources/externalconnectors-externalitem.md) 上的 [条目中使用](../resources/externalconnectors-externalitem.md)。

外部组的示例包括业务部门和工作组。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[创建 externalGroup](../api/externalconnectors-externalconnection-post-groups.md)|[microsoft.graph.externalConnectors.externalGroup](../resources/externalconnectors-externalgroup.md)|创建新的 **externalGroup** 对象。|
|[获取 externalGroup](../api/externalconnectors-externalgroup-get.md)|[microsoft.graph.externalConnectors.externalGroup](../resources/externalconnectors-externalgroup.md)|获取 **externalGroup** 对象。|
|[更新 externalGroup](../api/externalconnectors-externalgroup-update.md)|[microsoft.graph.externalConnectors.externalGroup](../resources/externalconnectors-externalgroup.md)|更新 **externalGroup 对象** 的属性。|
|[删除 externalGroup](../api/externalconnectors-externalgroup-delete.md)|无|删除 **externalGroup** 对象。|

## <a name="properties"></a>属性

| 属性    | 类型   | 说明                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | String | 连接内外部组的唯一 ID。 它必须是字母数字，并且最多为 128 个字符。 |
| displayName | String | 外部组的友好名称。 可选。                                                                       |
| 说明 | String | 外部组的说明。 可选。        

## <a name="relationships"></a>关系

| 关系 | 类型                                                                  | 说明                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| 成员      | [microsoft.graph.externalConnectors.identity](../resources/externalconnectors-identity.md) 集合 | 添加到 **externalGroup 的成员**。 可以将用户Azure Active Directory组Azure Active Directory外部 **组** 添加为成员。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```
