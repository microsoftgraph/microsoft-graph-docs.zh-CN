---
title: 帐户资源类型
description: Dynamics 365 Business Central 中的 account 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 671d81da52b28558fa5c24b13060b766c8d908c9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076454"
---
# <a name="accounts-resource-type"></a>帐户资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Dynamics 365 Business Central 中的 account 对象。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取帐户](../api/dynamics-account-get.md)|帐户|获取帐户对象。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|GUID|帐户的唯一 ID。|
|数字|字符串，最大大小为20|指定 G/L 帐号的号码。|
|displayName|字符串，最大大小为50|指定 G/L 帐户的名称。|
|“类别”|字符串，最大大小为20|指定 G/L 帐户的类别。|
|子类别|字符串，最大大小为80|指定 G/L 帐户的帐户类别的子类别。|
|堵塞|boolean|指定无法将条目投递到 G/L 帐户。 **如果为 True** ，则表示帐户被阻止，不允许进行发布。|
|lastModifiedDateTime|datetime|帐户修改后的最后一个日期/时间。|


## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "category": "string",
  "subCategory": "string",
  "blocked": "boolean",
  "lastModifiedDateTime": "datetime"
}
```


