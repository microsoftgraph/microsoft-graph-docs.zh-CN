---
title: securityResource 资源类型
description: 代表与警报相关的资源。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: ce0398ba134f7537420a99ccaed84f2ff209f883
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682262"
---
# <a name="securityresource-resource-type"></a>securityResource 资源类型

命名空间：microsoft.graph

代表与警报相关的资源。

## <a name="properties"></a>属性

| 属性   | 类型|Description|
|:---------------|:--------|:----------|
|资源|String|与当前警报相关的资源的名称。 **** 必需。|
|resourceType|[securityResourceType](#securityresourcetype-values)|表示与警报相关的安全资源的类型。 可取值为：`attacked`、`related`。|

### <a name="securityresourcetype-values"></a>securityResourceType 值

|成员|值|说明|
|-|-|-|
|遭受|1 |警报中的资源受到攻击。|
|关联方|双面|该资源与警报相关，但不直接受到攻击。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.securityResource"
}-->

```json
{
  "resource": "String",
  "resourceType": "@odata.type: microsoft.graph.securityResourceType"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
