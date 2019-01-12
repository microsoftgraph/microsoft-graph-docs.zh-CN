---
title: sharePointSiteUsagePages 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1a82c0a1174559db6d90e64f1fd1ed1403caa048
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950443"
---
# <a name="sharepointsiteusagepages-resource-type"></a>sharePointSiteUsagePages 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   |
| :---------------- | :----- |
| reportRefreshDate | 日期   |
| 键入一个文件夹          | 字符串 |
| pageViewCount     | Int64  |
| reportDate        | 日期   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsagePages"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "pageViewCount": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
