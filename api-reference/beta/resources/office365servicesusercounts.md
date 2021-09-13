---
title: office365ServicesUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 6470804a26a35b1aaf8411d5c0d5fddd2a3e0bbf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095323"
---
# <a name="office365servicesusercounts-resource-type"></a>office365ServicesUserCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性                 | 类型   | 说明                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | 日期   | 内容的最新日期。          |
| exchangeActive           | Int64  | 活动用户Exchange。 任何可以阅读和发送电子邮件的用户都将被视为活动用户。 |
| exchangeInactive         | Int64  | 非活动用户Exchange。 |
| oneDriveActive           | Int64  | 活动用户OneDrive。 在内部或外部查看或编辑文件、共享文件或同步文件的任何用户都将被视为活动用户。 |
| oneDriveInactive         | Int64  | 非活动用户OneDrive。 |
| sharePointActive         | Int64  | 活动用户SharePoint。 任何在内部或外部查看或编辑文件、共享文件、同步文件或SharePoint页面的用户均被视为活动用户。 |
| sharePointInactive       | Int64  | 非活动用户SharePoint。 |
| skypeForBusinessActive   | Int64  | Skype For Business 上的活动用户数。 组织或参与会议或加入对等会话的任何用户都将被视为活动用户。 |
| skypeForBusinessInactive | Int64  | Skype For Business 上的非活动用户数。 |
| yammerActive             | Int64  | 活动用户Yammer。 任何可以发布、阅读或喜欢消息的用户都将被视为活动用户。 |
| yammerInactive           | Int64  | 非活动用户Yammer。  |
| teamsActive              | Int64  | 活动用户Microsoft Teams。 任何在团队频道中发布消息、在私人聊天会话中发送消息或参与会议或通话的用户均被视为活跃用户。 |
| teamsInactive            | Int64  | 非活动用户Microsoft Teams。     |
| office365Active          | Int64  | 活动用户Microsoft 365。   |
| office365Inactive        | Int64  | 非活动用户Microsoft 365。     |
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


