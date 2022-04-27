---
title: documentSetVersionItem 资源类型
description: 表示一个项，它是捕获的文档集版本的一部分。
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: ab6bc8f0084935e66d8fd772c6e1d13b59841012
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061184"
---
# <a name="documentsetversionitem-resource-type"></a>documentSetVersionItem 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个 [项](../resources/listitem.md) ，它是捕获的 [documentSetVersion](../resources/documentsetversion.md) 的一部分。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|itemId|字符串| 项的唯一标识符。 |
|title|String| 项的标题。 |
|versionId|String| 项目的版本 ID。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.documentSetVersionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.documentSetVersionItem",
  "itemId": "String",
  "title": "String",
  "versionId": "String"
}
```

