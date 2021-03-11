---
title: assignedLabel 资源类型
description: 表示分配给 Microsoft 365 组的敏感度标签。 敏感度标签允许管理员通过向组分配分类（如机密、高度机密或常规 (）来强制实施组的特定组) 。
localization_priority: Normal
author: jpettere
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 7c71e59c022eb9a3314771598b47e938a61a946a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720345"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="e1d57-104">assignedLabel 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1d57-104">assignedLabel resource type</span></span>

<span data-ttu-id="e1d57-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1d57-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1d57-106">表示分配给 Microsoft 365 组的敏感度标签。</span><span class="sxs-lookup"><span data-stu-id="e1d57-106">Represents a sensitivity label assigned to a Microsoft 365 group.</span></span> <span data-ttu-id="e1d57-107">敏感度标签允许管理员通过向组分配分类（如机密、高度机密或常规 (）来强制实施组的特定组) 。</span><span class="sxs-lookup"><span data-stu-id="e1d57-107">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="e1d57-108">敏感度标签由 Microsoft 365 安全与合规& Microsoft 信息保护功能的一部分发布。</span><span class="sxs-lookup"><span data-stu-id="e1d57-108">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="e1d57-109">有关敏感度标签详细信息，请参阅 [敏感度标签概述](/Office365/SecurityCompliance/sensitivity-labels)。</span><span class="sxs-lookup"><span data-stu-id="e1d57-109">For more information about sensitivity labels, see [Sensitivity labels overview](/Office365/SecurityCompliance/sensitivity-labels).</span></span>

## <a name="properties"></a><span data-ttu-id="e1d57-110">属性</span><span class="sxs-lookup"><span data-stu-id="e1d57-110">Properties</span></span>
| <span data-ttu-id="e1d57-111">属性</span><span class="sxs-lookup"><span data-stu-id="e1d57-111">Property</span></span>     | <span data-ttu-id="e1d57-112">类型</span><span class="sxs-lookup"><span data-stu-id="e1d57-112">Type</span></span>   |<span data-ttu-id="e1d57-113">说明</span><span class="sxs-lookup"><span data-stu-id="e1d57-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1d57-114">labelId</span><span class="sxs-lookup"><span data-stu-id="e1d57-114">labelId</span></span>|<span data-ttu-id="e1d57-115">String</span><span class="sxs-lookup"><span data-stu-id="e1d57-115">String</span></span>|<span data-ttu-id="e1d57-116">标签的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e1d57-116">The unique identifier of the label.</span></span>|
|<span data-ttu-id="e1d57-117">displayName</span><span class="sxs-lookup"><span data-stu-id="e1d57-117">displayName</span></span>|<span data-ttu-id="e1d57-118">String</span><span class="sxs-lookup"><span data-stu-id="e1d57-118">String</span></span>|<span data-ttu-id="e1d57-119">标签显示名称。</span><span class="sxs-lookup"><span data-stu-id="e1d57-119">The display name of the label.</span></span> <span data-ttu-id="e1d57-120">只读。</span><span class="sxs-lookup"><span data-stu-id="e1d57-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1d57-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1d57-121">JSON representation</span></span>

<span data-ttu-id="e1d57-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1d57-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLabel"
}-->

```json
{
  "labelId": "String",
  "displayName": "String"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


