---
title: office365GroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 176e960c7d9ae8dd1bc29600ad7b64e45e2940fa
ms.sourcegitcommit: 6fe086e6a9396a71a82179853547cb7b5e22d980
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/20/2019
ms.locfileid: "35805212"
---
# <a name="office365groupsactivitydetail-resource-type"></a>office365GroupsActivityDetail 资源类型

## <a name="properties"></a>属性

| 属性                          | 类型    | 说明                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| groupId                           | String  | 组 id。          |
| reportRefreshDate                 | 日期    | 内容的最新日期。          |
| groupDisplayName                  | String  | 组的显示名称。           |
| isDeleted                         | Boolean | 此用户是否已被删除或软删除。 |
| ownerPrincipalName                | String  | 组所有者的主体名称。          |
| lastActivityDate                  | 日期    | 以下应用场景的上次活动日期: 组邮箱收到电子邮件;用户在 SharePoint 文档库中查看、编辑、共享或同步文件;用户查看了 SharePoint 页面;用户在 Yammer 组中投递、阅读或赞了邮件。 |
| groupType                         | String  | 组类型。 可能的值是: **Public**或**Private**。 |
| memberCount                       | Int64   | 组成员计数。                  |
| externalMemberCount               | Int64   | Group 外部成员计数。         |
| exchangeReceivedEmailCount        | Int64   | 组邮箱接收的电子邮件数。 |
| sharePointActiveFileCount         | Int64   | SharePoint 组网站中的活动文件数。 |
| yammerPostedMessageCount          | Int64   | 发布到 Yammer 组的邮件数。 |
| yammerReadMessageCount            | Int64   | Yammer 组中读取的邮件数。 |
| yammerLikedMessageCount           | Int64   | Yammer 组中的已赞邮件数。 |
| exchangeMailboxTotalItemCount     | Int64   | 组邮箱中的项目数。 |
| exchangeMailboxStorageUsedInBytes | Int64   | 组邮箱所使用的存储。   |
| sharePointTotalFileCount          | Int64   | SharePoint 组网站中的总文件数。 |
| sharePointSiteStorageUsedInBytes  | Int64   | SharePoint 组网站所使用的存储区。 |
| reportPeriod                      | String  | 报告覆盖的天数。    |

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
