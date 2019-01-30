---
title: implicitGrantSettings 资源类型
description: 指定此 web 应用程序是否可以请求令牌使用 OAuth 2.0 隐式流。 单独属性均可用于请求 ID 和访问令牌的隐式流的一部分。 若要启用隐式流，至少一个以下属性必须设置为 true。
localization_priority: Normal
ms.openlocfilehash: 6714b9448f2e49419e41fa62822498ceaa232170
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642763"
---
# <a name="implicitgrantsettings-resource-type"></a>implicitGrantSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定此 web 应用程序是否可以请求令牌使用 OAuth 2.0 隐式流。 单独属性均可用于请求 ID 和访问令牌的隐式流的一部分。 若要启用隐式流，至少一个以下属性必须设置为 true。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
|enableIdTokenIssuance| 布尔值 | 指定此 web 应用程序是否可以请求使用 OAuth 2.0 隐式流 ID 令牌。|
|enableAccessTokenIssuance| 布尔值 | 指定此 web 应用程序是否可以请求使用 OAuth 2.0 隐式流访问令牌。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/implicitgrantsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
