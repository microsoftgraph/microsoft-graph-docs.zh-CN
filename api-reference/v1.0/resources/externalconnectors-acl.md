---
title: acl 资源类型
description: 由 externalConnection 索引的项的访问控制Microsoft 搜索项。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 56fa0c8f47f9bec9e2c00cbff3423a8aed541a2709c117326d3d0a29effabc08
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141691"
---
# <a name="acl-resource-type"></a>acl 资源类型

命名空间：microsoft.graph.externalConnectors

由 externalConnection 索引的项的访问控制Microsoft 搜索项。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|accessType|microsoft.graph.externalConnectors.accessType|授予标识的访问权限。 可取值为：`grant`、`deny`、`unknownFutureValue`。|
|type|microsoft.graph.externalConnectors.aclType|标识的类型。 可取值为：`user`、`group`、`everyone`、`everyoneExceptGuests`、`externalGroup`、`unknownFutureValue`。|
|value|String|标识的唯一标识。 如果Azure Active Directory，则分别设置为类型为 user、group 和 everyone (和 everyoneExceptGuests 的用户、组或租户) `value` 标识符。 如果外部组设置为 `value` externalGroup 的 ID |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.acl"
}
-->
``` json
{
  "type": "String",
  "value": "String",
  "accessType": "String"
}
```

