---
title: workbookApplication 资源类型
description: 表示用于管理工作簿的 Excel 应用程序。
ms.localizationpriority: medium
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3663ba238ac0ab7a2346786d775b16326ddf0193
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139469"
---
# <a name="workbookapplication-resource-type"></a>workbookApplication 资源类型

命名空间：microsoft.graph

表示用于管理工作簿的 Excel 应用程序。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 workbookApplication](../api/workbookapplication-get.md) | [workbookApplication](workbookapplication.md) |读取 workbookApplication 对象的属性和关系。|
|[Calculate](../api/workbookapplication-calculate.md)|无|重新计算 Excel 中当前打开的所有工作簿。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|calculationMode|string|返回工作簿中使用的计算模式。 可取值为：`Automatic`、`AutomaticExceptTables`、`Manual`。|

## <a name="relationships"></a>关系
无。


## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookApplication"
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
  "description": "workbookApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

