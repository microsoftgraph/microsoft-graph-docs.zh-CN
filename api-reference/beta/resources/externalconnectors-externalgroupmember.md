---
title: externalGroupMember 资源类型
description: 表示 externalGroup 的成员，用于设置对添加到 Microsoft Graph 的外部内容的权限。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e3626c718360982bf79cb9757a13e4b4c01669cd
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467639"
---
# <a name="externalgroupmember-resource-type"></a>externalGroupMember 资源类型

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示[externalGroup](externalconnectors-externalgroup.md)的成员，用于设置对添加到 Microsoft Graph 的外部内容的权限。

## <a name="methods"></a>方法

| 方法                                                              | 返回类型         | 说明                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [创建 externalGroupMember](../api/externalconnectors-externalgroup-post-members.md) | [externalGroupMember](../resources/externalconnectors-externalgroupmember.md) | 创建新的 **externalGroupMember** 对象。 |
| [删除 externalGroupMember](../api/externalconnectors-externalgroupmember-delete.md)  | 无                | 删除 **externalGroupMember** 对象。   |

## <a name="properties"></a>属性

| 属性       | 类型                    | 说明                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| id             | String                  | 成员的唯一 ID。 对于用户或组，它将是 objectId Azure Active Directory组，对于外部组，为 **externalGroup** 的 **id** 属性。                                    |
| type           | microsoft.graph.externalConnectors.externalGroupMemberType | 添加到外部组的成员的类型。 可能的值是： `user` 或 `group` 当 **identitySource** 为 时，或者 `azureActiveDirectory` 当 `group` **identitySource** 为 `external` 时。 |
| identitySource | microsoft.graph.externalConnectors.identitySourceType      | 成员所属的标识源。 可取值为：`azureActiveDirectory`、`external`。                                                                                         |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalGroupMember",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "type": "String",
  "identitySource": "String"
}
```
