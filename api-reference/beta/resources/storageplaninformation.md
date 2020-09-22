---
author: psampath
description: StoragePlanInformation 资源提供有关驱动器的存储配额计划的信息。
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4c115276631c67cb796fd06c582dd490d4c59b20
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019472"
---
# <a name="storageplaninformation-resource-type"></a>storagePlanInformation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**StoragePlanInformation**资源提供有关驱动器的存储配额计划的信息。

### <a name="json-representation"></a>JSON 表示形式

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
## <a name="properties"></a>属性

| 属性名称     | 类型      | 说明                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| upgradeAvailable  | Boolean   | 指示是否有更高的存储配额计划可用。 只读。 |


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



