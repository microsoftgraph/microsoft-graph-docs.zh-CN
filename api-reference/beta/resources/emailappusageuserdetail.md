---
title: emailAppUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 700ef4b222860d19ef3ba78ae583a50e8cf8d0cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499482"
---
# <a name="emailappusageuserdetail-resource-type"></a>emailAppUsageUserDetail 资源类型

命名空间： microsoft. graph

## <a name="properties"></a>属性

| 属性          | 类型              |
| :---------------- | :---------------- |
| reportRefreshDate | 日期              |
| userPrincipalName | String            |
| displayName       | String            |
| isDeleted         | 布尔           |
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
