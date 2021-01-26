---
title: office365ActiveUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 057490d5e19a8e56a2e83047277292fbd0af4a16
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980687"
---
# <a name="office365activeuserdetail-resource-type"></a>office365ActiveUserDetail 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性                          | 类型              | 说明                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| reportRefreshDate                 | 日期              | 内容的最新日期。          |
| userPrincipalName                 | String            | 用户的用户主体名称 (UPN)。 UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。 按照惯例，此名称应映射到用户的电子邮件名称。 常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。 创建用户时此属性是必需的。 |
| displayName                       | String            | 用户通讯簿中显示的名称。 这通常是用户名字、中间名首字母和姓氏的组合。 此属性在创建用户时是必需的，并且在更新过程中不能清除。 |
| isDeleted                         | Boolean           | 此用户是已删除还是软删除。 |
| deletedDate                       | 日期              | 执行删除操作的日期。 当用户尚未删除时，默认值为"null"。 |
| hasExchangeLicense                | Boolean           | 是否已为用户分配 Exchange 许可证。 |
| hasOneDriveLicense                | Boolean           | 是否已为用户分配 OneDrive 许可证。 |
| hasSharePointLicense              | Boolean           | 是否已为用户分配 SharePoint 许可证。 |
| hasSkypeForBusinessLicense        | Boolean           | 是否已为用户分配 Skype For Business 许可证。 |
| hasYammerLicense                  | Boolean           | 是否已为用户分配 Yammer 许可证。 |
| hasTeamsLicense                   | Boolean           | 是否已为用户分配 Teams 许可证。 |
| exchangeLastActivityDate          | 日期              | 用户上次阅读或发送电子邮件的日期。 |
| oneDriveLastActivityDate          | 日期              | 用户上次查看或编辑文件、在内部或外部共享文件或同步文件的日期。 |
| sharePointLastActivityDate        | 日期              | 用户上次查看或编辑文件、在内部或外部共享文件、同步文件或查看 SharePoint 页面的日期。 |
| skypeForBusinessLastActivityDate  | 日期              | 用户上次组织或参与会议或加入对等会话的日期。 |
| yammerLastActivityDate            | 日期              | 用户上次发布、阅读或喜欢的邮件的日期。 |
| teamsLastActivityDate             | 日期              | 用户上次在团队频道中发布消息、在私人聊天会话中发送消息或参与会议或通话的日期。 |
| exchangeLicenseAssignDate         | 日期              | 上次为用户分配 Exchange 许可证的日期。 |
| oneDriveLicenseAssignDate         | 日期              | 上次向用户分配 OneDrive 许可证的日期。 |
| sharePointLicenseAssignDate       | 日期              | 上次为用户分配 SharePoint 许可证的日期。 |
| skypeForBusinessLicenseAssignDate | 日期              | 为用户分配 Skype For Business 许可证的最后一个日期。 |
| yammerLicenseAssignDate           | 日期              | 上次为用户分配 Yammer 许可证的日期。 |
| teamsLicenseAssignDate            | 日期              | 上次向用户分配 Teams 许可证的日期。 |
| assignedProducts                  | String collection | 为用户分配的所有产品。  |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "hasExchangeLicense": true, 
  "hasOneDriveLicense": true, 
  "hasSharePointLicense": true, 
  "hasSkypeForBusinessLicense": true, 
  "hasYammerLicense": true, 
  "hasTeamsLicense": true, 
  "exchangeLastActivityDate": "Date", 
  "oneDriveLastActivityDate": "Date", 
  "sharePointLastActivityDate": "Date", 
  "skypeForBusinessLastActivityDate": "Date", 
  "yammerLastActivityDate": "Date", 
  "teamsLastActivityDate": "Date", 
  "exchangeLicenseAssignDate": "Date", 
  "oneDriveLicenseAssignDate": "Date", 
  "sharePointLicenseAssignDate": "Date", 
  "skypeForBusinessLicenseAssignDate": "Date", 
  "yammerLicenseAssignDate": "Date", 
  "teamsLicenseAssignDate": "Date", 
  "assignedProducts": ["String"]
}
```


