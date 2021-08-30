---
title: externalGroup 资源类型
description: 代表非Azure Active Directory组。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5fbfcb8b462b490b33519f04268c505871613a24
ms.sourcegitcommit: 6efd9df497d795988cd85474f379d1989b0995b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697385"
---
# <a name="externalgroup-resource-type"></a>externalGroup 资源类型

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

命名空间：microsoft.graph.externalConnectors

代表非Azure Active Directory组。

外部组确定对外部数据源中内容的权限。 这些外部组可在 externalItem 的 [acl](../resources/externalconnectors-externalitem.md) 上的 [条目中使用](../resources/externalconnectors-externalitem.md)。

外部组的示例包括业务部门和工作组。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[创建 externalGroup](../api/externalconnectors-externalconnection-post-groups.md)|[microsoft.graph.externalConnectors.externalGroup](../resources/externalconnectors-externalgroup.md)|创建新的 **externalGroup** 对象。|
|[删除 externalGroup](../api/externalconnectors-externalgroup-delete.md)|无|删除 **externalGroup** 对象。|
|[创建成员](../api/externalconnectors-externalgroup-post-members.md)|[microsoft.graph.externalConnectors.externalGroupMember](../resources/externalconnectors-externalgroupmember.md)|创建新的 **externalGroupMember** 对象。|

## <a name="properties"></a>属性

| 属性    | 类型   | 说明                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | String | 连接内外部组的唯一 ID。 它必须是字母数字，并且最多为 128 个字符。 |
| displayName | String | 外部组的友好名称。 可选。                                                                       |
| description | String | 外部组的说明。 可选。                                                                         

## <a name="relationships"></a>关系

| 关系 | 类型                                                                  | 说明                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| 成员      | [microsoft.graph.externalConnectors.externalGroupMember](../resources/externalconnectors-externalgroupmember.md) 集合 | 添加到 **externalGroup 的成员**。 可以将用户Azure Active Directory组Azure Active Directory其他 **externalGroups 添加** 为成员。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalGroup",
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
