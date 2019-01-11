---
title: office365ServicesUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 18282aaa8dcd176a6eaa3a8176154670bfd6da9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808013"
---
# <a name="office365servicesusercounts-resource-type"></a>office365ServicesUserCounts 资源类型

## <a name="properties"></a>属性

| 属性                 | 类型   | Description                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | 日期   | 内容最晚日期。          |
| exchangeActive           | Int64  | 在 Exchange 上的活动用户数。 任何用户都可以读取和发送电子邮件被视为活动用户。 |
| exchangeInactive         | Int64  | 在 Exchange 上的非活动用户数。 |
| oneDriveActive           | Int64  | 在 OneDrive 上的活动用户数。 查看或编辑文件、 内部或外部，共享文件或同步文件的任何用户被视为活动用户。 |
| oneDriveInactive         | Int64  | Onedrive 非活动用户数。 |
| sharePointActive         | Int64  | 在 SharePoint 上的活动用户数。 查看或编辑文件、 共享文件内部或外部同步文件，或查看 SharePoint 页的任何用户被视为活动用户。 |
| sharePointInactive       | Int64  | 在 SharePoint 上的非活动用户数。 |
| skypeForBusinessActive   | Int64  | Skype 的业务上的活动用户数。 组织或参加会议，或加入对等会话的任何用户被视为活动用户。 |
| skypeForBusinessInactive | Int64  | Skype 的业务的非活动用户数。 |
| yammerActive             | Int64  | Yammer 上的活动用户数。 任何用户都可以发布、 读取或类似于邮件被视为活动用户。 |
| yammerInactive           | Int64  | 在 Yammer 上的非活动用户数。  |
| teamsActive              | Int64  | 团队上的活动用户数。 在工作组通道中发布消息、 私人聊天会话中发送的邮件或参加会议或进行呼叫的任何用户被视为活动用户。 |
| teamsInactive            | Int64  | 团队上的活动用户数。     |
| reportPeriod             | 字符串 | 报告涵盖天数。    |

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
  "reportPeriod": "String"
}
```
