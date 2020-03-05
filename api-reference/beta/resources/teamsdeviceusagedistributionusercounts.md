---
title: teamsDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c6b10af0e4b32c37a5fe365dc8deedae63efc8c4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519874"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a>teamsDeviceUsageDistributionUserCounts 资源类型

命名空间： microsoft. graph

## <a name="properties"></a>属性

| 属性          | 类型   |
| :---------------- | :----- |
| reportRefreshDate | 日期   |
| web               | Int64  |
| windowsPhone      | Int64  |
| androidPhone      | Int64  |
| ios               | Int64  |
| mac               | Int64  |
| 时间           | Int64  |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "reportPeriod": "String"
}
```
