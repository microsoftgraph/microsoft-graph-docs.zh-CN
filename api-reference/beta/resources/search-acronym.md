---
title: 首字母缩写资源类型
description: 首字母缩写词是 Microsoft 搜索结果中用于定义组织中常见首字母缩写词的管理答案。
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 0201a3b76201825b13e069b52924eacca9077d9f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338388"
---
# <a name="acronym-resource-type"></a>首字母缩写资源类型

命名空间：microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

首字母缩写词是 Microsoft 搜索结果中用于定义组织中常见首字母缩写词的管理答案。

继承自 [searchAnswer](../resources/search-searchAnswer.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出首字母缩略词](../api/search-searchentity-list-acronyms.md)|[microsoft.graph.search.acronym](../resources/search-acronym.md) 集合|获取首字母缩写词对象 [及其](../resources/search-acronym.md) 属性的列表。|
|[创建首字母缩略词](../api/search-searchentity-post-acronyms.md)|[microsoft.graph.search.acronym](../resources/search-acronym.md)|创建新的 [首字母缩写词](../resources/search-acronym.md) 对象。|
|[获取首字母缩略词](../api/search-acronym-get.md)|[microsoft.graph.search.acronym](../resources/search-acronym.md)|读取首字母缩写词对象 [的属性和](../resources/search-acronym.md) 关系。|
|[更新首字母缩略词](../api/search-acronym-update.md)|[microsoft.graph.search.acronym](../resources/search-acronym.md)|更新首字母缩写 [词对象](../resources/search-acronym.md) 的属性。|
|[删除首字母缩略词](../api/search-acronym-delete.md)|无|删除首字母 [缩写](../resources/search-acronym.md) 词对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|A brief description of the acronym that gives users more info about the acronym and what it stands for. 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|displayName|String|实际的短格式或缩写。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|id|String|首字母缩写 (GUID) 的唯一标识符。 继承自 [实体](../resources/entity.md)。|
|lastModifiedBy|[microsoft.graph.identitySet](../resources/identityset.md)|创建或上次修改首字母缩写词的用户的详细信息。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。 只读。|
|lastModifiedDateTime|DateTimeOffset|创建或编辑缩写词的时间戳。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。 只读。|
|standsFor|String 集合|首字母缩写词代表什么。|
|state|microsoft.graph.search.answerState|首字母缩写词的状态。 可能的值是：、`published``draft`、`excluded`或 `unknownFutureValue`。|
|webUrl|String|用户可以访问的页面或网站的 URL，以了解有关缩写词详细信息。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.search.acronym",
  "baseType": "microsoft.graph.search.searchAnswer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.acronym",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "webUrl": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "standsFor": [
    "String"
  ],
  "state": "String"
}
```

