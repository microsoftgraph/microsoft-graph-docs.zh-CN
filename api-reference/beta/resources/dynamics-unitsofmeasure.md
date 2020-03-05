---
title: unitsOfMeasure 资源类型
description: Dynamics 365 Business Central 中的度量单位对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 9b0774f24109f40684039bd8ac98188903f28c3d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503010"
---
# <a name="unitsofmeasure-resource-type"></a>unitsOfMeasure 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个度量单位，它是量的标准度量单位，在 Dynamics 365 Business Central 中。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 unitsOfMeasure](../api/dynamics-unitsofmeasure-get.md)|unitsOfMeasure|获取度量单位对象。|
|[Post unitsOfMeasure](../api/dynamics-create-unitsofmeasure.md)|unitsOfMeasure|创建一个度量单位对象。|
|[修补程序 unitsOfMeasure](../api/dynamics-unitsofmeasure-update.md)|unitsOfMeasure|更新度量单位对象。|
|[删除 unitsOfMeasure](../api/dynamics-unitsofmeasure-delete.md)|无|删除度量单位对象。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|GUID|UnitsOfMeasure 的唯一 ID。 不可编辑。|
|code|string|指定度量单位的代码。|
|displayName|string|指定度量单位的显示名称。|
|internationalStandardCode|string|根据与电子发送销售文档的连接的 UNECE Rec20 标准，指定度量单位代码（表示）。|
|lastModifiedDateTime|datetime|最后一个 datetime 的度量单位已修改。 只读。|  


## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是**unitsOfMeasure**资源的 JSON 表示形式。

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "internationalStandardCode": "string",
  "lastModifiedDateTime": "datetime"
}

```
