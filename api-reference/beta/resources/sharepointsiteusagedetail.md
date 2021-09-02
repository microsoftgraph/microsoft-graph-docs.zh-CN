---
title: sharePointSiteUsageDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 3cfba5694c4f3efc2b10dc9259a561c24ff042af
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820679"
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
| isDeleted               | Boolean |
| lastActivityDate        | 日期    |
| siteSensitivityLabelId  | String  |
| externalSharing         | Boolean |
| unmanagedDevicePolicy   | String  |
| geoLocation             | 字符串  |
| fileCount               | Int64   |
| activeFileCount         | Int64   |
| pageViewCount           | Int64   |
| visitedPageCount        | Int64   |
| anonymousLinkCount      | Int64   |
| companyLinkCount        | Int64   |
| secureLinkForGuestCount | Int64   |
| secureLinkForMemberCount| Int64   |
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
  "siteSensitivityLabelId": "String",
  "externalSharing": true,
  "unmanagedDevicePolicy": "String",
  "geoLocation": "String",
  "fileCount": 1024,
  "activeFileCount": 1024,
  "pageViewCount": 1024,
  "visitedPageCount": 1024,
  "anonymousLinkCount": 5,
  "companyLinkCount": 8,
  "secureLinkForGuestCount": 13,
  "secureLinkForMemberCount": 11,
  "storageUsedInBytes": 1024,
  "storageAllocatedInBytes": 1024,
  "rootWebTemplate": "String",
  "reportPeriod": "String"
}
```


