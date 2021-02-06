---
title: parentalControlSettings 资源类型
description: 指定应用程序的家长控制设置。 这些设置控制同意体验。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f63f81af9e35183a15ab07b1f8e8fce9e8488bae
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136001"
---
# <a name="parentalcontrolsettings-resource-type"></a>parentalControlSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定应用程序的家长控制设置。 这些设置控制同意体验。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
:---------------|:--------|:----------|
|countriesBlockedForMinors|字符串集合| 指定两 [个字母的 ISO 国家/地区代码](https://www.iso.org/iso-3166-country-codes.html)。 对于此列表中指定的国家/地区中的未成年人，将阻止其访问该应用程序。|
|legalAgeGroupRule| 字符串 | 指定适用于应用用户的法律年龄组规则。 可以设置为下列值之一： <table><tr><th>值</th><th>说明</th></tr><tr><td>允许</td><td>默认值。 强制执行法律最低要求。 这意味着欧盟和韩国的未成年人需要家长同意。</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>强制用户指定出生日期，以遵守 COPPA 规则。 </td></tr><tr><td>RequireConsentForMinors</td><td>需要 18 以下年龄的家长同意，无论国家/地区次要规则如何。</td></tr><tr><td>RequireConsentForKids</td><td>需要 14 以下年龄的家长同意，无论国家/地区次要规则如何。</td></tr><tr><td>BlockMinors</td><td>阻止未成年人使用应用。</td></tr></table> |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.parentalControlSettings"
}-->
```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```


