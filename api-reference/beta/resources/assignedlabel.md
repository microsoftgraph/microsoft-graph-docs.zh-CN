---
title: assignedLabel 资源类型
description: 代表分配给 Microsoft 365 组的敏感度标签。 通过将分类分配到组 (（如机密、高度机密或常规) ），允许管理员强制组中的特定组设置。
localization_priority: Normal
author: krbain
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 75cfeb74f8844325019c365b0714ae50dcfed063
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352359"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="b02ec-104">assignedLabel 资源类型</span><span class="sxs-lookup"><span data-stu-id="b02ec-104">assignedLabel resource type</span></span>

<span data-ttu-id="b02ec-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b02ec-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b02ec-106">代表分配给 Microsoft 365 组的敏感度标签。</span><span class="sxs-lookup"><span data-stu-id="b02ec-106">Represents a sensitivity label assigned to a Microsoft 365 group.</span></span> <span data-ttu-id="b02ec-107">通过将分类分配到组 (（如机密、高度机密或常规) ），允许管理员强制组中的特定组设置。</span><span class="sxs-lookup"><span data-stu-id="b02ec-107">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="b02ec-108">敏感度标签由 Microsoft 365 Security & 合规性中心中的管理员发布，作为 Microsoft 信息保护功能的一部分。</span><span class="sxs-lookup"><span data-stu-id="b02ec-108">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="b02ec-109">有关敏感度标签的详细信息，请参阅 [敏感度标签概述](/Office365/SecurityCompliance/sensitivity-labels)。</span><span class="sxs-lookup"><span data-stu-id="b02ec-109">For more information about sensitivity labels, see [Sensitivity labels overview](/Office365/SecurityCompliance/sensitivity-labels).</span></span>

## <a name="properties"></a><span data-ttu-id="b02ec-110">属性</span><span class="sxs-lookup"><span data-stu-id="b02ec-110">Properties</span></span>
| <span data-ttu-id="b02ec-111">属性</span><span class="sxs-lookup"><span data-stu-id="b02ec-111">Property</span></span>     | <span data-ttu-id="b02ec-112">类型</span><span class="sxs-lookup"><span data-stu-id="b02ec-112">Type</span></span>   |<span data-ttu-id="b02ec-113">Description</span><span class="sxs-lookup"><span data-stu-id="b02ec-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b02ec-114">labelId</span><span class="sxs-lookup"><span data-stu-id="b02ec-114">labelId</span></span>|<span data-ttu-id="b02ec-115">字符串</span><span class="sxs-lookup"><span data-stu-id="b02ec-115">String</span></span>|<span data-ttu-id="b02ec-116">标签的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b02ec-116">The unique identifier of the label.</span></span>|
|<span data-ttu-id="b02ec-117">displayName</span><span class="sxs-lookup"><span data-stu-id="b02ec-117">displayName</span></span>|<span data-ttu-id="b02ec-118">字符串</span><span class="sxs-lookup"><span data-stu-id="b02ec-118">String</span></span>|<span data-ttu-id="b02ec-119">标签的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b02ec-119">The display name of the label.</span></span> <span data-ttu-id="b02ec-120">只读。</span><span class="sxs-lookup"><span data-stu-id="b02ec-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b02ec-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b02ec-121">JSON representation</span></span>

<span data-ttu-id="b02ec-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b02ec-122">Here is a JSON representation of the resource.</span></span>

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


