---
title: educationTeamsAppResource 资源类型
description: 对应于[已安装的Microsoft Teams应用](teamsappinstallation.md)。 这允许教育服务用户使用嵌入式Teams应用程序创建和共享分配。
author: adarshgh
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a3f77be2aa1a5e6566b8d216735138da2daab8c3
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461686"
---
# <a name="educationteamsappresource-resource-type"></a>educationTeamsAppResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

与[已安装的Microsoft Teams应用](teamsappinstallation.md)对应的教育资源。 这允许教育服务用户使用嵌入式Teams应用程序（如 YouTube 或 FlipGrid）创建和共享作业。

有关在 Microsoft Teams 上使用 FlipGrid 进行教育的信息，请参阅 [FlipGrid 简介](https://education.microsoft.com/en-us/resource/13cb22b1)。

继承自 [educationResource](educationresource.md)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|string|资源的显示名称。|
|appId|string|Teams应用程序的应用 ID。|
|appIconWebUrl|string|指向应用图标的 URL。|
|teamsEmbeddedContentUrl|string|将由Teams打开的应用资源的 URL。|
|webUrl|string|可在浏览器中打开的应用资源的 URL。|
|createdBy|String|创建此资源的用户的显示名称。 继承自 **educationResource**。|
|createdDateTime|DateTimeOffset|添加重索的日期时间。 继承自 **educationResource**。|
|lastModifiedBy|[identitySet](identityset.md)|最后一个修改资源的用户。 继承自 **educationResource**。|
|lastModifiedDateTime|DateTimeOffset|上次修改资源的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 继承自 **educationResource**。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeamsAppResource"
}-->

```json
{
  "displayName": "String",
  "appId": "Unique String",
  "appIconWebUrl": "String URL",
  "teamsEmbeddedContentUrl": "String URL",
  "webUrl": "String URL",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


