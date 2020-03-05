---
author: psampath
description: StoragePlanInformation 资源提供有关驱动器的存储配额计划的信息。
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 79254efa033528bd8fd4cf66a07959a71e3fef1a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520434"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="bd45f-103">storagePlanInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd45f-103">storagePlanInformation resource type</span></span>

<span data-ttu-id="bd45f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="bd45f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd45f-105">**StoragePlanInformation**资源提供有关驱动器的存储配额计划的信息。</span><span class="sxs-lookup"><span data-stu-id="bd45f-105">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="bd45f-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd45f-106">JSON representation</span></span>

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
## <a name="properties"></a><span data-ttu-id="bd45f-107">属性</span><span class="sxs-lookup"><span data-stu-id="bd45f-107">Properties</span></span>

| <span data-ttu-id="bd45f-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="bd45f-108">Property name</span></span>     | <span data-ttu-id="bd45f-109">类型</span><span class="sxs-lookup"><span data-stu-id="bd45f-109">Type</span></span>      | <span data-ttu-id="bd45f-110">说明</span><span class="sxs-lookup"><span data-stu-id="bd45f-110">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="bd45f-111">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="bd45f-111">upgradeAvailable</span></span>  | <span data-ttu-id="bd45f-112">布尔</span><span class="sxs-lookup"><span data-stu-id="bd45f-112">Boolean</span></span>   | <span data-ttu-id="bd45f-113">指示是否有更高的存储配额计划可用。</span><span class="sxs-lookup"><span data-stu-id="bd45f-113">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="bd45f-114">只读。</span><span class="sxs-lookup"><span data-stu-id="bd45f-114">Read-only.</span></span> |


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

