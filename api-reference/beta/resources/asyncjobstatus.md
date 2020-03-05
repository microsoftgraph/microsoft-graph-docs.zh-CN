---
author: JeremyKelley
description: 此资源提供异步作业进度状态的相关信息。
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 81348ce59e060dadf4201222fca43bf96241dbc3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508169"
---
# <a name="asyncjobstatus-resource"></a>AsyncJobStatus 资源

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

此资源提供异步作业进度状态的相关信息。

以下 API 调用返回 **AsyncJobStatus** 资源：

* [复制项](../api/driveitem-copy.md)

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a>属性

| 属性名称          | 类型   | 说明                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| **percentageComplete** | Double | 指明完成百分比的值，介于 0 到 100 之间。                          |
| **status**             | String | 映射到作业状态可能值枚举的字符串值。 |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": []
}
-->
