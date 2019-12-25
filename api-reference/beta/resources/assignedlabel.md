---
title: assignedLabel 资源类型
description: 代表分配给 Office 365 组的敏感度标签。 通过将分类（如机密、高度机密或常规）分配给组，允许管理员在组上强制实施特定的组设置。
localization_priority: Normal
author: krbain
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 7e8390ec1773061d447e7526f55e67b87e51531b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870937"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="a4307-104">assignedLabel 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4307-104">assignedLabel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4307-105">代表分配给 Office 365 组的敏感度标签。</span><span class="sxs-lookup"><span data-stu-id="a4307-105">Represents a sensitivity label assigned to an Office 365 group.</span></span> <span data-ttu-id="a4307-106">通过将分类（如机密、高度机密或常规）分配给组，允许管理员在组上强制实施特定的组设置。</span><span class="sxs-lookup"><span data-stu-id="a4307-106">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="a4307-107">敏感度标签由 Microsoft 365 Security & 合规性中心中的管理员发布，作为 Microsoft 信息保护功能的一部分。</span><span class="sxs-lookup"><span data-stu-id="a4307-107">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="a4307-108">有关敏感度标签的详细信息，请参阅[敏感度标签概述](/Office365/SecurityCompliance/sensitivity-labels)。</span><span class="sxs-lookup"><span data-stu-id="a4307-108">For more information about sensitivity labels, see [Sensitivity labels overview](/Office365/SecurityCompliance/sensitivity-labels).</span></span>

## <a name="properties"></a><span data-ttu-id="a4307-109">属性</span><span class="sxs-lookup"><span data-stu-id="a4307-109">Properties</span></span>
| <span data-ttu-id="a4307-110">属性</span><span class="sxs-lookup"><span data-stu-id="a4307-110">Property</span></span>     | <span data-ttu-id="a4307-111">类型</span><span class="sxs-lookup"><span data-stu-id="a4307-111">Type</span></span>   |<span data-ttu-id="a4307-112">说明</span><span class="sxs-lookup"><span data-stu-id="a4307-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4307-113">labelId</span><span class="sxs-lookup"><span data-stu-id="a4307-113">labelId</span></span>|<span data-ttu-id="a4307-114">String</span><span class="sxs-lookup"><span data-stu-id="a4307-114">String</span></span>|<span data-ttu-id="a4307-115">标签的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a4307-115">The unique identifier of the label.</span></span>|
|<span data-ttu-id="a4307-116">displayName</span><span class="sxs-lookup"><span data-stu-id="a4307-116">displayName</span></span>|<span data-ttu-id="a4307-117">String</span><span class="sxs-lookup"><span data-stu-id="a4307-117">String</span></span>|<span data-ttu-id="a4307-118">标签的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a4307-118">The display name of the label.</span></span> <span data-ttu-id="a4307-119">只读。</span><span class="sxs-lookup"><span data-stu-id="a4307-119">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4307-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4307-120">JSON representation</span></span>

<span data-ttu-id="a4307-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4307-121">Here is a JSON representation of the resource.</span></span>

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
