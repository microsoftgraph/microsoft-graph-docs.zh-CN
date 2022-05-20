---
title: qna 资源类型
description: 表示Microsoft 搜索中 Q&A)  (问答。
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: d17f10b3613bb4e88791c90fd81e0440ece8eb2d
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602782"
---
# <a name="qna-resource-type"></a>qna 资源类型

命名空间：microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

问&搜索结果页中的管理答案结果是否为特定搜索关键字提供答案。 问&管理员可以直接在搜索中回答用户的问题，而不是提供指向网页的链接。 Q&A 具有许多属性，使管理员能够使其组织中更易于访问的常见资源。

继承自 [searchAnswer](../resources/search-searchAnswer.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 qnas](../api/search-searchentity-list-qnas.md)|[microsoft.graph.search.qna](../resources/search-qna.md) 集合|获取 [qna](../resources/search-qna.md) 对象及其属性的列表。|
|[创建 qna](../api/search-searchentity-post-qnas.md)|[microsoft.graph.search.qna](../resources/search-qna.md)|创建新的 [qna](../resources/search-qna.md) 对象。|
|[获取 qna](../api/search-qna-get.md)|[microsoft.graph.search.qna](../resources/search-qna.md)|读取 [qna](../resources/search-qna.md) 对象的属性和关系。|
|[更新 qna](../api/search-qna-update.md)|[microsoft.graph.search.qna](../resources/search-qna.md)|更新 [qna](../resources/search-qna.md) 对象的属性。|
|[删除 qna](../api/search-qna-delete.md)|无|删除 [qna](../resources/search-qna.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|qna 的唯一标识符 (GUID) 。 继承自 [entity](../resources/entity.md)。|
|displayName|字符串|搜索结果中显示的问题。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|说明|字符串|搜索结果中显示的答案。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|webUrl|String|Qna URL 链接。 当用户在搜索结果中单击此 qna 时，他们将转到此 URL。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|lastModifiedBy|[microsoft.graph.identitySet](../resources/identityset.md)|创建或上次修改 qna 的用户的详细信息。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。 只读。 |
|lastModifiedDateTime|DateTimeOffset| 创建或编辑 qna 的时间戳。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。 只读。|
|availabilityStartDateTime|DateTimeOffset|qna 何时开始显示为搜索结果的时间戳。 `null`设置为始终可用。|
|availabilityEndDateTime|DateTimeOffset|qna 何时停止显示为搜索结果的时间戳。 `null`设置为始终可用。|
|languageTags|字符串集合|地理上特定的语言名称列表，可在其中查看此 QnA。 每个语言标记值都遵循模式 {language}-{region}。 例如，`en-us`英语在美国中使用。 有关可能值的列表，请参阅 [支持的语言标记](search-api-answers-overview.md#supported-language-tags) 。 |
|平台|microsoft.graph.devicePlatformType 集合|能够查看此 qna 的设备和操作系统的列表。 可取值为：`unknown`、`android`、`androidForWork`、`ios`、`macOS`、`windowsPhone81`、`windowsPhone81AndLater`、`windows10AndLater`、`androidWorkProfile`、`androidASOP`。|
|targetedVariations|[microsoft.graph.search.answerVariant](../resources/search-answerVariant.md) 集合|不同国家/地区或设备的 qna 变体。 需要根据用户的设备、国家/地区或两者向用户显示不同内容时使用。 日期和组设置将应用于所有变体。|
|keywords|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|触发此 qna 以显示在搜索结果中的关键字。|
|state|microsoft.graph.search.answerState|qna 的状态。 可能的值为：`published`、`draft`或 `excluded``unknownFutureValue`。|
|isSuggested|Boolean| 如此 如果此 qna 是由用户建议给管理员的，或者是 Microsoft 挖掘和建议的。 只读。|
|groupIds|String collection|能够查看此 qna 的安全组列表。|


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.search.qna",
  "baseType": "microsoft.graph.search.searchAnswer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.qna",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "webUrl": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
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

