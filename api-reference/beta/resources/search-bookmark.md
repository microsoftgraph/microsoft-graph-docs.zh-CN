---
title: 书签资源类型
description: 书签是组织中常见Microsoft 搜索查询的结果中的管理答案。 书签具有许多属性，使管理员能够更易于在组织中访问常见资源。
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 24582a18ae2ad332a59bc3d8b2db28b3e3189b6a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338215"
---
# <a name="bookmark-resource-type"></a>书签资源类型

命名空间：microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

书签是组织中常见Microsoft 搜索查询的结果中的管理答案。 书签具有许多属性，使管理员能够更易于在组织中访问常见资源。

继承自 [searchAnswer](../resources/search-searchAnswer.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出书签](../api/search-searchentity-list-bookmarks.md)|[microsoft.graph.search.bookmark](../resources/search-bookmark.md) 集合|获取书签对象 [及其](../resources/search-bookmark.md) 属性的列表。|
|[创建书签](../api/search-searchentity-post-bookmarks.md)|[microsoft.graph.search.bookmark](../resources/search-bookmark.md)|创建新的 [书签](../resources/search-bookmark.md) 对象。|
|[获取书签](../api/search-bookmark-get.md)|[microsoft.graph.search.bookmark](../resources/search-bookmark.md)|读取书签对象 [的属性和](../resources/search-bookmark.md) 关系。|
|[更新书签](../api/search-bookmark-update.md)|[microsoft.graph.search.bookmark](../resources/search-bookmark.md)|更新 [书签对象的属性](../resources/search-bookmark.md) 。|
|[删除书签](../api/search-bookmark-delete.md)|无|删除 [书签对象](../resources/search-bookmark.md) 。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|书签的唯 (GUID) 标识符。 继承自 [实体](../resources/entity.md)。|
|displayName|String|搜索结果中显示的书签名称。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|说明|String|搜索结果页上显示的书签说明。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|webUrl|String|书签 URL 链接。 当用户在搜索结果中单击此书签时，他们将转到此 URL。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|lastModifiedBy|[microsoft.graph.identitySet](../resources/identityset.md)|创建或上次修改书签的用户的详细信息。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。 只读。|
|lastModifiedDateTime|DateTimeOffset|创建或编辑书签的时间戳。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。 只读。 |
|categories|String collection|通常用于描述此书签的类别。 例如，IT 和 HR。|
|availabilityStartDateTime|DateTimeOffset|书签开始显示为搜索结果的时间戳。 设置为" `null` 始终可用"。|
|availabilityEndDateTime|DateTimeOffset|书签停止显示为搜索结果的时间戳。 设置为" `null` 始终可用"。|
|languageTags|String collection|地理位置特定的语言名称列表，可以在其中查看此书签。 每个语言标记值都遵循 {language}-{REGION} 模式。 例如，美国 `en-US` 使用的英语。 有关 [可能值的列表](search-api-answers-overview.md#supported-language-tags) ，请参阅支持的语言标记。|
|平台|microsoft.graph.devicePlatformType 集合|能够查看此书签的设备列表和操作系统。 可取值为：`unknown`、`android`、`androidForWork`、`ios`、`macOS`、`windowsPhone81`、`windowsPhone81AndLater`、`windows10AndLater`、`androidWorkProfile`、`androidASOP`。|
|targetedVariations|[microsoft.graph.search.answerVariant](../resources/search-answerVariant.md) 集合|不同国家/地区或设备的书签变体。 当你需要根据用户的设备、国家/地区或两者向用户显示不同的内容时，请使用 。 日期和组设置将应用于所有变体。|
|powerAppIds|String collection|与此Power Apps关联的列表。 如果用户将现有Power Apps添加到书签，他们可以完成任务，例如输入休假时间或在搜索结果页上报告费用。|
|keywords|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|触发此书签显示在搜索结果中的关键字。|
|state|microsoft.graph.search.answerState|书签的状态。 可能的值是：、`published``draft`、`excluded`或 `unknownFutureValue`。|
|isSuggested|Boolean|如此 如果此书签是由用户建议管理员或已缩小和 Microsoft 建议。 只读。|
|groupIds|String collection|能够查看此书签的安全组列表。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.search.bookmark",
  "baseType": "microsoft.graph.search.searchAnswer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.bookmark",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "webUrl": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "categories": [
    "String"
  ],
  "availabilityStartDateTime": "String (timestamp)",
  "availabilityEndDateTime": "String (timestamp)",
  "languageTags": [
    "String"
  ],
  "platforms": [
    "String"
  ],
  "targetedVariations": [
    {
      "@odata.type": "microsoft.graph.search.answerVariant"
    }
  ],
  "powerAppIds": [
    "String"
  ],
  "keywords": {
    "@odata.type": "microsoft.graph.search.answerKeyword"
  },
  "state": "String",
  "isSuggested": "Boolean",
  "groupIds": [
    "String"
  ]
}
```

