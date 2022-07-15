---
title: searchHit 资源类型
description: searchHit 实体的说明
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 708945d9f6f28fe1ce83b40f276c5e8d7700112f
ms.sourcegitcommit: 84db9d70672e7a36a1130ff4f4b9baf3554d287f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2022
ms.locfileid: "66810275"
---
# <a name="searchhit-resource-type"></a>searchHit 资源类型

命名空间：microsoft.graph

表示搜索结果列表中的单个结果。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|contentSource|String|**externalItem** 所属的内容源的名称。|
|hitId|String|项的内部标识符。 标识符的格式因实体类型而异。 有关详细信息，请参阅 [hitId 格式](#hitid-format)。|
|排名|Int32|结果的排名或顺序。|
|resultTemplateId|String|用于呈现搜索结果的结果模板的 ID。 此 ID 必须映射到 **resultTemplates** 字典中的显示布局，该字典也包含在 [searchResponse 中](searchresponse.md)。|
|resource|[实体](entity.md)|搜索结果的基础 Microsoft Graph 表示形式。|
|摘要|String|如果摘要可用，则为结果的摘要。|

### <a name="hitid-format"></a>hitId 格式

| 实体类型     | ID 格式        | 示例 |
|:-------------|:------------|:------------|
|消息|RestId|`AAMkAGIwMDA5MmY0LWY5ZTgtNGY5YS04NzczLWNhNjc0ZGIyZDBjYgBGAAAAAADm35sgHbzESapJ8_BjBlhEBwDAYtphe7dsRbDrOT-HAHoKAACmqNsoAADAYtphe7dsRbDrOT-HAHoKAAFsBhyEAAA=`|
|event|EwsId|`AAMkAGIwMDA5MmY0LWY5ZTgtNGY5YS04NzczLWNhNjc0ZGIyZDBjYgFRAAgI232z8Q+AAEYAAAAA5t+bIB28xEmqSfPgYwZYRAcAwGLaYXu3bEWw6zk/xwB6CgAAAAABDQAAwGLaYXu3bEWw6zk/xwB6CgABGnD/jwAAEA==`|
|list|GUID|`6249f5a0-c9fd-4103-8da5-8362fe911151`|
|listItem|GUID|`89b4aeff-de77-4b0e-bec9-a20cd4f6c32d` |
|网站|Host，GUID，GUID|`microsoft.sharepoint.com,a5eb6988-c9ad-44be-b3b4-d334d01066c0,4c5ce7de-dbe6-4807-9909-3018f0b83266`|
|驱动器|编码的字符串|`b!kf7AlbfRu0SMqtfcmhLTwf7MGLd-Z0BEqfzvkoqsr21iQFpfPV09TIVf1sa8xOJ0` |
|driveItem|编码的字符串|`01ALOVTAX7V22IS566BZF35SNCBTKPNQZN`|
|externalItem|编码的字符串|`AAMkADRiYWU5MDRkLWE1NGEtNDg5OS1hZWM2LWIxOWZmNzQzMTdiYQBGAAAAAAAvZTGE+1bNQp4lDRL1ctayBwCQNOp97HTbQK/QVOV30iomAAAAEF6yAACQNOp97HTbQK/QVOV30iomAAAAG/DWAAA=` |
|person|GUID@GUID|`497b7a2a-9e1a-48d7-80e8-2965d2fc3a81@72f988bf-86f1-41af-91ab-2d7cd011db47`|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHit",
  "baseType": null
}-->

```json
{
  "contentSource": "String",
  "hitId": "String",
  "rank": "Int32",
  "resultTemplateId": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" },
  "summary": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

