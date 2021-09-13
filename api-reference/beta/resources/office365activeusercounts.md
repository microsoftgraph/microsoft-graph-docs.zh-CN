---
title: office365ActiveUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 2f11c81394dd346d46b50d2c9a19eefb56984956
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59026761"
---
# <a name="office365activeusercounts-resource-type"></a>office365ActiveUserCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性          | 类型   | 描述                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | 日期   | 内容的最新日期。          |
| office365         | Int64  | 活动用户Microsoft 365。 此数字包括 Exchange、OneDrive、SharePoint、Skype For Business、Yammer 和 Microsoft Teams 中Yammer。 您可以在各自的属性说明中查找每个产品的活动用户的定义。 |
| exchange          | Int64  | 活动用户数Exchange。 任何可以阅读和发送电子邮件的用户都将被视为活动用户。 |
| oneDrive          | Int64  | 活动用户数OneDrive。 在内部或外部查看或编辑文件、共享文件或同步文件的任何用户都将被视为活动用户。 |
| sharePoint        | Int64  | 活动用户数SharePoint。 任何在内部或外部查看或编辑文件、共享文件、同步文件或SharePoint页面的用户均被视为活动用户。 |
| skypeForBusiness  | Int64  | Skype For Business 中的活动用户数。 组织或参与会议或加入对等会话的任何用户都将被视为活动用户。 |
| yammer            | Int64  | 活动用户数Yammer。 任何可以发布、阅读或喜欢消息的用户都将被视为活动用户。 |
| teams             | Int64  | 活动用户数Microsoft Teams。 任何在团队频道中发布消息、在私人聊天会话中发送消息或参与会议或通话的用户均被视为活跃用户。 |
| reportDate        | 日期   | 多个用户处于活动状态的日期。 |
| reportPeriod      | String | 报告涵盖的天数。    |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "office365": 1024, 
  "exchange": 1024, 
  "oneDrive": 1024, 
  "sharePoint": 1024, 
  "skypeForBusiness": 1024, 
  "yammer": 1024, 
  "teams": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


