---
title: dataSource 资源类型
description: Datasource 实体 - 抽象基类
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: c019a6b8338180584a31382c0741018791973184
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161920"
---
# <a name="datasource-resource-type"></a>dataSource 资源类型

命名空间：microsoft.graph

DataSource 实体是一个抽象基类，用于标识电子数据展示的内容源。

## <a name="methods"></a>方法

无

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|创建 **DataSource 的用户**。|
|createdDateTime|DateTimeOffset|DataSource **的** 创建日期和时间。|
|displayName|String|dataSource 的 显示名称。 这将是 SharePoint 网站的名称。|
|id|String| DataSource 的ID。 这不是实际网站的 ID。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSource",
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
