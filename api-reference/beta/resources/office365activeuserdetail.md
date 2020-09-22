---
title: office365ActiveUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 05a47c175e7e9ed6334e691f91556190e459eec0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092417"
---
# <a name="office365activeuserdetail-resource-type"></a>office365ActiveUserDetail 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性                          | 类型              | 说明                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| reportRefreshDate                 | 日期              | 内容的最新日期。          |
| userPrincipalName                 | String            | 用户的用户主体名称 (UPN)。 UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。 按照惯例，此名称应映射到用户的电子邮件名称。 常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。 创建用户时此属性是必需的。 |
| displayName                       | String            | 用户通讯簿中显示的名称。 这通常是用户名字、中间名首字母和姓氏的组合。 此属性在创建用户时是必需的，并且在更新过程中不能清除。 |
| isDeleted                         | 布尔           | 此用户是否已被删除或软删除。 |
| deletedDate                       | 日期              | 删除操作发生的日期。 当用户未被删除时，默认值为 "null"。 |
| hasExchangeLicense                | 布尔           | 是否已为用户分配了 Exchange 许可证。 |
| hasOneDriveLicense                | 布尔           | 是否已为用户分配 OneDrive 许可证。 |
| hasSharePointLicense              | 布尔           | 是否已为用户分配 SharePoint 许可证。 |
| hasSkypeForBusinessLicense        | 布尔           | 是否已为用户分配 Skype For Business 许可证。 |
| hasYammerLicense                  | 布尔           | 是否为用户分配了 Yammer 许可证。 |
| hasTeamsLicense                   | 布尔           | 是否已向用户分配团队许可证。 |
| exchangeLastActivityDate          | 日期              | 用户最后一次阅读或发送电子邮件的日期。 |
| oneDriveLastActivityDate          | 日期              | 用户上次查看或编辑文件、内部或外部共享文件或同步文件的日期。 |
| sharePointLastActivityDate        | 日期              | 用户上次查看或编辑文件、内部或外部共享文件、同步文件或查看 SharePoint 页面的日期。 |
| skypeForBusinessLastActivityDate  | 日期              | 用户最后一次组织或参与会议的日期，或加入的对等会话。 |
| yammerLastActivityDate            | 日期              | 用户上次发布、阅读或赞邮件的日期。 |
| teamsLastActivityDate             | 日期              | 用户上次在团队频道中发布的邮件，在私人聊天会话中发送的邮件，或参与会议或呼叫的日期。 |
| exchangeLicenseAssignDate         | 日期              | 向用户分配 Exchange 许可证的最后日期。 |
| oneDriveLicenseAssignDate         | 日期              | 向用户分配 OneDrive 许可证的最后日期。 |
| sharePointLicenseAssignDate       | 日期              | 向用户分配 SharePoint 许可证的最后日期。 |
| skypeForBusinessLicenseAssignDate | 日期              | 为用户分配 Skype For Business 许可证的最后一个日期。 |
| yammerLicenseAssignDate           | 日期              | 向用户分配 Yammer 许可证的最后日期。 |
| teamsLicenseAssignDate            | 日期              | 向用户分配团队许可证的最后日期。 |
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


