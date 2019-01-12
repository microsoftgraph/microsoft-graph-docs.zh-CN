---
title: emailAppUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1ebc99f25bf0b16343f48686496c1dbd7d329e65
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977652"
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
