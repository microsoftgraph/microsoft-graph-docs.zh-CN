---
title: teamworkUserIdentity 资源类型
description: 表示用户Microsoft Teams。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 107ff351d17cf999fa0d2dce085587f5b2ea16edd6bf5315ded551fe78554629
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146382"
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

