---
title: sharePointSiteUsageDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: f8f06cf9fcf1dfc01af3e98c01a79a86426e19ee
ms.sourcegitcommit: 1b01c820be659f85f380fc883bbb36036b7daadf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2021
ms.locfileid: "50115218"
---
# <a name="sharepointsiteusagedetail-resource-type"></a>sharePointSiteUsageDetail 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性                | 类型    |
| :---------------------- | :------ |
| reportRefreshDate       | 日期    |
| siteId                  | Guid  |
| siteUrl                 | String  |
| ownerDisplayName        | String  |
| ownerPrincipalName      | String  |
| isDeleted               | 布尔 |
| lastActivityDate        | 日期    |
| SiteSensitivityLabelId  | String  |
| ExternalSharing         | 布尔 |
| UnmanagedDevicePolicy   | String  |
| GeoLocation             | String  |
| fileCount               | Int64   |
| activeFileCount         | Int64   |
| pageViewCount           | Int64   |
| visitedPageCount        | Int64   |
| AnonymousLinkCount      | Int64   |
| CompanyLinkCount        | Int64   |
| SecureLinkForGuestCount | Int64   |
| SecureLinkForMemberCount| Int64   |
| storageUsedInBytes      | Int64   |
| storageAllocatedInBytes | Int64   |
| rootWebTemplate         | String  |
| reportPeriod            | String  |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date",
  "siteId": "Guid",
  "siteUrl": "String",
  "ownerDisplayName": "String",
  "ownerPrincipalName": "String",
  "isDeleted": true,
  "lastActivityDate": "Date",
  "lastActivityDate": "2017-09-01", 
  "SiteSensitivityLabelId": "String",
  "ExternalSharing": true,
  "UnmanagedDevicePolicy": "String",
  "GeoLocation": "String",
  "fileCount": 1024,
  "activeFileCount": 1024,
  "pageViewCount": 1024,
  "visitedPageCount": 1024,
  "AnonymousLinkCount": 5,
  "CompanyLinkCount": 8,
  "SecureLinkForGuestCount": 13,
  "SecureLinkForMemberCount": 11,
  "storageUsedInBytes": 1024,
  "storageAllocatedInBytes": 1024,
  "rootWebTemplate": "String",
  "reportPeriod": "String"
}
```


