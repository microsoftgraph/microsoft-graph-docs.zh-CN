---
title: answerKeyword 资源类型
description: Answer 关键字允许用户定义将触发管理搜索答案显示在搜索结果中的字词和短语。
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: b63a3a286528c7b1e7a1f87759cf7635499bde01
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338373"
---
# <a name="answerkeyword-resource-type"></a>answerKeyword 资源类型

命名空间：microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

answer 关键字用于配置将触发管理搜索答案显示在搜索结果中的单词和短语。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|keywords|String collection|用于触发搜索答案的关键字集合。|
|matchSimilarKeywords|Boolean|如果 `true`为 ，则指示搜索词包含与应触发搜索答案的关键字类似的单词。|
|reservedKeywords|String collection|确保触发搜索答案的唯一关键字。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.search.answerKeyword"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.answerKeyword",
  "keywords": [
    "String"
  ],
  "reservedKeywords": [
    "String"
  ],
  "matchSimilarKeywords": "Boolean"
}
```

