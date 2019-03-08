---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: c951aa05b2b0f6f2b036bdf145e161a8d5b52ba7
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482229"
---
# <a name="asyncjobstatus-resource"></a>AsyncJobStatus 资源

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
  "suppressions": [
    "Error: /api-reference/beta/resources/asyncjobstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
