---
title: agedAccountsPayable 资源类型
description: Dynamics 365 Business Central 中的一个过期的应付帐款对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 679c24b7ef32ef59b34a5885ea745d8c244376b2
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365904"
---
# <a name="agedaccountspayable-resource-type"></a>agedAccountsPayable 资源类型
代表 Dynamics 365 Business Central 中的 agedAccountsPayable 对象, 它显示供应商帐户的帐龄。

## <a name="methods"></a>方法

| 方法         | 返回类型  |说明|
|:---------------|:-------------|:----------|
|[获取 agedAccountsPayable](../api/dynamics-agedaccountspayable-get.md)|agedAccountsPayable|获取 agedAccountsPayable 对象|

## <a name="properties"></a>属性
| 属性      | 类型     |说明                                 |
|:--------------|:---------|:-------------------------------------------|
|vendorId       |GUID      |供应商的唯一 ID。                    |
|vendorNumber   |string    |指定供应商的编号。                  |
|name           |string    |指定供应商的名称。                    |
|currencyCode   |string    |指定货币。                     |
|balanceDue     |位数   |指定供应商到期的总余额。|
|currentAmount  |位数   |指定在第一个帐龄期间之前的余额。|
|period1Amount  |位数   |指定第一个帐龄期间的余额。|
|period2Amount  |位数   |指定第二个帐龄期间的余额。|
|period3Amount  |位数   |指定第三个帐龄期间的余额。|
|agedAsOfDate   |date|指定用于计算帐龄期间的时间段起始日期。|
|periodLengthFilter|string |指定时间段的长度。 可接受的时间单位值为: D、WD、W、M、Q 或 Y (即基于日期的当前时间单位) 可以指定为时间单位的前缀。|


## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


```json
{
    "vendorId": "GUID",
    "vendorNumber": "string",
    "name": "string",
    "currencyCode": "string",
    "balanceDue": "decimal",
    "currentAmount": "decimal",
    "period1Amount": "decimal",
    "period2Amount": "decimal",
    "period3Amount": "decimal",
    "agedAsOfDate": "date",
    "periodLengthFilter": "string"
}

```
