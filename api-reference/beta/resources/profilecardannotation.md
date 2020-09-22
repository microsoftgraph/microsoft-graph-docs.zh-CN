---
title: profileCardAnnotation 资源类型
description: 允许管理员自定义 Microsoft 365 配置文件卡片中所选字段的外观。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 57b6378c811727676f7b34c1812955639598054b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973727"
---
# <a name="profilecardannotation-resource-type"></a>profileCardAnnotation 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于为共享的 Microsoft 365 人员 experieence 中显示的字段设置自定义显示名称。 管理员可以为其组织中支持的语言定义默认的显示名称字符串和一组替代转换。

## <a name="properties"></a>属性

| 属性     | 类型                                                            | 说明                                                                                                                       |
|:-------------|:----------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------|
|displayName   |String                                                           | 如果存在，则配置文件卡片将使用此字段的值作为体验 (中的默认属性标签。例如，"成本中心" ) 。 |
|localizations |[displayNameLocalization](displaynamelocalization.md) 集合 | 此集合中的每个资源都代表给定语言的属性名称的本地化值，用作该区域设置的默认标签。 例如，拥有客户端的用户将 `no-NB` "Kostnads Senter" 作为属性标签，而不是 "成本中心"。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profileCardAnnotation",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "localizations": [
    {
      "displayName": "String",
      "languageTag": "String"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profileCardAnnotation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


