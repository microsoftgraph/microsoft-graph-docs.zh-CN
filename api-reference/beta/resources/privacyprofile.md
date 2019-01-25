---
title: privacyProfile 资源类型
description: 表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。
localization_priority: Normal
ms.openlocfilehash: 9c110cbdb8a456b43936d3b56db5d4563686ed6e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510118"
---
# <a name="privacyprofile-resource-type"></a>privacyProfile 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。

## <a name="properties"></a>属性
| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|contactEmail|String| 隐私声明联系人的有效 smtp 电子邮件地址。 可选。|
|statementUrl|String| 以 http:// 或 https:// 开头的有效 URL 格式。 最大长度为 255 个字符。 定向到公司隐私声明的 URL。 可选。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/privacyprofile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
