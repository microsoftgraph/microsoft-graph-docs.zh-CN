---
title: trialBalance 资源类型
description: Dynamics 365 Business Central 中的试算平衡表对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1a7e906e50ddf39e4c9e2d3d9dde11226c7ec662
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534848"
---
# <a name="trialbalance-resource-type"></a>trialBalance 资源类型
表示 Dynamics 365 Business Central 中的试算平衡表。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 trialBalance](../api/dynamics-trialbalance-get.md)|trialBalance|获取试算平衡表对象。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|数字|string|trialBalance 项目的 G/L 帐号|
|accountId|GUID|记录的 G/L 帐户的唯一标识符。|
|accountType|string|记录的 G/L 帐户的帐户类型。|
|显示屏|string|trialBalance 项目的 G/L 帐户名称。|
|totalDebit|string|表示在 G/L 帐户中的借方总额。|
|totalCredit|string|表示 G/L 帐户中的总贷方金额。|
|balanceAtDateDebit|string|表示 G/L 帐户中的日期金额的正余额。|
|balanceAtDateCredit|string|表示在 G/L 帐户中的日期量为负余额。|
|dateFilter|date|用于计算 trialBalance 项目的日期筛选器。|


## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


```json
{
    "number": "string",
    "accountId": "GUID",
    "accountType": "string",
    "display": "string",
    "totalDebit": "string",
    "totalCredit": "string",
    "balanceAtDateDebit": "string",
    "balanceAtDateCredit": "string",
    "dateFilter": "date"
}

```

