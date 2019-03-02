---
title: dimensionValues 资源类型
description: Dynamics 365 Business Central 中的维度值。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: da3935b8e784b05551af123c1832d5dc84a2c81c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365316"
---
# <a name="dimensionvalues-resource-type"></a>dimensionValues 资源类型
表示 Dynamics 365 Business Central 中的维度值。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明                   |
|:-------------|:-------------|:-----------------------------|
|[获取 dimensionValues](../api/dynamics-dimensionvalue-get.md)|dimensionValues|获取一个维度值对象。|


## <a name="properties"></a>属性
| 属性           | 类型                  |说明                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|id                  |GUID                   |项目的唯一 ID。                         |
|code                |字符串, 最大大小为20|维度值代码。                          |
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


