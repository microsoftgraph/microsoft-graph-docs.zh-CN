---
title: 配置资源类型
description: 指定允许管理 externalConnection 和索引 externalConnection 中的内容的其他应用程序 Id。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c7808d014ee2ab19fda9eceb6064375cf5904d52
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704148"
---
# <a name="configuration-resource-type"></a>配置资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定允许管理 externalConnection 和索引[externalConnection](../resources/externalconnection.md)中的内容的其他应用程序 id。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>属性

| 属性       | 类型              | 说明 |
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
