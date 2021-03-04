---
title: dataSource 资源类型
description: DataSource 实体是一个抽象基类，用于标识电子数据展示的内容源。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 2f945ba74a5576a35146ee1832f3740b537ed23b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446156"
---
# <a name="datasource-resource-type"></a>dataSource 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

DataSource 实体是一个抽象基类，用于标识电子数据展示的内容源。

## <a name="methods"></a>Methods

无

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|创建 **DataSource 的用户**。|
|createdDateTime|DateTimeOffset|创建 **dataSource 的** 日期和时间。|
|displayName|String|dataSource 显示名称 **。** 这将是 SharePoint 网站的名称。|
|id|String| DataSource 的ID。 这不是实际网站的 ID。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.dataSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
