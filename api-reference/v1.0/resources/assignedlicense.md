---
title: assignedLicense 资源类型
description: 表示分配给用户的许可证。 User 实体的 **assignedLicenses** 属性是 **assignedLicense**的集合。
localization_priority: Normal
author: krbain
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b7d03a4f6fd9703a3a24900f12b2e522c6535452
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808394"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="b08f9-104">assignedLicense 资源类型</span><span class="sxs-lookup"><span data-stu-id="b08f9-104">assignedLicense resource type</span></span>

<span data-ttu-id="b08f9-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b08f9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b08f9-106">表示分配给用户的许可证。</span><span class="sxs-lookup"><span data-stu-id="b08f9-106">Represents a license assigned to a user.</span></span> <span data-ttu-id="b08f9-107">[User](user.md)实体的**AssignedLicenses**属性是**assignedLicense**的集合。</span><span class="sxs-lookup"><span data-stu-id="b08f9-107">The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="b08f9-108">属性</span><span class="sxs-lookup"><span data-stu-id="b08f9-108">Properties</span></span>
| <span data-ttu-id="b08f9-109">属性</span><span class="sxs-lookup"><span data-stu-id="b08f9-109">Property</span></span>     | <span data-ttu-id="b08f9-110">类型</span><span class="sxs-lookup"><span data-stu-id="b08f9-110">Type</span></span>   |<span data-ttu-id="b08f9-111">说明</span><span class="sxs-lookup"><span data-stu-id="b08f9-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b08f9-112">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="b08f9-112">disabledPlans</span></span>|<span data-ttu-id="b08f9-113">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="b08f9-113">Guid collection</span></span>|<span data-ttu-id="b08f9-114">已禁用的计划的唯一标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="b08f9-114">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="b08f9-115">skuId</span><span class="sxs-lookup"><span data-stu-id="b08f9-115">skuId</span></span>|<span data-ttu-id="b08f9-116">Guid</span><span class="sxs-lookup"><span data-stu-id="b08f9-116">Guid</span></span>|<span data-ttu-id="b08f9-117">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b08f9-117">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b08f9-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b08f9-118">JSON representation</span></span>

<span data-ttu-id="b08f9-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b08f9-119">Here is a JSON representation of the resource</span></span>

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
