---
author: learafa
description: StoragePlanInformation 资源提供有关驱动器的存储配额计划的信息。
title: StoragePlanInformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: b8b4778a4726c227bfe79ad13ecb14507b13a889
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036952"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="67d7e-103">storagePlanInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="67d7e-103">storagePlanInformation resource type</span></span>

<span data-ttu-id="67d7e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67d7e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="67d7e-105">提供有关驱动器的存储配额计划的信息。</span><span class="sxs-lookup"><span data-stu-id="67d7e-105">Provides information about the drive's storage quota plans.</span></span>

## <a name="properties"></a><span data-ttu-id="67d7e-106">属性</span><span class="sxs-lookup"><span data-stu-id="67d7e-106">Properties</span></span>

| <span data-ttu-id="67d7e-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="67d7e-107">Property name</span></span>     | <span data-ttu-id="67d7e-108">类型</span><span class="sxs-lookup"><span data-stu-id="67d7e-108">Type</span></span>      | <span data-ttu-id="67d7e-109">说明</span><span class="sxs-lookup"><span data-stu-id="67d7e-109">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="67d7e-110">**upgradeAvailable**</span><span class="sxs-lookup"><span data-stu-id="67d7e-110">**upgradeAvailable**</span></span>  | <span data-ttu-id="67d7e-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="67d7e-111">Boolean</span></span>   | <span data-ttu-id="67d7e-112">指示是否有更高的存储配额计划可用。</span><span class="sxs-lookup"><span data-stu-id="67d7e-112">Indicates whether there are higher storage quota plans available.</span></span> <span data-ttu-id="67d7e-113">只读。</span><span class="sxs-lookup"><span data-stu-id="67d7e-113">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="67d7e-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67d7e-114">JSON representation</span></span>

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


