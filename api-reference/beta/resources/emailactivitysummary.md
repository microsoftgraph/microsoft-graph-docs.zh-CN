---
title: emailActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
ms.localizationpriority: medium
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ae2c1d52ab736106f9f76ef07b93b09db4de4d94
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129297"
---
# <a name="emailactivitysummary-resource-type"></a>emailActivitySummary 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性          | 类型   |
| :---------------- | :----- |
| reportRefreshDate | 日期   |
| 发送              | Int64  |
| receive           | Int64  |
| 阅读              | Int64  |
| reportDate        | 日期   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


