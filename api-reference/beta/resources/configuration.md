---
title: 配置资源类型
description: 指定允许管理 externalConnection 和索引 externalConnection 中的内容的其他应用程序 Id。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 080a966ae9435c189a34155d108e1c48235ffb07
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938889"
---
# <a name="configuration-resource-type"></a>配置资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定允许管理 externalConnection 和索引[externalConnection](../resources/externalconnection.md)中的内容的其他应用程序 id。

## <a name="properties"></a>属性

| 属性       | 类型              | 描述 |
|:---------------|:------------------|:------------|
| authorizedApps | String collection | 允许管理 externalConnection 和索引 externalConnection 中的内容的注册的 Azure Active Directory 应用程序的应用程序 Id 的集合。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.configuration",
  "baseType": null
}-->

```json
{
  "authorizedApps": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "configuration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
