---
title: mailboxUsageQuotaStatusMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: b87bb1ce91626f9151d294e2243bba72ba72346b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835218"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a>mailboxUsageQuotaStatusMailboxCounts 资源类型

## <a name="properties"></a>属性

| 属性              | 类型   |
| :-------------------- | :----- |
| reportRefreshDate     | 日期   |
| underLimit            | Int64  |
| warningIssued         | Int64  |
| sendProhibited        | Int64  |
| sendReceiveProhibited | Int64  |
| 不确定         | Int64  |
| reportDate            | 日期   |
| reportPeriod          | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageQuotaStatusMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "underLimit": 1024, 
  "warningIssued": 1024, 
  "sendProhibited": 1024, 
  "sendReceiveProhibited": 1024, 
  "indeterminate": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
