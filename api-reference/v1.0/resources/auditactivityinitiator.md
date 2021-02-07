---
title: auditActivityInitiator 资源类型
description: 标识启动活动的资源对象。 发起人可以是用户、应用或系统 (被视为应用) 。
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: fbc2fd2f6c93cac583fc1ec28375d8538d35b447
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135756"
---
# <a name="auditactivityinitiator-resource-type"></a>auditActivityInitiator 资源类型

命名空间：microsoft.graph

标识启动活动的资源对象。 发起人可以是用户、应用或系统 (被视为应用) 。

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|应用|[appIdentity](appidentity.md)|如果启动活动的资源是应用，则此属性指示 appId、Name、servicePrincipalId、Name 等所有应用相关信息。|
|user|[userIdentity](useridentity.md)|如果启动活动的资源是用户，则此属性指示与用户 Id、名称、UserPrinicpalName 等所有用户相关信息。|

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

