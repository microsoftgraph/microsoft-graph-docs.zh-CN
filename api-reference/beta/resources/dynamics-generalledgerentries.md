---
title: generalLedgerEntries 资源类型
description: Dynamics 365 Business Central 中的总帐条目。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 500c78d0e29d83c68c2b7247a9787b977cc8a7b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973602"
---
# <a name="generalledgerentries-resource-type"></a>generalLedgerEntries 资源类型
代表 Dynamics 365 Business Central 中的 generalLedgerEntry 对象。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:-------------|:-------------|:----------|
|[获取 generalLedgerEntries](../api/dynamics-generalledgerentries-get.md)|generalLedgerEntries|获取一个 G/L 入口对象。|

## <a name="properties"></a>属性
| 属性           | 类型                  |说明                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|id                  |位数                |G/L 条目的唯一 ID。              |
|postingDate         |date                   |指定 G/L 条目的过帐日期。 |
|documentNumber      |字符串, 最大大小为20|指定 G/L 条目的文档编号。|
|documentType        |string                 |指定 G/L 项的文档类型。|
|accountId           |GUID                   |指定 G/L 条目的 accountId。    |
|accountNumber       |字符串, 最大大小为20|指定 G/L 条目的 accountNumber。|
|说明         |字符串, 最大大小为50|指定 G/L 条目的说明。  |
|debitAmount         |位数                |指定 G/L 条目的 debitAmount。  |
|creditAmount        |位数                |指定 G/L 条目的 creditAmount。 |
|lastModifiedDateTime|datetime               |修改了 G/L 条目的最后一个日期/时间。|


## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


```json
{
  "id": "int",
  "postingDate": "Date",
  "documentNumber": "string",
  "documentType": "string",
  "accountId": "GUID",
  "accountNumber": "string",
  "description": "string",
  "debitAmount": "decimal",
  "creditAmount": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

