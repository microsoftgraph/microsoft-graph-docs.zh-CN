---
title: externalGroup 资源类型
description: 代表在添加到 Microsoft Graph 连接的 externalItems 上用于设置权限的外部组。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c258df9e6f20cf7a19e291fd298ad66345a72949
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193825"
---
# <a name="externalgroup-resource-type"></a>externalGroup 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表一个外部组。 外部组 (以及 Azure Active Directory users 和 groups) 用于在添加到 Microsoft Graph 连接的 **externalItems** 上设置权限。 使用 **externalGroups** 表示非 Azure Active Directory 组或类似组的构造 (例如，) 上的业务单位、团队和子儿子确定对外部数据源中内容的权限。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[创建 externalGroup](../api/externalconnection-post-groups.md)|[externalGroup](../resources/externalgroup.md)|创建新的 **externalGroup** 对象。|
|[删除 externalGroup](../api/externalgroup-delete.md)|无|删除 **externalGroup** 对象。|
|[创建成员](../api/externalgroup-post-members.md)|[externalGroupMember](../resources/externalgroupmember.md)|创建新的 **externalGroupMember** 对象。|

## <a name="properties"></a>属性

| 属性    | 类型   | 说明                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | 字符串 | 连接中的外部组的唯一 ID。 它必须是字母数字，最长可为128个字符。 |
| displayName | 字符串 | 外部组的友好名称。 可选。                                                                       |
| 说明 | 字符串 | 外部组的说明。 可选。                                                                         

## <a name="relationships"></a>关系

| 关系 | 类型                                                                  | 说明                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| 成员      | [externalGroupMember](../resources/externalgroupmember.md) 集合 | 添加到 **externalGroup**中的成员。 你可以将 Azure Active Directory 用户、Azure Active Directory 组或其他 **externalGroups** 添加为成员。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroup",
  "baseType": "",
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
