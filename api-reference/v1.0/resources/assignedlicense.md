---
title: assignedLicense 资源类型
description: 表示分配给用户的许可证。用户 实体的 **AssignedLicenses** 属性是一个 **assignedLicense** 集合。
ms.openlocfilehash: 48863a9acdcfa173a3f0c1a2a008516360ffdf9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008768"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="0efe2-104">assignedLicense 资源类型</span><span class="sxs-lookup"><span data-stu-id="0efe2-104">assignedLicense resource type</span></span>

<span data-ttu-id="0efe2-p102">表示分配给用户的许可证。[用户](user.md) 实体的 **AssignedLicenses** 属性是一个 **assignedLicense** 集合。</span><span class="sxs-lookup"><span data-stu-id="0efe2-p102">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="0efe2-107">属性</span><span class="sxs-lookup"><span data-stu-id="0efe2-107">Properties</span></span>
| <span data-ttu-id="0efe2-108">属性</span><span class="sxs-lookup"><span data-stu-id="0efe2-108">Property</span></span>     | <span data-ttu-id="0efe2-109">类型</span><span class="sxs-lookup"><span data-stu-id="0efe2-109">Type</span></span>   |<span data-ttu-id="0efe2-110">说明</span><span class="sxs-lookup"><span data-stu-id="0efe2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0efe2-111">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="0efe2-111">disabledPlans</span></span>|<span data-ttu-id="0efe2-112">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="0efe2-112">Guid collection</span></span>|<span data-ttu-id="0efe2-113">已禁用的计划的唯一标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="0efe2-113">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="0efe2-114">skuId</span><span class="sxs-lookup"><span data-stu-id="0efe2-114">skuId</span></span>|<span data-ttu-id="0efe2-115">Guid</span><span class="sxs-lookup"><span data-stu-id="0efe2-115">Guid</span></span>|<span data-ttu-id="0efe2-116">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0efe2-116">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0efe2-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0efe2-117">JSON representation</span></span>

<span data-ttu-id="0efe2-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0efe2-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
