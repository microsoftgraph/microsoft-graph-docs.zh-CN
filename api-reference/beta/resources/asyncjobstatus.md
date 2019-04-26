---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: 74ead4ca8e45c5baebe3ea74377ce102d9e2ee88
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328645"
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
  "suppressions": []
}
-->
