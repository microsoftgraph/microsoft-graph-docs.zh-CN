---
title: synchronizationProgress 资源类型
description: 表示 synchronizationJob 的进度向完成。
localization_priority: Normal
ms.openlocfilehash: b22bd95f54a9f268524dc98a8d3df94fcc14f773
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453955"
---
# <a name="synchronizationprogress-resource-type"></a>synchronizationProgress 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示[synchronizationJob](synchronization-synchronizationjob.md)的进度向完成。

## <a name="properties"></a>属性

| 属性                              | 类型      | 描述    |
|:--------------------------------------|:----------|:---------------|
|completedUnits|Int32|进度比率的分子;已处理的更改的单位数。|
|progressObservationDateTime|DateTimeOffset|进度观察的时间, 作为从 UTC 的偏移量 (以分钟为单位)。|
|totalUnits|Int32|进度比率的分母;要处理的用于完成同步的更改的多个单元。|
|units|字符串|单位的可选说明。|

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationprogress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
