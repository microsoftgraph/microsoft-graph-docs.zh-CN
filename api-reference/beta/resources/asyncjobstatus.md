---
author: JeremyKelley
description: 此资源提供异步作业进度状态的相关信息。
ms.date: 09/10/2017
title: AsyncJobStatus
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 9dfa9d8422df85f5f0cabb875d855050e4643425
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944981"
---
# <a name="asyncjobstatus-resource"></a>AsyncJobStatus 资源

命名空间：microsoft.graph

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


