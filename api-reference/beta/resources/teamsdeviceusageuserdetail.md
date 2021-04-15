---
title: teamsDeviceUsageUserDetail 资源类型
description: 表示有关用户 Microsoft Teams 设备使用情况的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 294ffee8a1a5db208508cce230377285d6834b07
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766054"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>teamsDeviceUsageUserDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关用户 Microsoft Teams 设备使用情况的详细信息。

## <a name="properties"></a>属性

| 属性          | 类型    | 说明                                                  |
| :---------------- | :------ | ------------------------------------------------------------ |
| reportRefreshDate | 日期    | 内容的最新日期。                              |
| userPrincipalName | String  | 用户的用户主体名称 (UPN)。 UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。 按照惯例，此名称应映射到用户的电子邮件名称。 常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。 创建用户时此属性是必需的。 |
| isLicensed        | Boolean | 是否已为用户分配 Teams 许可证。          |
| lastActivityDate  | 日期    | 用户上次参与 Microsoft Teams 活动的日期。 |
| isDeleted         | Boolean | 此用户是已删除还是软删除。          |
| deletedDate       | 日期    | 删除操作发生的日期。 如果用户尚未删除，则默认值为"null"。 |
| usedWeb           | Boolean | 用户是否在设备的 Teams Web 客户端中处于活动状态。 |
| usedWindowsPhone  | Boolean | 用户是否在适用于 Windows Phone 的 Teams 移动客户端上处于活动状态。 |
| usediOS           | Boolean | 用户是否在适用于 iOS 的 Teams 移动客户端上处于活动状态。 |
| usedMac           | Boolean | 用户是否在 macOS 计算机的 Teams 桌面客户端中处于活动状态。 |
| usedAndroidPhone  | Boolean | 用户是否在适用于 Android 的 Teams 移动客户端上处于活动状态。 |
| usedWindows       | Boolean | 用户是否在基于 Windows 的计算机的 Teams 桌面客户端中处于活动状态。 |
| usedChromeOS      | Boolean | 用户是否在 ChromeOS 计算机的 Teams 桌面客户端中处于活动状态。 |
| used 过         | Boolean | 用户在 Linux 计算机的 Teams 桌面客户端中是否处于活动状态。 |
| reportPeriod      | String  | 报告涵盖的天数。                        |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isLicensed": true, 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "usedChromeOS": true, 
  "usedLinux": true, 
  "reportPeriod": "String"
}
```


