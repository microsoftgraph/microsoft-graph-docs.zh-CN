---
title: auditActivityInitiator 资源类型
description: '标识启动活动的资源对象。 发起者可以是用户、应用或系统 (被视为应用) '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: besiler
ms.openlocfilehash: e681f56f3caf0792241a92ce5137ac8468b623d8
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647160"
---
# <a name="auditactivityinitiator-resource-type"></a>auditActivityInitiator 资源类型

命名空间：microsoft.graph 标识启动活动的资源对象。 发起者可以是用户、应用或系统 (被视为应用) 



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|应用|[appIdentity](appidentity.md)|如果启动活动的人是应用，则此属性指示其所有标识信息，包括 appId、displayName、servicePrincipalId 和 servicePrincipalName。|
|用户|[auditUserIdentity](auditUserIdentity.md)|如果发起活动的人是用户，则此属性指示其标识信息，包括其 id、displayName 和 userPrincipalName。|

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


