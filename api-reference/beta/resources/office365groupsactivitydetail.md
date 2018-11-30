---
title: office365GroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: a849932d646be61f3cedec76ecdafdaca941baaf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042251"
---
# <a name="office365groupsactivitydetail-resource-type"></a>office365GroupsActivityDetail 资源类型

## <a name="properties"></a>属性

| 属性                          | 类型    | 说明                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| reportRefreshDate                 | 日期    | 内容最晚日期。          |
| groupDisplayName                  | 字符串  | 组的显示名称。           |
| 被                         | 布尔 | 此用户是否已被删除或软删除。 |
| ownerPrincipalName                | 字符串  | 组的所有者主体名称。          |
| lastActivityDate                  | 日期    | 以下方案的最后一个活动日期： 组邮箱收到电子邮件;用户可以查看、 编辑、 共享，或同步中 SharePoint 文档库; 文件用户查看 SharePoint 页面; 例如：用户发布、 读取或喜欢 Yammer 组中的邮件。 |
| groupType                         | 字符串  | 组类型。 可能的值为：**公共**或**专用**。 |
| memberCount                       | Int64   | 组成员计数。                  |
| externalMemberCount               | Int64   | 组外部成员计数。         |
| exchangeReceivedEmailCount        | Int64   | 组邮箱收到的电子邮件数。 |
| sharePointActiveFileCount         | Int64   | SharePoint 组网站中的活动文件数。 |
| yammerPostedMessageCount          | Int64   | 发布到 Yammer 组的消息数。 |
| yammerReadMessageCount            | Int64   | Yammer 组中读取的消息数。 |
| yammerLikedMessageCount           | Int64   | 喜欢 Yammer 组中的消息数。 |
| exchangeMailboxTotalItemCount     | Int64   | 组邮箱中的项目数。 |
| exchangeMailboxStorageUsedInBytes | Int64   | 使用的组邮箱的存储。   |
| sharePointTotalFileCount          | Int64   | SharePoint 组网站中的文件总数。 |
| sharePointSiteStorageUsedInBytes  | Int64   | 使用 SharePoint 组网站的存储。 |
| reportPeriod                      | 字符串  | 报告涵盖天数。    |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "memberCount": 1024, 
  "externalMemberCount": 1024, 
  "exchangeReceivedEmailCount": 1024, 
  "sharePointActiveFileCount": 1024, 
  "yammerPostedMessageCount": 1024, 
  "yammerReadMessageCount": 1024, 
  "yammerLikedMessageCount": 1024, 
  "exchangeMailboxTotalItemCount": 1024, 
  "exchangeMailboxStorageUsedInBytes": 1024, 
  "sharePointTotalFileCount": 1024, 
  "sharePointSiteStorageUsedInBytes": 1024, 
  "reportPeriod": "String"
}
```
