---
title: auditActivityInitiator 资源类型
description: '标识启动活动的资源对象。 发起方可以是用户、应用程序或系统 (，它被视为应用程序) '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: SarahBar
ms.openlocfilehash: 49c60dc42cb84d047f36904b2af11fe5c8d3bd8e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812546"
---
# <a name="auditactivityinitiator-resource-type"></a>auditActivityInitiator 资源类型

命名空间： microsoft. graph 标识启动活动的资源对象。 发起方可以是用户、应用程序或系统 (，它被视为应用程序) 



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|应用程序|[appIdentity](appidentity.md)|如果启动活动的资源是一个应用程序，则此属性指示所有与应用程序相关的信息，如 appId、Name、servicePrincipalId、Name。|
|user|[userIdentity](useridentity.md)|如果启动活动的资源是用户，则此属性指示与用户相关的所有信息，如 userId、Name、UserPrinicpalName。|

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
