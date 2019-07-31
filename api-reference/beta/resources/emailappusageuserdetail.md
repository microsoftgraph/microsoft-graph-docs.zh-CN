---
title: emailAppUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ae0409124569f4318df94f97729402a91d4b8e45
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972143"
---
# <a name="emailappusageuserdetail-resource-type"></a>emailAppUsageUserDetail 资源类型

## <a name="properties"></a>属性

| 属性          | 类型              |
| :---------------- | :---------------- |
| reportRefreshDate | 日期              |
| userPrincipalName | String            |
| displayName       | String            |
| isDeleted         | Boolean           |
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
