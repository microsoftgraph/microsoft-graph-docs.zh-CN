---
title: externalGroup 资源类型
description: 表示一个外部组，用于对添加到 Microsoft Graph外部项目设置权限。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3f0c6adbd47d1823b82e19d3fb9a352e26391da9
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467643"
---
# <a name="externalgroup-resource-type"></a>externalGroup 资源类型

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示外部组。 外部 (组Azure Active Directory用户和组) 用于设置对添加到 Microsoft Graph 连接的外部项的权限。  使用 **externalGroups** 表示非 Azure Active Directory 组或类似组的构造 (如) 上的业务单位、Teams 和 son，这些构造可确定对外部数据源中内容的权限。

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
| 说明 | String | 外部组的说明。 可选。                                                                         

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
