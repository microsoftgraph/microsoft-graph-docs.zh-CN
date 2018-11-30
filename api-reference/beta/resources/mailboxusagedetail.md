---
title: mailboxUsageDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: af49fac7c6286c7e9f9ce1e6d7ffdede225b4072
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043127"
---
# <a name="mailboxusagedetail-resource-type"></a>mailboxUsageDetail 资源类型

## <a name="properties"></a>属性

| 属性                        | 类型    |
| :------------------------------ | :------ |
| reportRefreshDate               | 日期    |
| userPrincipalName               | 字符串  |
| displayName                     | 字符串  |
| 被                       | 布尔 |
| deletedDate                     | 日期    |
| createdDate                     | 日期    |
| lastActivityDate                | 日期    |
| itemCount                       | Int64   |
| storageUsedInBytes              | Int64   |
| issueWarningQuotaInBytes        | Int64   |
| prohibitSendQuotaInBytes        | Int64   |
| prohibitSendReceiveQuotaInBytes | Int64   |
| reportPeriod                    | String  |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "createdDate": "Date", 
  "lastActivityDate": "Date", 
  "itemCount": 1024, 
  "storageUsedInBytes": 1024, 
  "issueWarningQuotaInBytes": 1024, 
  "prohibitSendQuotaInBytes": 1024, 
  "prohibitSendReceiveQuotaInBytes": 1024, 
  "reportPeriod": "String"
}
```
