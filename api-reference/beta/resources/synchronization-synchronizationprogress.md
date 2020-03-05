---
title: synchronizationProgress 资源类型
description: 表示 synchronizationJob 的进度向完成。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4fb5fb9482a9b8523f1967928a4243a5b104f6a0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520056"
---
# <a name="synchronizationprogress-resource-type"></a>synchronizationProgress 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示[synchronizationJob](synchronization-synchronizationjob.md)的进度向完成。

## <a name="properties"></a>属性

| 属性                              | 类型      | 说明    |
|:--------------------------------------|:----------|:---------------|
|completedUnits|Int32|进度比率的分子;已处理的更改的单位数。|
|progressObservationDateTime|DateTimeOffset|进度观察的时间，作为从 UTC 的偏移量（以分钟为单位）。|
|totalUnits|Int32|进度比率的分母;要处理的用于完成同步的更改的多个单元。|
|units|String|单位的可选说明。|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationProgress"
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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
