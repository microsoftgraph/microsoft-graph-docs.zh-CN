---
title: emailActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a25061ccea7c6971625a96e9ececd60b3f87a9f4817c1aee4c8892385a6c7d55
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54248976"
---
# <a name="emailactivityuserdetail-resource-type"></a>emailActivityUserDetail 资源类型

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
| sendCount         | Int64             |
| receiveCount      | Int64             |
| readCount         | Int64             |
| assignedProducts  | String collection |
| reportPeriod      | String            |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "sendCount": 1024, 
  "receiveCount": 1024, 
  "readCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```


