---
author: psampath
description: storagePlanInformation 资源提供有关驱动器的存储配额计划的信息。
ms.date: 06/20/2018
title: StoragePlanInformation
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 036da4561666bacf12f3cd7a448c9b9ba18808aa
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735941"
---
# <a name="storageplaninformation-resource-type"></a>storagePlanInformation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**storagePlanInformation** 资源提供有关驱动器的存储配额计划的信息。

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

| 属性         | 类型    | 说明                                                             |
| :--------------- | :------ | :---------------------------------------------------------------------- |
| upgradeAvailable | Boolean | 指示是否有更高的存储配额计划可用。 只读。 |

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
