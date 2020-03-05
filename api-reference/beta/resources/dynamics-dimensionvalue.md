---
title: dimensionValues 资源类型
description: Dynamics 365 Business Central 中的维度值。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 368fc28f7bd46d8d5385b6e6041cd82255e0271f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504137"
---
# <a name="dimensionvalues-resource-type"></a>dimensionValues 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Dynamics 365 Business Central 中的维度值。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明                   |
|:-------------|:-------------|:-----------------------------|
|[获取 dimensionValues](../api/dynamics-dimensionvalue-get.md)|dimensionValues|获取一个维度值对象。|


## <a name="properties"></a>属性
| 属性           | 类型                  |说明                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|id                  |GUID                   |项目的唯一 ID。                         |
|code                |字符串，最大大小为20|维度值代码。                          |
|displayName         |string                 |指定维度值的名称。 此名称将显示在使用维度值的位置。|
|lastModifiedDateTime|datetime               |修改了维度值的最后一个日期/时间。|  


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```


