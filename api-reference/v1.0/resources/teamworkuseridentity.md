---
title: teamworkUserIdentity 资源类型
description: 表示Microsoft Teams中的用户。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 86b827be0a7d947a627f41f97b4002b7406006ca
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917610"
---
# <a name="teamworkuseridentity-resource-type"></a>teamworkUserIdentity 资源类型

命名空间：microsoft.graph

表示Microsoft Teams中的 **用户**。


继承自 [标识](../resources/identity.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|继承自 [标识](../resources/identity.md)。 用户的显示名称。 可选。|
|id|字符串|继承自 [标识](../resources/identity.md)。 用户的 ID。 |
|userIdentityType|teamworkUserIdentityType| 用户类型。 可能的值为：`aadUser`、、`onPremiseAadUser``anonymousGuest`、`federatedUser`、`personalMicrosoftAccountUser`、`phoneUser``skypeUser`和 `unknownFutureValue` `emailUser`。|

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

