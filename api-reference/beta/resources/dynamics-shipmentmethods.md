---
title: shipmentMethods 资源类型
description: Dynamics 365 Business Central 中的装运方法。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 94ebd10ef87946b5333ec5a06d5edccadc298158
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503570"
---
# <a name="shipmentmethods-resource-type"></a>shipmentMethods 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表 Dynamics 365 Business Central 中的送货方法，如 UPS、Fedex 和 DHL。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 shipmentMethods](../api/dynamics-shipmentmethods-get.md)|shipmentMethods|获取装运方法。|
|[Post shipmentMethods](../api/dynamics-create-shipmentmethods.md)|shipmentMethods|创建装运方法。|
|[修补程序 shipmentMethods](../api/dynamics-shipmentmethods-update.md)|shipmentMethods|更新装运方法。|
|[删除 shipmentMethods](../api/dynamics-shipmentmethods-delete.md)|无|删除装运方法。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|GUID|ShipmentMethod 的唯一 ID。 不可编辑。|
|code|string|指定装运方法代码。|
|displayName|string|指定装运方法的显示名称。|
|lastModifiedDateTime|datetime|最后一个日期/时间修改了运输方法。 只读。|  


## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是 shipmentMethod 的 JSON 表示形式。

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


