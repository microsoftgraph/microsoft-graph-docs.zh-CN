---
title: assignedLicense 资源类型
description: 表示分配给用户的许可证。 user 实体的**assignedLicenses**属性是**assignedLicense**的集合。
localization_priority: Normal
ms.openlocfilehash: 1e190060d0aafa4d494240f691b354b28e7697c8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569492"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="13b65-104">assignedLicense 资源类型</span><span class="sxs-lookup"><span data-stu-id="13b65-104">assignedLicense resource type</span></span>

<span data-ttu-id="13b65-105">表示分配给用户的许可证。</span><span class="sxs-lookup"><span data-stu-id="13b65-105">Represents a license assigned to a user.</span></span> <span data-ttu-id="13b65-106">[user](user.md)实体的**assignedLicenses**属性是**assignedLicense**的集合。</span><span class="sxs-lookup"><span data-stu-id="13b65-106">The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="13b65-107">属性</span><span class="sxs-lookup"><span data-stu-id="13b65-107">Properties</span></span>
| <span data-ttu-id="13b65-108">属性</span><span class="sxs-lookup"><span data-stu-id="13b65-108">Property</span></span>     | <span data-ttu-id="13b65-109">类型</span><span class="sxs-lookup"><span data-stu-id="13b65-109">Type</span></span>   |<span data-ttu-id="13b65-110">说明</span><span class="sxs-lookup"><span data-stu-id="13b65-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13b65-111">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="13b65-111">disabledPlans</span></span>|<span data-ttu-id="13b65-112">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="13b65-112">Guid collection</span></span>|<span data-ttu-id="13b65-113">已禁用的计划的唯一标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="13b65-113">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="13b65-114">skuId</span><span class="sxs-lookup"><span data-stu-id="13b65-114">skuId</span></span>|<span data-ttu-id="13b65-115">Guid</span><span class="sxs-lookup"><span data-stu-id="13b65-115">Guid</span></span>|<span data-ttu-id="13b65-116">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="13b65-116">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13b65-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13b65-117">JSON representation</span></span>

<span data-ttu-id="13b65-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13b65-118">Here is a JSON representation of the resource</span></span>

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
