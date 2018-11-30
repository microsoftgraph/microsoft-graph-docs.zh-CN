---
title: auditActivityInitiator 资源类型
description: 标识启动活动的资源对象。 发起人可以是用户、 应用程序或系统 （它被认为是作为应用程序）
ms.openlocfilehash: 834b39f67a9a3a251c61f15d3b1fa8aa964870e9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046199"
---
# <a name="auditactivityinitiator-resource-type"></a>auditActivityInitiator 资源类型
标识启动活动的资源对象。 发起人可以是用户、 应用程序或系统 （它被认为是作为应用程序）



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|应用程序|[appIdentity](appidentity.md)|如果启动活动资源是应用程序，此属性指示所有应用程序相关信息，appId，如姓名、 servicePrincipalId，名称。|
|user|[userIdentity](useridentity.md)|如果启动了此活动的资源是用户，此属性指示所有用户相关的用户 Id，名称、 UserPrinicpalName 类似的信息。|

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