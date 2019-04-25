---
title: auditActivityInitiator 资源类型
description: 标识启动活动的资源对象。 发起方可以是用户、应用程序或系统 (被视为应用程序)
localization_priority: Normal
ms.openlocfilehash: 14c92a4df42c3d8dbcd6836695df8d6caac3cf87
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543766"
---
# <a name="auditactivityinitiator-resource-type"></a>auditActivityInitiator 资源类型
标识启动活动的资源对象。 发起方可以是用户、应用程序或系统 (被视为应用程序)



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|应用程序|[appIdentity](appidentity.md)|如果启动活动的资源是一个应用程序, 则此属性指示所有与应用程序相关的信息, 如 appId、Name、servicePrincipalId、Name。|
|user|[userIdentity](useridentity.md)|如果启动活动的资源是用户, 则此属性指示与用户相关的所有信息, 如 userId、Name、UserPrinicpalName。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.auditActivityInitiator"
}-->

```json
{
  "app": {"@odata.type": "microsoft.graph.appIdentity"},
  "user": {"@odata.type": "microsoft.graph.userIdentity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditActivityInitiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
