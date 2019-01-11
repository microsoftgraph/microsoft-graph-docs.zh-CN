---
title: office365ActiveUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 887f9b08d7f46aac023fbd0f34e6174e5f422760
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882717"
---
# <a name="office365activeusercounts-resource-type"></a>office365ActiveUserCounts 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   | Description                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | 日期   | 内容最晚日期。          |
| office365         | Int64  | Office 365 中的活动用户数。 此数值包括 Exchange、 OneDrive、 SharePoint、 Skype 的业务、 Yammer，和 Microsoft 团队中的所有活动的用户。 您可以找到各自属性说明中的每个产品的活动用户定义。 |
| exchange          | Int64  | Exchange 中的活动用户数。 任何用户都可以读取和发送电子邮件被视为活动用户。 |
| oneDrive          | Int64  | OneDrive 中的活动用户数。 查看或编辑文件、 内部或外部，共享文件或同步文件的任何用户被视为活动用户。 |
| sharePoint        | Int64  | 在 SharePoint 中的活动用户数。 查看或编辑文件、 共享文件内部或外部同步文件，或查看 SharePoint 页的任何用户被视为活动用户。 |
| skypeForBusiness  | Int64  | Skype 的企业中的活动用户数。 组织或参加会议，或加入对等会话的任何用户被视为活动用户。 |
| yammer            | Int64  | Yammer 中的活动用户数。 任何用户都可以发布、 读取或类似于邮件被视为活动用户。 |
| 团队             | Int64  | 在 Microsoft 团队中的活动用户数。 在工作组通道中发布消息、 私人聊天会话中发送的邮件或参加会议或进行呼叫的任何用户被视为活动用户。 |
| reportDate        | 日期   | 多个用户在其处于活动状态日期。 |
| reportPeriod      | 字符串 | 报告涵盖天数。    |

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
