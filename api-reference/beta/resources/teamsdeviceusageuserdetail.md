---
title: teamsDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5bd7443e775a8a9de0dbbc27cf8843331f8f8cb7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007625"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>teamsDeviceUsageUserDetail 资源类型

## <a name="properties"></a>属性

| 属性          | 类型    |
| :---------------- | :------ |
| reportRefreshDate | 日期    |
| userPrincipalName | String  |
| lastActivityDate  | 日期    |
| isDeleted         | Boolean |
| deletedDate       | 日期    |
| usedWeb           | Boolean |
| usedWindowsPhone  | Boolean |
| usediOS           | Boolean |
| usedMac           | Boolean |
| usedAndroidPhone  | Boolean |
| usedWindows       | Boolean |
| reportPeriod      | String  |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "reportPeriod": "String"
}
```
