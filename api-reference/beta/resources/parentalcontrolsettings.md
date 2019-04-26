---
title: parentalControlSettings 资源类型
description: 指定应用程序的家长控制设置。 这些设置控制许可体验。
localization_priority: Normal
ms.openlocfilehash: 52a808cd4c3e6f29e4d43c7c4ea5c9e30a81447b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568666"
---
# <a name="parentalcontrolsettings-resource-type"></a>parentalControlSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定应用程序的家长控制设置。 这些设置控制许可体验。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
:---------------|:--------|:----------|
|countriesBlockedForMinors|String collection| 指定[两个字母的 ISO 国家/地区代码](https://www.iso.org/iso-3166-country-codes.html)。 将阻止对此列表中指定国家/地区的未成年人访问应用程序。|
|legalAgeGroupRule| String | 指定适用于应用程序用户的法律年龄组规则。 可以设置为下列值之一： <table><tr><th>值</th><th>说明</th></tr><tr><td>允许</td><td>默认值。 强制实施合法的最小值。 这意味着欧盟和韩国的未成年人需要家长同意。</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>强制用户指定要符合 COPPA 规则的出生日期。 </td></tr><tr><td>RequireConsentForMinors</td><td>要求对低于18岁的家长同意, 而不考虑国家/地区的次要规则。</td></tr><tr><td>RequireConsentForKids</td><td>需要对低于14的年龄进行家长同意, 而不考虑国家/地区的次要规则。</td></tr><tr><td>BlockMinors</td><td>阻止未成年人使用应用。</td></tr></table> |

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
