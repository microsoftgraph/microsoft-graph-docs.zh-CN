---
title: externalGroup 资源类型
description: 表示一个外部组，用于设置对添加到 Microsoft Graph 连接的外部项目的权限。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 2e9d8e3a605f1c3df39b13607f82e7541d59e62e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161700"
---
# <a name="externalgroup-resource-type"></a>externalGroup 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示外部组。 外部组 (Azure Active Directory 用户和组) 用于设置对添加到 Microsoft Graph 连接 **的外部** 项目的权限。 使用 **externalGroups** 表示非 Azure Active Directory 组或类似组 (例如) 上的业务单位、Teams 和子级，这些构造可确定对外部数据源中内容的权限。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[创建 externalGroup](../api/externalconnection-post-groups.md)|[externalGroup](../resources/externalgroup.md)|创建新的 **externalGroup** 对象。|
|[删除 externalGroup](../api/externalgroup-delete.md)|无|删除 **externalGroup** 对象。|
|[创建成员](../api/externalgroup-post-members.md)|[externalGroupMember](../resources/externalgroupmember.md)|创建新的 **externalGroupMember** 对象。|

## <a name="properties"></a>属性

| 属性    | 类型   | 说明                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | String | 连接内外部组的唯一 ID。 它必须是字母数字，并且最多为 128 个字符。 |
| displayName | String | 外部组的友好名称。 可选。                                                                       |
| 说明 | String | 外部组的说明。 可选。                                                                         

## <a name="relationships"></a>关系

| 关系 | 类型                                                                  | 说明                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| 成员      | [externalGroupMember](../resources/externalgroupmember.md) 集合 | 添加到 **externalGroup 的成员**。 可以将 Azure Active Directory 用户、Azure Active Directory 组或其他 **外部组** 添加为成员。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroup",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```
