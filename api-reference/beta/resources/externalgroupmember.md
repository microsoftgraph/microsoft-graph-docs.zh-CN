---
title: externalGroupMember 资源类型
description: 表示用于对添加到 Microsoft Graph 的外部内容设置权限的 externalGroup 的成员。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 19b5c5094501215cc3ffd3e852ba6ca427807988
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193824"
---
# <a name="externalgroupmember-resource-type"></a>externalGroupMember 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用于对添加到 Microsoft Graph 的外部内容设置权限的 [externalGroup](externalgroup.md) 的成员。

## <a name="methods"></a>方法

| 方法                                                              | 返回类型         | 说明                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [创建 externalGroupMember](../api/externalgroup-post-members.md) | externalGroupMember | 创建新的 **externalGroupMember** 对象。 |
| [删除 externalGroupMember](../api/externalgroupmember-delete.md)  | 无                | 删除 **externalGroupMember** 对象。   |

## <a name="properties"></a>属性

| 属性       | 类型                    | 说明                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| id             | 字符串                  | 成员的唯一 ID。 当 Azure Active Directory 用户或组以及外部组的 **id** 属性为 **externalGroup** 时，它就是相应的 objectId。                                    |
| type           | externalGroupMemberType | 添加到外部组的成员类型。 可能的值为： `user` 或者 `group` 当 **identitySource** 是 `azureActiveDirectory` `group` **identitySource** 时， `external` 则为。 |
| identitySource | identitySourceType      | 成员所属的标识源。 可取值为：`azureActiveDirectory`、`external`。                                                                                         |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroupMember",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "String (identifier)",
  "type": "String",
  "identitySource": "String"
}
```
