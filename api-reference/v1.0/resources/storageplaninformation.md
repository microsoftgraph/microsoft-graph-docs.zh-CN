---
author: learafa
description: StoragePlanInformation 资源提供有关驱动器的存储配额计划的信息。
title: StoragePlanInformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: a5e6c10bdbc8a68230a223501844d0ee121014c2
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863773"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="9a276-103">storagePlanInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a276-103">storagePlanInformation resource type</span></span>

<span data-ttu-id="9a276-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a276-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9a276-105">提供有关驱动器的存储配额计划的信息。</span><span class="sxs-lookup"><span data-stu-id="9a276-105">Provides information about the drive's storage quota plans.</span></span>

## <a name="properties"></a><span data-ttu-id="9a276-106">属性</span><span class="sxs-lookup"><span data-stu-id="9a276-106">Properties</span></span>

| <span data-ttu-id="9a276-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="9a276-107">Property name</span></span>     | <span data-ttu-id="9a276-108">类型</span><span class="sxs-lookup"><span data-stu-id="9a276-108">Type</span></span>      | <span data-ttu-id="9a276-109">说明</span><span class="sxs-lookup"><span data-stu-id="9a276-109">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="9a276-110">**upgradeAvailable**</span><span class="sxs-lookup"><span data-stu-id="9a276-110">**upgradeAvailable**</span></span>  | <span data-ttu-id="9a276-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a276-111">Boolean</span></span>   | <span data-ttu-id="9a276-112">指示是否有更高的存储配额计划可用。</span><span class="sxs-lookup"><span data-stu-id="9a276-112">Indicates whether there are higher storage quota plans available.</span></span> <span data-ttu-id="9a276-113">只读。</span><span class="sxs-lookup"><span data-stu-id="9a276-113">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9a276-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a276-114">JSON representation</span></span>

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

