---
title: teamworkUserIdentity 资源类型
description: 表示用户Microsoft Teams。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b0c50856a2b7051a631cd14ab3985cd8724bfe4c
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211306"
---
# <a name="teamworkuseridentity-resource-type"></a>teamworkUserIdentity 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 **用户Microsoft Teams。**


继承自 [标识](../resources/identity.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|继承自 [标识](../resources/identity.md)。 用户的显示名称。 可选。|
|id|String|继承自 [标识](../resources/identity.md)。 用户的 ID。 |
|userIdentityType|teamworkUserIdentityType| 用户类型。 可能的值是 `aadUser` `onPremiseAadUser` `anonymousGuest` ：、、、、、、 `federatedUser` `personalMicrosoftAccountUser` 和 `skypeUser` `phoneUser` 。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkUserIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkUserIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "userIdentityType": "String"
}
```

