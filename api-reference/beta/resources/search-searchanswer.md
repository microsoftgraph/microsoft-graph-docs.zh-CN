---
title: searchAnswer 资源类型
description: 搜索答案是其他搜索答案的基本类型。
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 06fa9cfe754af55d4ee19640a9d75c00b7dbca2f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338370"
---
# <a name="searchanswer-resource-type"></a>searchAnswer 资源类型

命名空间：microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

搜索答案是其他搜索答案的基本类型，例如首字母[缩写](../resources/search-acronym.md)词、书签和 [QnA](../resources/search-qna.md) 资源。 [](../resources/search-bookmark.md) 包括应用于其他搜索应答实体的属性。


继承自 [实体](../resources/entity.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|搜索答案 (GUID) 的唯一标识符。 继承自 [实体](../resources/entity.md)。|
|displayName|String|搜索结果中显示的搜索应答名称。|
|description|String|搜索结果页面上显示的搜索答案说明。|
|webUrl|String|搜索应答 URL 链接。 当用户在搜索结果中单击此搜索答案时，他们将转到此 URL。|
|lastModifiedBy|[microsoft.graph.identitySet](../resources/identityset.md)|创建或上次修改搜索答案的用户的详细信息。 只读。|
|lastModifiedDateTime|DateTimeOffset|创建或编辑搜索答案的时间戳。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.search.searchAnswer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.searchAnswer",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "webUrl": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```

