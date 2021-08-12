---
title: provisionedIdentity 资源类型
description: 描述与设置对象摘要事件关联的标识。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 89ba5791235810529e7cc3b2b3c4e1d817920148790f7f9934edb20432420215
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251834"
---
# <a name="provisionedidentity-resource-type"></a>provisionedIdentity 资源类型

命名空间：microsoft.graph


描述与设置对象摘要事件关联的标识。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|详细信息|[detailsInfo](detailsinfo.md)|标识的详细信息。|
|displayName|String|标识的显示名称。 |
|id|String|唯一标识标识。|
|identityType|String|已预配的标识类型，例如"user"或"group"。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedIdentity",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String",
  "identityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


