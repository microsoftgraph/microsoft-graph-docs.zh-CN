---
title: 配置资源类型
description: 指定允许管理 externalConnection 和为 externalConnection 中的内容编制索引的附加应用程序 ID。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8a82c5e9e4cbd915d5a7e11b9e162bc510628ecf
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366775"
---
# <a name="configuration-resource-type"></a>配置资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定允许管理 externalConnection 和为 externalConnection 中的内容编制索引的附加[应用程序 ID。](../resources/externalconnection.md)

## <a name="properties"></a>属性

| 属性       | 类型              | 说明 |
|:---------------|:------------------|:------------|
| authorizedApps | String collection | 允许管理 externalConnection 和为 externalConnection 中的内容编制索引的已注册 Azure Active Directory 应用程序的应用程序 ID 的集合。 |

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


