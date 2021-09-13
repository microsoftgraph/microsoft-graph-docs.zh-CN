---
title: office365ActiveUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 9f41a0b1fa74c203bfe6b46e9d7ed9788ba46ff5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115133"
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
| deletedDate                       | 日期              | 删除操作发生的日期。 如果用户尚未删除，则默认值为"null"。 |
| hasExchangeLicense                | Boolean           | 用户是否已分配有Exchange许可证。 |
| hasOneDriveLicense                | Boolean           | 是否已为用户分配OneDrive许可证。 |
| hasSharePointLicense              | Boolean           | 是否已为用户分配SharePoint许可证。 |
| hasSkypeForBusinessLicense        | Boolean           | 是否已为用户分配 Skype For Business 许可证。 |
| hasYammerLicense                  | Boolean           | 用户是否已分配有Yammer许可证。 |
| hasTeamsLicense                   | Boolean           | 用户是否已分配有Teams许可证。 |
| exchangeLastActivityDate          | 日期              | 用户上次阅读或发送电子邮件的日期。 |
| oneDriveLastActivityDate          | 日期              | 用户上次查看或编辑文件、在内部或外部共享文件或同步文件的日期。 |
| sharePointLastActivityDate        | 日期              | 用户上次查看或编辑文件、在内部或外部共享文件、同步文件或在页面SharePoint的日期。 |
| skypeForBusinessLastActivityDate  | 日期              | 用户上次组织或参与会议或加入对等会话的日期。 |
| yammerLastActivityDate            | 日期              | 用户上次发布、阅读或点过消息的日期。 |
| teamsLastActivityDate             | 日期              | 用户上次在团队频道中发布消息、在私人聊天会话中发送消息或参与会议或通话的日期。 |
| exchangeLicenseAssignDate         | 日期              | 上次向用户分配许可证Exchange日期。 |
| oneDriveLicenseAssignDate         | 日期              | 上次向用户分配许可证OneDrive日期。 |
| sharePointLicenseAssignDate       | 日期              | 上次向用户分配许可证SharePoint日期。 |
| skypeForBusinessLicenseAssignDate | 日期              | 上次向用户分配企业版Skype的日期。 |
| yammerLicenseAssignDate           | 日期              | 上次向用户分配许可证Yammer日期。 |
| teamsLicenseAssignDate            | 日期              | 上次向用户分配许可证Teams日期。 |
| assignedProducts                  | 字符串集合 | 为用户分配的所有产品。  |

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


