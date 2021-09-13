---
title: acl 资源类型
description: 由 externalConnection 索引的项的访问控制Microsoft 搜索项。
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 523ce420b4796d6ca3032839bf28393ea4975d21
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123487"
---
# <a name="acl-resource-type"></a>acl 资源类型

命名空间：microsoft.graph.externalConnectors

由 externalConnection 索引的项的访问控制Microsoft 搜索项。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|accessType|microsoft.graph.externalConnectors.accessType|授予标识的访问权限。 可取值为：`grant`、`deny`、`unknownFutureValue`。|
|type|microsoft.graph.externalConnectors.aclType|标识的类型。 可取值为：`user`、`group`、`everyone`、`everyoneExceptGuests`、`externalGroup`、`unknownFutureValue`。|
|value|String|标识的唯一标识。 如果Azure Active Directory，则分别设置为 user、group 和 everyone (和 everyoneExceptGuests 类型的用户、组或租户 `value`) 标识符。 如果外部组设置为 `value` externalGroup 的 ID |

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

