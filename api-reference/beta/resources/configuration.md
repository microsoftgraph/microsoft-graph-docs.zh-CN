---
title: 配置资源类型
description: 指定允许管理 externalConnection 和索引 externalConnection 中的内容的其他应用程序 Id。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bd267c77a9904564e8b2b7f592f207204d9396b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994216"
---
# <a name="configuration-resource-type"></a>配置资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定允许管理 externalConnection 和索引 [externalConnection](../resources/externalconnection.md)中的内容的其他应用程序 id。

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


