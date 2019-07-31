---
title: office365ActiveUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 0d0ebd451252766801239e63804b59b9a1747764
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966543"
---
# <a name="office365activeusercounts-resource-type"></a>office365ActiveUserCounts 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   | 说明                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | 日期   | 内容的最新日期。          |
| office365         | Int64  | Office 365 中的活动用户数。 此数目包括 Exchange、OneDrive、SharePoint、Skype For Business、Yammer 和 Microsoft 团队中的所有活动用户。 您可以在各自的属性说明中查找每个产品的活动用户的定义。 |
| 汇票          | Int64  | Exchange 中的活动用户数。 任何可以读取和发送电子邮件的用户都被视为活动用户。 |
| For          | Int64  | OneDrive 中的活动用户数。 任何查看或编辑文件、内部或外部共享文件或已同步文件的用户都被视为活动用户。 |
| sharePoint        | Int64  | SharePoint 中的活动用户数。 任何查看或编辑过文件、内部或外部共享文件、同步文件或查看 SharePoint 页面的用户都被视为活动用户。 |
| skypeForBusiness  | Int64  | Skype For Business 中的活动用户数。 任何组织或参加过会议的用户或加入的对等会话都被视为活动用户。 |
| yammer            | Int64  | Yammer 中的活动用户数。 任何可以发布、阅读或赞邮件的用户都被视为活动用户。 |
| 协作             | Int64  | Microsoft 团队中的活动用户数。 任何在团队频道中投递了邮件、在私人聊天会话中发送的邮件或参与会议或呼叫的用户都被视为活动用户。 |
| reportDate        | 日期   | 用户数处于活动状态的日期。 |
| reportPeriod      | String | 报告覆盖的天数。    |

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
