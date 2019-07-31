---
author: psampath
description: StoragePlanInformation 资源提供有关驱动器的存储配额计划的信息。
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d8ddb39f9f7c6443f0e669052084af27b8fd5cec
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008080"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="3ecf4-103">storagePlanInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ecf4-103">storagePlanInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ecf4-104">**StoragePlanInformation**资源提供有关驱动器的存储配额计划的信息。</span><span class="sxs-lookup"><span data-stu-id="3ecf4-104">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="3ecf4-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ecf4-105">JSON representation</span></span>

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
## <a name="properties"></a><span data-ttu-id="3ecf4-106">属性</span><span class="sxs-lookup"><span data-stu-id="3ecf4-106">Properties</span></span>

| <span data-ttu-id="3ecf4-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="3ecf4-107">Property name</span></span>     | <span data-ttu-id="3ecf4-108">类型</span><span class="sxs-lookup"><span data-stu-id="3ecf4-108">Type</span></span>      | <span data-ttu-id="3ecf4-109">说明</span><span class="sxs-lookup"><span data-stu-id="3ecf4-109">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="3ecf4-110">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="3ecf4-110">upgradeAvailable</span></span>  | <span data-ttu-id="3ecf4-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ecf4-111">Boolean</span></span>   | <span data-ttu-id="3ecf4-112">指示是否有更高的存储配额计划可用。</span><span class="sxs-lookup"><span data-stu-id="3ecf4-112">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="3ecf4-113">只读。</span><span class="sxs-lookup"><span data-stu-id="3ecf4-113">Read-only.</span></span> |


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

