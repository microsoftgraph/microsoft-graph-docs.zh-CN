---
title: 配置资源类型
description: 指定允许管理 externalConnection 和为 externalConnection 中的内容编制索引的附加应用程序 ID。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 05fbf022c11cf318281831d1b4e8572646875a06
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467647"
---
# <a name="configuration-resource-type"></a>配置资源类型

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定允许管理 externalConnection 和为 externalConnection 中的内容编制索引的附加[应用程序 ID。](../resources/externalconnectors-externalconnection.md)

## <a name="properties"></a>属性

| 属性       | 类型              | 说明 |
|:---------------|:------------------|:------------|
| authorizedAppIds | 字符串集合 | 允许管理 externalConnection 和为 externalConnection 中的内容编制索引的已注册 Azure Active Directory 应用程序的应用程序 ID 的集合。 |

> [!NOTE]
> 属性 `authorizedAppIds` 以前名为 `authorizedApps` 。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.configuration",
  "baseType": null
}-->

```json
{
  "authorizedAppIds": ["String"]
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
