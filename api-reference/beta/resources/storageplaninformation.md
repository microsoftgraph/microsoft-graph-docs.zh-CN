---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
ms.openlocfilehash: 3911d3af5f2149d1043ed246e7c11d287c840842
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342925"
---
# <a name="storageplaninformation-resource-type"></a>storagePlanInformation 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**storagePlanInformation**资源提供有关驱动器的存储配额计划的信息。

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

