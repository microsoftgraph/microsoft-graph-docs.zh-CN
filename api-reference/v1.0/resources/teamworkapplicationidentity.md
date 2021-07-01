---
title: teamworkApplicationIdentity 资源类型
description: 表示应用程序中Microsoft Teams。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 67e1ed4365febae44032c09d94656d2e3ac0b504
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211082"
---
# <a name="teamworkapplicationidentity-resource-type"></a>teamworkApplicationIdentity 资源类型

命名空间：microsoft.graph

表示 **应用程序中** Microsoft Teams。 `teamworkApplicationIdentity` 用于表示消息中的自动程序@mentioned传出 webhook。


继承自 [标识](../resources/identity.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|applicationIdentityType|teamworkApplicationIdentityType| 引用的应用程序的类型。 可能的值是 `aadApplication` `bot` `tenantBot` ：、、、、 `office365Connector` `outgoingWebhook` 和 `unknownFutureValue` 。|
|displayName|String|继承自 [标识](../resources/identity.md)。 应用程序的显示名称。 可选。|
|id|String|继承自 [标识](../resources/identity.md)。 应用程序的 ID。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkApplicationIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkApplicationIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "applicationIdentityType": "String"
}
```

