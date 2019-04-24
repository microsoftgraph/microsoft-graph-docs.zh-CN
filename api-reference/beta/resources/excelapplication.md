---
title: 应用程序资源类型
description: 表示用于管理工作簿的 Excel 应用程序。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 48ee13a67d97f9c5c1a96a6ef6e104c5629f4108
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506529"
---
# <a name="application-resource-type"></a>应用程序资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用于管理工作簿的 Excel 应用程序。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取应用程序](../api/excelapplication-get.md) | [应用程序](application.md) |读取 application 对象的属性和关系。|
|[Calculate](../api/excelapplication-calculate.md)|无|重新计算 Excel 中当前打开的所有工作簿。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|calculationMode|string|返回工作簿中使用的计算模式。 可取值为：`Automatic`、`AutomaticExceptTables`、`Manual`。 只读。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/excelapplication.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
