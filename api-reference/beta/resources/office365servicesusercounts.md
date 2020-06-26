---
title: office365ServicesUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 8600e79d425d15746fd7015adea98eb49a8a3c82
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896551"
---
# <a name="office365servicesusercounts-resource-type"></a>office365ServicesUserCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性                 | 类型   | 说明                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | 日期   | 内容的最新日期。          |
| exchangeActive           | Int64  | Exchange 上的活动用户数。 任何可以读取和发送电子邮件的用户都被视为活动用户。 |
| exchangeInactive         | Int64  | Exchange 上的非活动用户数。 |
| oneDriveActive           | Int64  | OneDrive 上的活动用户数。 任何查看或编辑文件、内部或外部共享文件或已同步文件的用户都被视为活动用户。 |
| oneDriveInactive         | Int64  | OneDrive 上的非活动用户数。 |
| sharePointActive         | Int64  | SharePoint 上的活动用户数。 任何查看或编辑过文件、内部或外部共享文件、同步文件或查看 SharePoint 页面的用户都被视为活动用户。 |
| sharePointInactive       | Int64  | SharePoint 上的非活动用户数。 |
| skypeForBusinessActive   | Int64  | Skype For Business 中的活动用户数。 任何组织或参加过会议的用户或加入的对等会话都被视为活动用户。 |
| skypeForBusinessInactive | Int64  | Skype For Business 上的非活动用户数。 |
| yammerActive             | Int64  | Yammer 上的活动用户数。 任何可以发布、阅读或赞邮件的用户都被视为活动用户。 |
| yammerInactive           | Int64  | Yammer 上的非活动用户数。  |
| teamsActive              | Int64  | Microsoft 团队中的活动用户数。 任何在团队频道中投递了邮件、在私人聊天会话中发送的邮件或参与会议或呼叫的用户都被视为活动用户。 |
| teamsInactive            | Int64  | Microsoft 团队中的非活动用户数。     |
| office365Active          | Int64  | Microsoft 365 上的活动用户数。   |
| office365Inactive        | Int64  | Microsoft 365 上的非活动用户数。     |
| reportPeriod             | String | 报告覆盖的天数。    |

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
