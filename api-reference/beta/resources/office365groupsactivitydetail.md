---
title: office365GroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: fe2df5614525f27b294bed93be7f3f9cd8170b30
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981506"
---
# <a name="office365groupsactivitydetail-resource-type"></a>office365GroupsActivityDetail 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性                          | 类型    | 说明                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| groupId                           | String  | 组 ID。          |
| reportRefreshDate                 | 日期    | 内容的最新日期。          |
| groupDisplayName                  | String  | 组的显示名称。           |
| isDeleted                         | Boolean | 此用户是已删除还是软删除。 |
| ownerPrincipalName                | String  | 组所有者主体名称。          |
| lastActivityDate                  | 日期    | 以下方案的最后一个活动日期：组邮箱收到电子邮件;用户在 SharePoint 文档库中查看、编辑、共享或同步的文件;用户查看的 SharePoint 页面;用户发布、阅读或喜欢的 Yammer 组中的消息。 |
| groupType                         | String  | 组类型。 可能的值是 **：Public** 或 **Private。** |
| memberCount                       | Int64   | 组的成员计数。                  |
| externalMemberCount               | Int64   | 组外部成员计数。         |
| exchangeReceivedEmailCount        | Int64   | 组邮箱接收的电子邮件数。 |
| sharePointActiveFileCount         | Int64   | SharePoint 组网站中的活动文件数。 |
| yammerPostedMessageCount          | Int64   | 张贴到 Yammer 组的消息数。 |
| yammerReadMessageCount            | Int64   | Yammer 组中读取的消息数。 |
| yammer已用MessageCount           | Int64   | Yammer 组中喜欢的消息数。 |
| exchangeMailboxTotalItemCount     | Int64   | 组邮箱中的项目数。 |
| exchangeMailboxStorageUsedInBytes | Int64   | 组邮箱所使用的存储。   |
| sharePointTotalFileCount          | Int64   | SharePoint 组网站中的文件总数。 |
| sharePointSiteStorageUsedInBytes  | Int64   | SharePoint 组网站所使用的存储。 |
| reportPeriod                      | String  | 报告涵盖的天数。    |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
  "groupId": "0003cf63-7ff3-4471-b24b-50ffbfb8b5d2",
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


