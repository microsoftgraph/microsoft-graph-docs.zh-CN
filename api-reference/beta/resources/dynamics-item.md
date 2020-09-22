---
title: items 资源类型
description: Dynamics 365 Business Central 中的 item 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 89ccee3123fc3f0fc04b620e5b3528f4a253d1fa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058448"
---
# <a name="items-resource-type"></a>items 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Dynamics 365 Business Central 中的项。

## <a name="methods"></a>方法

| 方法                                      |返回类型|说明 |
|:--------------------------------------------|:----------|:-----------|
|[获取项目](../api/dynamics-item-get.md)      |items     |获取一个项目对象。   |
|[发布项目](../api/dynamics-create-item.md)  |items     |创建一个 item 对象。|
|[修补程序项](../api/dynamics-item-update.md)  |items     |更新项目对象。|
|[删除项目](../api/dynamics-item-delete.md)|无      |删除 item 对象。|

## <a name="properties"></a>属性
| 属性           | 类型 |说明                                          |
|:-------------------|:-------|:----------------------------------------------------|
|id                  |GUID    |项目的唯一 ID。 不可编辑。             |
|数字              |string  |物料编号。                                     |
|displayName         |string  |指定项的说明。                 |
|type                |位数 |项目的库存类型。 1 = 库存项，2 = 服务项。 此属性是必需的。|
|堵塞             |boolean |指定无法发布项目的事务，例如，由于该项目处于隔离中。 如果项目被阻止，则设置为 **true**。|
|baseUnitOfMeasureId |GUID    |指定度量单位的 ID。             |
|baseUnitOfMeasure   |[翻.UnitOfMeasure](../resources/dynamics-complextypes.md)|指定项在库存中保留的单位。|
|gtin                |位数 |这是全局贸易项目编号。                |
|itemCategoryId      |GUID |指定项所属的类别。 项类别还包含任何已分配的项属性。|
|inventory           |数位 |指定项目在库存中的单位（例如，棋子、方框或箱）的数量。 只读。|
|价格           |数位 |以指定货币指定项目的一个单位的价格。|
|priceIncludesTax    |boolean |指定单价包含税。 如果单价包含税，则设置为 **true**。|
|unitCost            |数位 |指定项目的每单位成本。             |
|taxGroupId          |GUID    |指定项目的税务组的 ID。      |
|taxGroupCode        |位数 |税组表示符合相同税条款的一组库存物料或资源。|
|lastModifiedDateTime|datetime|项目修改后的最后一个日期/时间。 只读。  |  


## <a name="relationships"></a>关系
税组 (taxGroupCode) 必须存在于税务组表中。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


```json
{
      "id": "GUID",
      "number": "string",
      "displayName": "string",
      "type": "string",
      "blocked": "boolean",
      "baseUnitOfMeasureId": "GUID",
      "baseUnitOfMeasure": "NAV.UnitOfMeasure",
      "gtin": "numeric",
      "itemCategoryId": "GUID",
      "inventory": "decimal",
      "unitPrice": "decimal",
      "priceIncludesTax": "boolean",
      "unitCost": "decimal",
      "taxGroupId": "GUID",
      "taxGroupCode": "string",
      "lastModifiedDateTime": "datetime"
}

```




