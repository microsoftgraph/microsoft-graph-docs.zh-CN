---
title: agedAccountsReceivable 资源类型
description: Dynamics 365 Business Central 中的已过期的应收帐款对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ce5d010c08f956468398082821040e30b4ef2ace
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507614"
---
# <a name="agedaccountsreceivable-resource-type"></a>agedAccountsReceivable 资源类型
代表 Dynamics 365 Business Central 中的 agedAccountsReceivable 对象, 它显示客户帐户的帐龄。

## <a name="methods"></a>方法

| 方法         | 返回类型  |说明|
|:---------------|:-------------|:----------|
|[获取 agedAccountsReceivable](../api/dynamics-agedaccountsreceivable-get.md)|agedAccountsReceivable|获取 agedAccountsReceivable 对象|

## <a name="properties"></a>属性
| 属性       | 类型    |说明                                  |
|:---------------|:--------|:--------------------------------------------|
|customerId      |GUID     |客户的唯一 ID。                   |
|customerNumber  |字符串   |指定 customer 的号码。                 |
|name            |string   |指定客户的名称。                   |
|currencyCode    |字符串   |指定货币。                      |
|balanceDue      |位数  |指定客户的总余额。      |
|currentAmount   |位数  |指定当前帐龄时段的余额。|
|period1Amount   |位数  |指定第一个帐龄期间的余额。 |
|period2Amount   |位数  |指定第二个帐龄期间的余额。|
|period3Amount   |位数  |指定第三个帐龄期间的余额。 |
|agedAsOfDate    |date     |指定用于计算帐龄期间的时间段起始日期。|
|periodLengthFilter|字符串 |指定时间段的长度。 可接受的时间单位包括: D、WD、W、M、Q 和 Y (意味着当前时间单位基于日期) 可以指定为时间单位的前缀。|


## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


```json
{
    "customerId": "GUID",
    "customerNumber": "string",
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


