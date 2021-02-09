---
title: externalGroupMember 资源类型
description: 表示用于设置对添加到 Microsoft Graph 的外部内容的权限的外部组的成员。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1e86fb275b941b7a3033999fedd4c71aa3ac1de1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161689"
---
# <a name="externalgroupmember-resource-type"></a>externalGroupMember 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用于设置 [对](externalgroup.md) 添加到 Microsoft Graph 的外部内容的权限的外部组的成员。

## <a name="methods"></a>方法

| 方法                                                              | 返回类型         | 说明                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [创建 externalGroupMember](../api/externalgroup-post-members.md) | externalGroupMember | 创建新的 **externalGroupMember** 对象。 |
| [删除 externalGroupMember](../api/externalgroupmember-delete.md)  | 无                | 删除 **externalGroupMember** 对象。   |

## <a name="properties"></a>属性

| 属性       | 类型                    | 说明                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| id             | String                  | 成员的唯一 ID。 对于 Azure Active Directory 用户或组，它将是 objectId，对于外部组，为 **externalGroup** 的 **id** 属性。                                    |
| type           | externalGroupMemberType | 添加到外部组的成员的类型。 可能的值是： `user` 或 `group` 当 **identitySource** 是时，或者 `azureActiveDirectory` 当 `group` **identitySource** 为时 `external` 。 |
| identitySource | identitySourceType      | 成员所属的标识源。 可取值为：`azureActiveDirectory`、`external`。                                                                                         |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroupMember",
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
