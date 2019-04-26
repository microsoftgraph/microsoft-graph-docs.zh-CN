---
title: genericError 资源类型
description: 常规用途的错误。
localization_priority: Normal
ms.openlocfilehash: 314bb5f5e94e44c326fceb71f4a79463989f2129
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333665"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="6fd43-103">genericError 资源类型</span><span class="sxs-lookup"><span data-stu-id="6fd43-103">genericError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fd43-104">常规用途的错误。</span><span class="sxs-lookup"><span data-stu-id="6fd43-104">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="6fd43-105">属性</span><span class="sxs-lookup"><span data-stu-id="6fd43-105">Properties</span></span>

| <span data-ttu-id="6fd43-106">属性</span><span class="sxs-lookup"><span data-stu-id="6fd43-106">Property</span></span> | <span data-ttu-id="6fd43-107">类型</span><span class="sxs-lookup"><span data-stu-id="6fd43-107">Type</span></span> | <span data-ttu-id="6fd43-108">描述</span><span class="sxs-lookup"><span data-stu-id="6fd43-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="6fd43-109">message</span><span class="sxs-lookup"><span data-stu-id="6fd43-109">message</span></span> | <span data-ttu-id="6fd43-110">String</span><span class="sxs-lookup"><span data-stu-id="6fd43-110">String</span></span> | <span data-ttu-id="6fd43-111">错误消息。</span><span class="sxs-lookup"><span data-stu-id="6fd43-111">The error message.</span></span> |
| <span data-ttu-id="6fd43-112">code</span><span class="sxs-lookup"><span data-stu-id="6fd43-112">code</span></span> | <span data-ttu-id="6fd43-113">String</span><span class="sxs-lookup"><span data-stu-id="6fd43-113">String</span></span> | <span data-ttu-id="6fd43-114">错误代码。</span><span class="sxs-lookup"><span data-stu-id="6fd43-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6fd43-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6fd43-115">JSON representation</span></span>

<span data-ttu-id="6fd43-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fd43-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```
