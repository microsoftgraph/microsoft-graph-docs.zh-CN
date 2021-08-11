---
title: securityResource 资源类型
description: 表示与警报相关的资源。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 49eb0b1fae46653e9cf538339b3b4b412a8d8f80674702b0151efec5c03a60a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152234"
---
# <a name="securityresource-resource-type"></a>securityResource 资源类型

命名空间：microsoft.graph

表示与警报相关的资源。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|资源|String|与当前警报相关的资源的名称。 **必需**。|
|resourceType|[securityResourceType](#securityresourcetype-values)|表示与警报相关的安全资源类型。 可取值为：`attacked`、`related`。|

### <a name="securityresourcetype-values"></a>securityResourceType 值

|成员|值|说明|
|-|-|-|
|attacked|1|资源在警报中受到攻击。|
|related|2|资源与警报相关，但并未受到直接攻击。|

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

