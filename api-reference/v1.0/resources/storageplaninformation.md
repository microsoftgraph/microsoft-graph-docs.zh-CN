---
author: learafa
description: storagePlanInformation 资源提供有关驱动器的存储配额计划的信息。
title: StoragePlanInformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 0000275139bef3765b7be2e44c26c5e6c12c3e73d04d52b009bfad558081202c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163654"
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


