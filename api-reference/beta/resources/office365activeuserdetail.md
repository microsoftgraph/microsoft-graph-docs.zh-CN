---
title: office365ActiveUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 192629623b0a0d46453f4dd4f9bfd7f1dc48cccf
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575368"
---
# <a name="office365activeuserdetail-resource-type"></a>office365ActiveUserDetail 资源类型

## <a name="properties"></a>属性

| 属性                          | 类型              | 说明                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| reportRefreshDate                 | Date              | 内容最晚日期。          |
| userPrincipalName                 | String            | 用户主体名称 (UPN) 的用户。 UPN 是基于 Internet 标准 RFC 822 用户 Internet 风格登录名。 按照惯例，这应映射到用户的电子邮件名称。 常规格式为 alias@domain，域必须存在于中的已验证域的租户的集合。 创建用户时此属性是必需的。 |
| displayName                       | String            | 用户通讯簿中显示的名称。 这通常是用户名字、中间名首字母和姓氏的组合。 此属性在创建用户时是必需的，并且在更新过程中不能清除。 |
| 被                         | 布尔值           | 此用户是否已被删除或软删除。 |
| deletedDate                       | Date              | 删除操作发生的日期。 用户未被删除时，默认值为"null"。 |
| hasExchangeLicense                | 布尔值           | 是否已分配用户的 Exchange 许可证。 |
| hasOneDriveLicense                | 布尔值           | 是否具有已为用户分配 OneDrive 许可证。 |
| hasSharePointLicense              | 布尔值           | 是否具有已为用户分配 SharePoint 许可证。 |
| hasSkypeForBusinessLicense        | 布尔值           | 是否具有已为用户分配 Skype 的业务许可证。 |
| hasYammerLicense                  | 布尔值           | 是否具有已为用户分配 Yammer 许可证。 |
| hasTeamsLicense                   | 布尔值           | 是否具有已为用户分配的工作组许可证。 |
| exchangeLastActivityDate          | Date              | 用户上次读取或发送电子邮件的日期。 |
| oneDriveLastActivityDate          | Date              | 用户上次查看或编辑文件的日期内部或外部，共享文件，或同步文件。 |
| sharePointLastActivityDate        | Date              | 用户上次查看或编辑文件的日期共享文件内部或外部同步文件，或查看 SharePoint 页面。 |
| skypeForBusinessLastActivityDate  | Date              | 当用户上次组织或参加会议，或加入对等会话的日期。 |
| yammerLastActivityDate            | Date              | 当用户上次发布、 读取或喜欢消息日期。 |
| teamsLastActivityDate             | Date              | 当用户上次发布消息团队通道中的日期私人聊天会话中发送的邮件，或参与会议或进行呼叫。 |
| exchangeLicenseAssignDate         | Date              | 用户已分配的 Exchange 许可证的最后一个日期。 |
| oneDriveLicenseAssignDate         | Date              | 用户已分配 OneDrive 许可证的最后一个日期。 |
| sharePointLicenseAssignDate       | Date              | 用户已分配 SharePoint 许可证的最后一个日期。 |
| skypeForBusinessLicenseAssignDate | Date              | 用户已分配的 Skype 的业务许可证的最后一个日期。 |
| yammerLicenseAssignDate           | Date              | 用户已分配的 Yammer 许可证的最后一个日期。 |
| teamsLicenseAssignDate            | Date              | 用户已分配的团队许可证的最后一个日期。 |
| assignedProducts                  | String 集合 | 为用户分配的所有产品。  |

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
