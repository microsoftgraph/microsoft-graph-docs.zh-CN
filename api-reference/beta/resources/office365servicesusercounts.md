---
title: office365ServicesUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 276153f9613f464cdf11f6dfdad307bb341f646d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982150"
---
# <a name="office365servicesusercounts-resource-type"></a>office365ServicesUserCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性                 | 类型   | 说明                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | 日期   | 内容的最新日期。          |
| exchangeActive           | Int64  | Exchange 上的活动用户数。 任何可以阅读和发送电子邮件的用户都将被视为活动用户。 |
| exchangeInactive         | Int64  | Exchange 上的非活动用户数。 |
| oneDriveActive           | Int64  | OneDrive 上的活跃用户数。 任何在内部或外部查看或编辑文件、共享文件或同步文件的用户都将被视为活动用户。 |
| oneDriveInactive         | Int64  | OneDrive 上的非活动用户数。 |
| sharePointActive         | Int64  | SharePoint 上的活动用户数。 任何在内部或外部查看或编辑文件、共享文件、同步文件或查看 SharePoint 页面的用户都将被视为活动用户。 |
| sharePointInactive       | Int64  | SharePoint 上的非活动用户数。 |
| skypeForBusinessActive   | Int64  | Skype For Business 上的活动用户数。 组织或参与会议或加入对等会话的任何用户都将被视为活动用户。 |
| skypeForBusinessInactive | Int64  | Skype For Business 上的非活动用户数。 |
| yammerActive             | Int64  | Yammer 上的活动用户数。 任何可以发布、阅读或喜欢消息的用户都将被视为活动用户。 |
| yammerInactive           | Int64  | Yammer 上的非活动用户数。  |
| teamsActive              | Int64  | Microsoft Teams 上的活动用户数。 任何在团队频道中发布消息、在私人聊天会话中发送消息或参与会议或通话的用户均被视为活动用户。 |
| teamsInactive            | Int64  | Microsoft Teams 上的非活动用户数。     |
| office365Active          | Int64  | Microsoft 365 上的活动用户数。   |
| office365Inactive        | Int64  | Microsoft 365 上的非活动用户数。     |
| reportPeriod             | String | 报告涵盖的天数。    |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeActive": 1024, 
  "exchangeInactive": 1024, 
  "oneDriveActive": 1024, 
  "oneDriveInactive": 1024, 
  "sharePointActive": 1024, 
  "sharePointInactive": 1024, 
  "skypeForBusinessActive": 1024, 
  "skypeForBusinessInactive": 1024, 
  "yammerActive": 1024, 
  "yammerInactive": 1024, 
  "teamsActive": 1024, 
  "teamsInactive": 1024, 
  "office365Active": 1024,
  "office365Inactive": 1024,
  "reportPeriod": "String"
}
```


