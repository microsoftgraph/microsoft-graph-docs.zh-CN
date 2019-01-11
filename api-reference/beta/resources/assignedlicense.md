---
title: assignedLicense 资源类型
description: 表示分配给用户的许可证。用户 实体的 **AssignedLicenses** 属性是一个 **assignedLicense** 集合。
localization_priority: Normal
ms.openlocfilehash: dfb93075fe62a0cfb479e12554e9078e876c4529
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853780"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="2a9b7-104">assignedLicense 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a9b7-104">assignedLicense resource type</span></span>

> <span data-ttu-id="2a9b7-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2a9b7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a9b7-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2a9b7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2a9b7-p103">表示分配给用户的许可证。[用户](user.md) 实体的 **AssignedLicenses** 属性是一个 **assignedLicense** 集合。</span><span class="sxs-lookup"><span data-stu-id="2a9b7-p103">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="2a9b7-109">属性</span><span class="sxs-lookup"><span data-stu-id="2a9b7-109">Properties</span></span>
| <span data-ttu-id="2a9b7-110">属性</span><span class="sxs-lookup"><span data-stu-id="2a9b7-110">Property</span></span>     | <span data-ttu-id="2a9b7-111">类型</span><span class="sxs-lookup"><span data-stu-id="2a9b7-111">Type</span></span>   |<span data-ttu-id="2a9b7-112">说明</span><span class="sxs-lookup"><span data-stu-id="2a9b7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a9b7-113">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="2a9b7-113">disabledPlans</span></span>|<span data-ttu-id="2a9b7-114">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="2a9b7-114">Guid collection</span></span>|<span data-ttu-id="2a9b7-115">已禁用的计划的唯一标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="2a9b7-115">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="2a9b7-116">skuId</span><span class="sxs-lookup"><span data-stu-id="2a9b7-116">skuId</span></span>|<span data-ttu-id="2a9b7-117">Guid</span><span class="sxs-lookup"><span data-stu-id="2a9b7-117">Guid</span></span>|<span data-ttu-id="2a9b7-118">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2a9b7-118">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a9b7-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a9b7-119">JSON representation</span></span>

<span data-ttu-id="2a9b7-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a9b7-120">Here is a JSON representation of the resource</span></span>

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
