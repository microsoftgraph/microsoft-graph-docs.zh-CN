---
title: teamworkApplicationIdentity 资源类型
description: 表示应用程序中Microsoft Teams。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: af3f0205bf53137791414c2e4777877220ed6ca5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113523"
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

