---
title: dataSource 资源类型
description: 数据源实体-摘要基类
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 645ae33eb6c43972122623e52bfecf17f39491e4
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597594"
---
# <a name="datasource-resource-type"></a>dataSource 资源类型

命名空间：microsoft.graph

DataSource 实体是一个抽象 baseclass，用于标识电子数据展示的内容源。

## <a name="methods"></a>方法

无

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|创建 **数据源** 的用户。|
|createdDateTime|DateTimeOffset|**数据源** 的创建日期和时间。|
|displayName|String|**数据源** 的显示名称。 这将是 SharePoint 网站的名称。|
|id|String| **数据源** 的 ID。 这不是实际网站的 ID。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSource",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
