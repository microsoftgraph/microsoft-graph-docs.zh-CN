---
title: mailboxUsageQuotaStatusMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 2be392d12aea4dfe5dfd9a7ae21a78fe79bb2fdbb8b571633277ede95687190d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54195069"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a>mailboxUsageQuotaStatusMailboxCounts 资源类型

命名空间：microsoft.graph

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


