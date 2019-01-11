---
title: synchronizationProgress 资源类型
description: 代表完成 synchronizationJob 的进度。
localization_priority: Normal
ms.openlocfilehash: 3c1168cdac6a073842cb5e08d165572591d2d8e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885384"
---
# <a name="synchronizationprogress-resource-type"></a>synchronizationProgress 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表完成[synchronizationJob](synchronization-synchronizationjob.md)的进度。

## <a name="properties"></a>属性

| 属性                              | 类型      | Description    |
|:--------------------------------------|:----------|:---------------|
|completedUnits|Int32|进度比例; 分子已处理的更改的单位数。|
|progressObservationDateTime|DateTimeOffset|进度观察值作为偏移量，以分钟为单位从 UTC 时间。|
|totalUnits|Int32|进度比例; 分母处理以完成同步更改的单位数。|
|单位|字符串|单位的可选说明。|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
}-->

```json
{
  "completedUnits": 1025,
  "progressObservationDateTime": "2017-10-10T17:00:00Z",
  "totalUnits": 3024,
  "units": "pages"
}

```

<!-- uuid: 15571993-7e2f-4842-84d5-01ceb67cdc05
20185-08-14 22:30:00 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
