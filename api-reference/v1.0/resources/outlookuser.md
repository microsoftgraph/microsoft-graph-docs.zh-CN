---
title: outlookUser 资源类型
description: 表示用户可用的 Outlook 服务。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 6a4f15266ebfda3e2af43a5d39e28803fe9d87b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837371"
---
# <a name="outlookuser-resource-type"></a>outlookUser 资源类型


表示用户可用的 Outlook 服务。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Create category](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) |在用户主类别列表中创建 **outlookCategory** 对象。|
|[List categories](../api/outlookuser-list-mastercategories.md) | [outlookCategory](outlookcategory.md) 集合 |获取为用户定义的所有类别。|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md) | [localeInfo](localeinfo.md) 集合 | 获取用户支持的区域设置和语言列表，就像在用户的邮箱服务器上配置的那样。 |
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md) | [timeZoneInformation](timezoneinformation.md) 集合 | 获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。 |


## <a name="properties"></a>属性
无

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|masterCategories|[outlookCategory](../resources/outlookcategory.md) 集合| 为用户定义的类别列表。 | 

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookUser",
  "@odata.annotations": [
    {
      "property": "masterCategories",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
