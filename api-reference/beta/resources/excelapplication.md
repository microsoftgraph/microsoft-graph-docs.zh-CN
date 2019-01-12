---
title: 应用程序资源类型
description: 表示用于管理工作簿的 Excel 应用程序。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 250141ff6c6da3a81a1b3492908bc2e04b5a0605
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921974"
---
# <a name="application-resource-type"></a>应用程序资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示用于管理工作簿的 Excel 应用程序。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取应用程序](../api/excelapplication-get.md) | [Application](application.md) |读取属性和 application 对象的关系。|
|[Calculate](../api/excelapplication-calculate.md)|无|重新计算 Excel 中当前打开的所有工作簿。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|calculationMode|string|返回工作簿中使用的计算模式。 可取值为：`Automatic`、`AutomaticExceptTables`、`Manual`。 只读。|

## <a name="relationships"></a>Relationships
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
<!-- {
  "type": "#page.annotation",
  "description": "Application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
