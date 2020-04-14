---
title: mailboxUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 636417b5ec299bb11f82c406abecdebe72ee45de
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473413"
---
# <a name="mailboxusagestorage-resource-type"></a>mailboxUsageStorage 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性           | 类型   |
| :----------------- | :----- |
| reportRefreshDate  | 日期   |
| storageUsedInBytes | Int64  |
| reportDate         | 日期   |
| reportPeriod       | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
