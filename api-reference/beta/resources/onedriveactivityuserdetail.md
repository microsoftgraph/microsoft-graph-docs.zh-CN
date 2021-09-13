---
title: oneDriveActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 89b6cd03e4f4b4876806ca0588073b98e3c235c7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59085887"
---
# <a name="onedriveactivityuserdetail-resource-type"></a>oneDriveActivityUserDetail 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性                  | 类型              |
| :------------------------ | :---------------- |
| reportRefreshDate         | 日期              |
| userPrincipalName         | String            |
| isDeleted                 | Boolean           |
| deletedDate               | 日期              |
| lastActivityDate          | 日期              |
| viewedOrEditedFileCount   | Int64             |
| syncedFileCount           | Int64             |
| sharedInternallyFileCount | Int64             |
| sharedExternallyFileCount | Int64             |
| assignedProducts          | 字符串集合 |
| reportPeriod              | String            |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date",
  "userPrincipalName": "String",
  "isDeleted": true,
  "deletedDate": "Date",
  "lastActivityDate": "Date",
  "viewedOrEditedFileCount": 1024,
  "syncedFileCount": 1024,
  "sharedInternallyFileCount": 1024,
  "sharedExternallyFileCount": 1024,
  "assignedProducts": ["String"],
  "reportPeriod": "String"
}
```


