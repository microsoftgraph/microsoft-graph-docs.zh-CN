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
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="60a42-102">storagePlanInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="60a42-102">storagePlanInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60a42-103">**storagePlanInformation**资源提供有关驱动器的存储配额计划的信息。</span><span class="sxs-lookup"><span data-stu-id="60a42-103">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="60a42-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60a42-104">JSON representation</span></span>

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
## <a name="properties"></a><span data-ttu-id="60a42-105">属性</span><span class="sxs-lookup"><span data-stu-id="60a42-105">Properties</span></span>

| <span data-ttu-id="60a42-106">属性名称</span><span class="sxs-lookup"><span data-stu-id="60a42-106">Property name</span></span>     | <span data-ttu-id="60a42-107">类型</span><span class="sxs-lookup"><span data-stu-id="60a42-107">Type</span></span>      | <span data-ttu-id="60a42-108">说明</span><span class="sxs-lookup"><span data-stu-id="60a42-108">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="60a42-109">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="60a42-109">upgradeAvailable</span></span>  | <span data-ttu-id="60a42-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="60a42-110">Boolean</span></span>   | <span data-ttu-id="60a42-111">指示是否有更高的存储配额计划可用。</span><span class="sxs-lookup"><span data-stu-id="60a42-111">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="60a42-112">只读。</span><span class="sxs-lookup"><span data-stu-id="60a42-112">Read-only.</span></span> |


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

