---
title: synchronizationError 资源类型
description: 表示同步过程中发生的错误。
localization_priority: Normal
ms.openlocfilehash: 7f678cdbd48a3d5f013c22120d01c28bb61738e6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324712"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="dc9f9-103">synchronizationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc9f9-103">synchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc9f9-104">表示同步过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="dc9f9-104">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="dc9f9-105">属性</span><span class="sxs-lookup"><span data-stu-id="dc9f9-105">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="dc9f9-106">属性</span><span class="sxs-lookup"><span data-stu-id="dc9f9-106">Property</span></span>     | <span data-ttu-id="dc9f9-107">类型</span><span class="sxs-lookup"><span data-stu-id="dc9f9-107">Type</span></span>   |<span data-ttu-id="dc9f9-108">说明</span><span class="sxs-lookup"><span data-stu-id="dc9f9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc9f9-109">code</span><span class="sxs-lookup"><span data-stu-id="dc9f9-109">code</span></span>|<span data-ttu-id="dc9f9-110">String</span><span class="sxs-lookup"><span data-stu-id="dc9f9-110">String</span></span>||
|<span data-ttu-id="dc9f9-111">message</span><span class="sxs-lookup"><span data-stu-id="dc9f9-111">message</span></span>|<span data-ttu-id="dc9f9-112">String</span><span class="sxs-lookup"><span data-stu-id="dc9f9-112">String</span></span>||
|<span data-ttu-id="dc9f9-113">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="dc9f9-113">tenantActionable</span></span>|<span data-ttu-id="dc9f9-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc9f9-114">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="dc9f9-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc9f9-115">JSON representation</span></span>

<span data-ttu-id="dc9f9-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc9f9-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
