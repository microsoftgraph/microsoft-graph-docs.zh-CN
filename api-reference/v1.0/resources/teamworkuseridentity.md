---
title: teamworkUserIdentity 资源类型
description: 表示用户Microsoft Teams。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d6989f7b3c5689fefe8e9516e25fd6ff3777fe16
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128156"
---
# <a name="teamworkuseridentity-resource-type"></a>teamworkUserIdentity 资源类型

命名空间：microsoft.graph

表示 **用户Microsoft Teams。**


继承自 [标识](../resources/identity.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|继承自 [标识](../resources/identity.md)。 用户的显示名称。 可选。|
|id|String|继承自 [标识](../resources/identity.md)。 用户的 ID。 |
|userIdentityType|teamworkUserIdentityType| 用户类型。 可能的值是 `aadUser` `onPremiseAadUser` `anonymousGuest` ：、、、、、、、 `federatedUser` `personalMicrosoftAccountUser` `skypeUser` 和 `phoneUser` `unknownFutureValue` 。|

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

