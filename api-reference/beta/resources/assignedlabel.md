---
title: assignedLabel 资源类型
description: 代表分配给 Office 365 组的敏感度标签。 通过将分类 (如机密、高度机密或常规) 分配给组, 允许管理员在组上强制实施特定的组设置。
localization_priority: Normal
author: krbain
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 118a8a85a8abb68f59438db9024952d16f7a279c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013288"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="c13fb-104">assignedLabel 资源类型</span><span class="sxs-lookup"><span data-stu-id="c13fb-104">assignedLabel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c13fb-105">代表分配给 Office 365 组的敏感度标签。</span><span class="sxs-lookup"><span data-stu-id="c13fb-105">Represents a sensitivity label assigned to an Office 365 group.</span></span> <span data-ttu-id="c13fb-106">通过将分类 (如机密、高度机密或常规) 分配给组, 允许管理员在组上强制实施特定的组设置。</span><span class="sxs-lookup"><span data-stu-id="c13fb-106">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="c13fb-107">敏感度标签由 Microsoft 365 Security & 合规性中心中的管理员发布, 作为 Microsoft 信息保护功能的一部分。</span><span class="sxs-lookup"><span data-stu-id="c13fb-107">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="c13fb-108">有关敏感度标签的详细信息, 请参阅[敏感度标签概述](https://docs.microsoft.com/en-us/Office365/SecurityCompliance/sensitivity-labels)。</span><span class="sxs-lookup"><span data-stu-id="c13fb-108">For more information about sensitivity labels, see [Sensitivity labels overview](https://docs.microsoft.com/en-us/Office365/SecurityCompliance/sensitivity-labels).</span></span>

## <a name="properties"></a><span data-ttu-id="c13fb-109">属性</span><span class="sxs-lookup"><span data-stu-id="c13fb-109">Properties</span></span>
| <span data-ttu-id="c13fb-110">属性</span><span class="sxs-lookup"><span data-stu-id="c13fb-110">Property</span></span>     | <span data-ttu-id="c13fb-111">类型</span><span class="sxs-lookup"><span data-stu-id="c13fb-111">Type</span></span>   |<span data-ttu-id="c13fb-112">说明</span><span class="sxs-lookup"><span data-stu-id="c13fb-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c13fb-113">labelId</span><span class="sxs-lookup"><span data-stu-id="c13fb-113">labelId</span></span>|<span data-ttu-id="c13fb-114">String</span><span class="sxs-lookup"><span data-stu-id="c13fb-114">String</span></span>|<span data-ttu-id="c13fb-115">标签的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c13fb-115">The unique identifier of the label.</span></span>|
|<span data-ttu-id="c13fb-116">displayName</span><span class="sxs-lookup"><span data-stu-id="c13fb-116">displayName</span></span>|<span data-ttu-id="c13fb-117">String</span><span class="sxs-lookup"><span data-stu-id="c13fb-117">String</span></span>|<span data-ttu-id="c13fb-118">标签的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c13fb-118">The display name of the label.</span></span> <span data-ttu-id="c13fb-119">只读。</span><span class="sxs-lookup"><span data-stu-id="c13fb-119">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c13fb-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c13fb-120">JSON representation</span></span>

<span data-ttu-id="c13fb-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c13fb-121">Here is a JSON representation of the resource.</span></span>

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
