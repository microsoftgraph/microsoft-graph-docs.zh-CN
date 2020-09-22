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
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="b2f38-103">storagePlanInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="b2f38-103">storagePlanInformation resource type</span></span>

<span data-ttu-id="b2f38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2f38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2f38-105">**StoragePlanInformation**资源提供有关驱动器的存储配额计划的信息。</span><span class="sxs-lookup"><span data-stu-id="b2f38-105">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="b2f38-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b2f38-106">JSON representation</span></span>

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
## <a name="properties"></a><span data-ttu-id="b2f38-107">属性</span><span class="sxs-lookup"><span data-stu-id="b2f38-107">Properties</span></span>

| <span data-ttu-id="b2f38-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="b2f38-108">Property name</span></span>     | <span data-ttu-id="b2f38-109">类型</span><span class="sxs-lookup"><span data-stu-id="b2f38-109">Type</span></span>      | <span data-ttu-id="b2f38-110">说明</span><span class="sxs-lookup"><span data-stu-id="b2f38-110">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="b2f38-111">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="b2f38-111">upgradeAvailable</span></span>  | <span data-ttu-id="b2f38-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2f38-112">Boolean</span></span>   | <span data-ttu-id="b2f38-113">指示是否有更高的存储配额计划可用。</span><span class="sxs-lookup"><span data-stu-id="b2f38-113">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="b2f38-114">只读。</span><span class="sxs-lookup"><span data-stu-id="b2f38-114">Read-only.</span></span> |


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



