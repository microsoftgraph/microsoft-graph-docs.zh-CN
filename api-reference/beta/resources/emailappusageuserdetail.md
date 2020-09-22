---
title: emailAppUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8365e856ee1b34b15b1aea3369b6cc22f99991e2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081676"
---
# <a name="emailappusageuserdetail-resource-type"></a>emailAppUsageUserDetail 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性          | 类型              |
| :---------------- | :---------------- |
| reportRefreshDate | 日期              |
| userPrincipalName | 字符串            |
| displayName       | 字符串            |
| isDeleted         | 布尔           |
| deletedDate       | 日期              |
| lastActivityDate  | 日期              |
| mailForMac        | 字符串集合 |
| outlookForMac     | 字符串集合 |
| outlookForWindows | 字符串集合 |
| outlookForMobile  | 字符串集合 |
| otherForMobile    | 字符串集合 |
| outlookForWeb     | 字符串集合 |
| pop3App           | 字符串集合 |
| imap4App          | 字符串集合 |
| smtpApp           | 字符串集合 |
| reportPeriod      | 字符串            |

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


