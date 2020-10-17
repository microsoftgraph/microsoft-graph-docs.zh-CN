---
title: assignedLabel 资源类型
description: 代表分配给 Microsoft 365 组的敏感度标签。
localization_priority: Normal
author: krbain
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 923b616c024a240407161b909baf22ac73d590cc
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581951"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="1be46-103">assignedLabel 资源类型</span><span class="sxs-lookup"><span data-stu-id="1be46-103">assignedLabel resource type</span></span>

<span data-ttu-id="1be46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1be46-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1be46-105">代表分配给 Microsoft 365 组的敏感度标签。</span><span class="sxs-lookup"><span data-stu-id="1be46-105">Represents a sensitivity label assigned to an Microsoft 365 group.</span></span> <span data-ttu-id="1be46-106">通过将分类分配到组 (（如机密、高度机密或常规) ），允许管理员强制组中的特定组设置。</span><span class="sxs-lookup"><span data-stu-id="1be46-106">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="1be46-107">敏感度标签由 Microsoft 365 Security & 合规性中心中的管理员发布，作为 Microsoft 信息保护功能的一部分。</span><span class="sxs-lookup"><span data-stu-id="1be46-107">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="1be46-108">有关敏感度标签的详细信息，请参阅 [敏感度标签概述](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="1be46-108">For more information about sensitivity labels, see [Sensitivity labels overview](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide).</span></span>

## <a name="properties"></a><span data-ttu-id="1be46-109">属性</span><span class="sxs-lookup"><span data-stu-id="1be46-109">Properties</span></span>
| <span data-ttu-id="1be46-110">属性</span><span class="sxs-lookup"><span data-stu-id="1be46-110">Property</span></span>     | <span data-ttu-id="1be46-111">类型</span><span class="sxs-lookup"><span data-stu-id="1be46-111">Type</span></span>   |<span data-ttu-id="1be46-112">说明</span><span class="sxs-lookup"><span data-stu-id="1be46-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1be46-113">labelId</span><span class="sxs-lookup"><span data-stu-id="1be46-113">labelId</span></span>|<span data-ttu-id="1be46-114">字符串</span><span class="sxs-lookup"><span data-stu-id="1be46-114">String</span></span>|<span data-ttu-id="1be46-115">标签的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1be46-115">The unique identifier of the label.</span></span>|
|<span data-ttu-id="1be46-116">displayName</span><span class="sxs-lookup"><span data-stu-id="1be46-116">displayName</span></span>|<span data-ttu-id="1be46-117">字符串</span><span class="sxs-lookup"><span data-stu-id="1be46-117">String</span></span>|<span data-ttu-id="1be46-118">标签的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1be46-118">The display name of the label.</span></span> <span data-ttu-id="1be46-119">只读。</span><span class="sxs-lookup"><span data-stu-id="1be46-119">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1be46-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1be46-120">JSON representation</span></span>

<span data-ttu-id="1be46-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1be46-121">Here is a JSON representation of the resource.</span></span>

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