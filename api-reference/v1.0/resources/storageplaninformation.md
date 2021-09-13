---
author: learafa
description: storagePlanInformation 资源提供有关驱动器的存储配额计划的信息。
title: StoragePlanInformation
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: a26704495253d9dd33f4bcb37395b927ca8a4342
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136325"
---
# <a name="storageplaninformation-resource-type"></a>storagePlanInformation 资源类型

命名空间：microsoft.graph

提供有关驱动器的存储配额计划的信息。

## <a name="properties"></a>属性

| 属性名称     | 类型      | 说明                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| **upgradeAvailable**  | Boolean   | 指示是否有更高的存储配额计划可用。 只读。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
   "@odata.type": "microsoft.graph.storagePlanInformation",
} -->

```json
{
  "upgradeAvailable": true
}

```

<!--
{
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation",
  "suppressions": []
}
-->


