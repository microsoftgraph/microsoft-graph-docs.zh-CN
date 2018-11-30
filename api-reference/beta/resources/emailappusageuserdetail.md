---
title: emailAppUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 951d53f7491ff7f2b7721b14ed354d770cfd1730
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042088"
---
# <a name="emailappusageuserdetail-resource-type"></a>emailAppUsageUserDetail 资源类型

## <a name="properties"></a>属性

| 属性          | 类型              |
| :---------------- | :---------------- |
| reportRefreshDate | 日期              |
| userPrincipalName | 字符串            |
| displayName       | 字符串            |
| 被         | 布尔           |
| deletedDate       | 日期              |
| lastActivityDate  | 日期              |
| mailForMac        | String 集合 |
| outlookForMac     | String 集合 |
| outlookForWindows | String 集合 |
| outlookForMobile  | String 集合 |
| otherForMobile    | String 集合 |
| outlookForWeb     | String 集合 |
| pop3App           | String 集合 |
| imap4App          | String 集合 |
| smtpApp           | String 集合 |
| reportPeriod      | String            |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "mailForMac": ["String"], 
  "outlookForMac": ["String"], 
  "outlookForWindows": ["String"], 
  "outlookForMobile": ["String"], 
  "otherForMobile": ["String"], 
  "outlookForWeb": ["String"], 
  "pop3App": ["String"], 
  "imap4App": ["String"], 
  "smtpApp": ["String"], 
  "reportPeriod": "String"
}
```
