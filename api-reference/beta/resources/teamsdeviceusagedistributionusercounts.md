---
title: teamsDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
ms.openlocfilehash: 01b9f67f30a7b2f13aac65cbcd4795792ee0aaa0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345848"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a>teamsDeviceUsageDistributionUserCounts 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   |
| :---------------- | :----- |
| reportRefreshDate | 日期   |
| web               | Int64  |
| windowsPhone      | Int64  |
| androidPhone      | Int64  |
| ios               | Int64  |
| mac               | Int64  |
| windows           | Int64  |
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
