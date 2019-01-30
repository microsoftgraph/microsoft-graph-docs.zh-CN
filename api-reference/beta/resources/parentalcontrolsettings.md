---
title: parentalControlSettings 资源类型
description: 指定应用程序的家长控制设置。 这些设置控制的同意体验。
localization_priority: Normal
ms.openlocfilehash: 52a808cd4c3e6f29e4d43c7c4ea5c9e30a81447b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643001"
---
# <a name="parentalcontrolsettings-resource-type"></a>parentalControlSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定应用程序的家长控制设置。 这些设置控制的同意体验。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
:---------------|:--------|:----------|
|countriesBlockedForMinors|String collection| 指定[两个字母的 ISO 国家/地区代码](https://www.iso.org/iso-3166-country-codes.html)。 将此列表中指定的国家/地区从未成年人阻止访问应用程序。|
|legalAgeGroupRule| String | 指定应用于用户的应用程序的法律期限组规则。 可以设置为下列值之一： <table><tr><th>值</th><th>说明</th></tr><tr><td>允许</td><td>默认值。 强制执行法律最小值。 这意味着家长同意，则需要进行评级欧盟和韩国中。</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>强制执行用户指定出生日期遵守 COPPA 规则。 </td></tr><tr><td>RequireConsentForMinors</td><td>需要为 18，无论国家/地区次要规则下方岁家长同意。</td></tr><tr><td>RequireConsentForKids</td><td>需要为 14，无论国家/地区次要规则下方岁家长同意。</td></tr><tr><td>BlockMinors</td><td>使用应用程序的块未成年人。</td></tr></table> |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/parentalcontrolsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
