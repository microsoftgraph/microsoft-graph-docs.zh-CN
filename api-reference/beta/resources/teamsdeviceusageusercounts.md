---
title: teamsDeviceUsageUserCounts 资源类型
description: 表示按设备类型表示的每日用户数。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9d7b813727a5ac9b2f7547e108bad8ee455d206b
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766572"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a>teamsDeviceUsageUserCounts 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示按设备类型表示的每日用户数。

## <a name="properties"></a>属性

| 属性          | 类型   | 说明                                                  |
| :---------------- | :----- | ------------------------------------------------------------ |
| reportRefreshDate | 日期   | 内容的最新日期。                              |
| web               | Int64  | 在设备上 Teams Web 客户端中处于活动状态的用户数。 |
| windowsPhone      | Int64  | 在适用于 Windows Phone 的 Teams 移动客户端上处于活动状态的用户数量。 |
| androidPhone      | Int64  | 在适用于 Android 的 Teams 移动客户端上处于活动状态的用户数。 |
| ios               | Int64  | 在适用于 iOS 的 Teams 移动客户端上处于活动状态的用户数量。 |
| mac               | Int64  | 在 macOS 计算机上 Teams 桌面客户端中处于活动状态的用户数。 |
| windows           | Int64  | 在基于 Windows 的计算机上在 Teams 桌面客户端中处于活动状态的用户数。 |
| chromeOS          | Int64  | 在 ChromeOS 计算机上 Teams 桌面客户端中处于活动状态的用户数。 |
| linux             | Int64  | 在 Linux 计算机上在 Teams 桌面客户端中处于活动状态的用户数。 |
| reportDate        | 日期   | 用户执行活动的日期。        |
| reportPeriod      | String | 报告涵盖的天数。                        |

## <a name="representation"></a>表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
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
  "chromeOS": 1024, 
  "linux": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


