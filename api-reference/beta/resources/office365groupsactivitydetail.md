---
title: office365GroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 0d32d6c44c520f3dd7fe88494da4bfecc0d1ad14
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61863527"
---
# <a name="office365groupsactivitydetail-resource-type"></a>office365GroupsActivityDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>属性

| 属性                          | 类型    | 说明                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| groupId                           | String  | 组 ID。          |
| reportRefreshDate                 | 日期    | 内容的最新日期。          |
| groupDisplayName                  | String  | 组的显示名称。           |
| isDeleted                         | 布尔 | 此用户是已删除还是软删除。 |
| ownerPrincipalName                | String  | 组所有者主体名称。          |
| lastActivityDate                  | 日期    | 以下方案的最后活动日期：组邮箱收到的电子邮件;用户在 SharePoint 文档库中查看、编辑、共享或同步的文件;用户查看的 SharePoint 页面;用户在 Yammer 组中发布、阅读或Yammer消息。 |
| groupType                         | String  | 组类型。 可能的值是 **：Public** 或 **Private**。 |
| memberCount                       | Int64   | 组的成员计数。                  |
| externalMemberCount               | Int64   | 组外部成员计数。         |
| exchangeReceivedEmailCount        | Int64   | 组邮箱收到的电子邮件数。 |
| sharePointActiveFileCount         | Int64   | 组网站中的SharePoint数。 |
| yammerPostedMessageCount          | Int64   | 发送到组的邮件Yammer数量。 |
| yammerReadMessageCount            | Int64   | 在邮件组中读取Yammer数。 |
| yammer在 Yammer的 YamEdMessageCount           | Int64   | 用户组中喜欢的邮件Yammer数量。 |
| exchangeMailboxTotalItemCount     | Int64   | 组邮箱中的项目数。 |
| exchangeMailboxStorageUsedInBytes | Int64   | 组邮箱所使用的存储。   |
| sharePointTotalFileCount          | Int64   | 组网站中的SharePoint总数。 |
| sharePointSiteStorageUsedInBytes  | Int64   | 组网站SharePoint存储。 |
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


