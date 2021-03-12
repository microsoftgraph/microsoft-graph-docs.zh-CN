---
title: assignedLabel 资源类型
description: 表示分配给 Microsoft 365 组的敏感度标签。
localization_priority: Normal
author: jpettere
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 9602e10dda5d558110c55f1fb4ee166e53187989
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720891"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="00fdd-103">assignedLabel 资源类型</span><span class="sxs-lookup"><span data-stu-id="00fdd-103">assignedLabel resource type</span></span>

<span data-ttu-id="00fdd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00fdd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="00fdd-105">表示分配给 Microsoft 365 组的敏感度标签。</span><span class="sxs-lookup"><span data-stu-id="00fdd-105">Represents a sensitivity label assigned to an Microsoft 365 group.</span></span> <span data-ttu-id="00fdd-106">敏感度标签允许管理员通过向组分配分类（如"机密 (高度机密"或"常规"策略）对组强制执行特定) 。</span><span class="sxs-lookup"><span data-stu-id="00fdd-106">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="00fdd-107">敏感度标签由 Microsoft 365 安全与合规& Microsoft 信息保护功能的一部分发布。</span><span class="sxs-lookup"><span data-stu-id="00fdd-107">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="00fdd-108">有关敏感度标签详细信息，请参阅敏感度 [标签概述](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="00fdd-108">For more information about sensitivity labels, see [Sensitivity labels overview](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide).</span></span>

## <a name="properties"></a><span data-ttu-id="00fdd-109">属性</span><span class="sxs-lookup"><span data-stu-id="00fdd-109">Properties</span></span>
| <span data-ttu-id="00fdd-110">属性</span><span class="sxs-lookup"><span data-stu-id="00fdd-110">Property</span></span>     | <span data-ttu-id="00fdd-111">类型</span><span class="sxs-lookup"><span data-stu-id="00fdd-111">Type</span></span>   |<span data-ttu-id="00fdd-112">说明</span><span class="sxs-lookup"><span data-stu-id="00fdd-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00fdd-113">labelId</span><span class="sxs-lookup"><span data-stu-id="00fdd-113">labelId</span></span>|<span data-ttu-id="00fdd-114">字符串</span><span class="sxs-lookup"><span data-stu-id="00fdd-114">String</span></span>|<span data-ttu-id="00fdd-115">标签的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="00fdd-115">The unique identifier of the label.</span></span>|
|<span data-ttu-id="00fdd-116">displayName</span><span class="sxs-lookup"><span data-stu-id="00fdd-116">displayName</span></span>|<span data-ttu-id="00fdd-117">字符串</span><span class="sxs-lookup"><span data-stu-id="00fdd-117">String</span></span>|<span data-ttu-id="00fdd-118">标签显示名称。</span><span class="sxs-lookup"><span data-stu-id="00fdd-118">The display name of the label.</span></span> <span data-ttu-id="00fdd-119">只读。</span><span class="sxs-lookup"><span data-stu-id="00fdd-119">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00fdd-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00fdd-120">JSON representation</span></span>

<span data-ttu-id="00fdd-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00fdd-121">Here is a JSON representation of the resource.</span></span>

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