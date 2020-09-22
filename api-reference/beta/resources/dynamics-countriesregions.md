---
title: countriesRegions 资源类型
description: Dynamics 365 Business Central 中的国家/地区对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 490fa240cda525b517bf4e8dcec3e89aedbcc201
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049807"
---
# <a name="countriesregions-resource-type"></a>countriesRegions 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表 Dynamics 365 业务中心中的 countriesRegions 对象，该业务中心是地址的一部分。

## <a name="methods"></a>方法

| 方法                                                              | 返回类型    |说明                |
|:--------------------------------------------------------------------|:---------------|:--------------------------|
|[获取 countriesRegions](../api/dynamics-countriesregions-get.md)      |countriesRegions|获取国家/地区。   |
|[Post countriesRegions](../api/dynamics-create-countriesregions.md)  |countriesRegions|创建国家/地区。|
|[修补程序 countriesRegions](../api/dynamics-countriesregions-update.md) |countriesRegions|更新国家/地区。|
|[删除 countriesRegions](../api/dynamics-countriesregions-delete.md)|无            |删除国家/地区。|

## <a name="properties"></a>属性
| 属性       | 类型       |说明                                                  |
|:---------------|:-----------|:------------------------------------------------------------|
|id              |GUID        |国家/地区的唯一 ID。 不可编辑。           |
|code            |string      |指定国家/地区的代码。                    |
|displayName     |string      |指定国家/地区的显示名称。            |
|addressFormat   |string      |指定在面向外部的文档上显示的地址的格式。 将地址格式链接到国家/地区代码，以便基于包含该国家/地区代码的卡片或文档的面向外部的文档使用指定的地址格式。|
|lastModifiedDateTime|datetime|国家/地区的最后修改日期时间。 只读。|  


## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是 countriesRegions 的 JSON 表示形式。


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "addressFormat": "string",
  "lastModifiedDateTime": "datetime"
}

```




