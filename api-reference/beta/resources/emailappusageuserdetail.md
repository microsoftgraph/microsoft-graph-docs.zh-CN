---
title: emailAppUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: dce83b17f029bec2bf8977d0e863dcdb5c7fc4e1a9c5dea731b654d5ce6ab9f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54210069"
---
# <a name="emailappusageuserdetail-resource-type"></a>emailAppUsageUserDetail 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性          | 类型              |
| :---------------- | :---------------- |
| reportRefreshDate | 日期              |
| userPrincipalName | String            |
| displayName       | 字符串            |
| isDeleted         | 布尔值           |
| deletedDate       | 日期              |
| lastActivityDate  | 日期              |
| mailForMac        | String collection |
| outlookForMac     | String collection |
| outlookForWindows | String collection |
| outlookForMobile  | String collection |
| otherForMobile    | String collection |
| outlookForWeb     | String collection |
| pop3App           | String collection |
| imap4App          | String collection |
| smtpApp           | String collection |
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


