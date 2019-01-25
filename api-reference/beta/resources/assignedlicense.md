---
title: assignedLicense 资源类型
description: 表示分配给用户的许可证。**用户** 实体的 **AssignedLicenses** 属性是一个 assignedLicense 集合。
localization_priority: Normal
ms.openlocfilehash: 2d9620ec33a296c09ced9bc9d8af8d6d032bb7d9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524917"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="a60b9-104">assignedLicense 资源类型</span><span class="sxs-lookup"><span data-stu-id="a60b9-104">assignedLicense resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a60b9-p102">表示分配给用户的许可证。[用户](user.md) 实体的 **AssignedLicenses** 属性是一个 **assignedLicense** 集合。</span><span class="sxs-lookup"><span data-stu-id="a60b9-p102">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="a60b9-107">属性</span><span class="sxs-lookup"><span data-stu-id="a60b9-107">Properties</span></span>
| <span data-ttu-id="a60b9-108">属性</span><span class="sxs-lookup"><span data-stu-id="a60b9-108">Property</span></span>     | <span data-ttu-id="a60b9-109">类型</span><span class="sxs-lookup"><span data-stu-id="a60b9-109">Type</span></span>   |<span data-ttu-id="a60b9-110">说明</span><span class="sxs-lookup"><span data-stu-id="a60b9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a60b9-111">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="a60b9-111">disabledPlans</span></span>|<span data-ttu-id="a60b9-112">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="a60b9-112">Guid collection</span></span>|<span data-ttu-id="a60b9-113">已禁用的计划的唯一标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="a60b9-113">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="a60b9-114">skuId</span><span class="sxs-lookup"><span data-stu-id="a60b9-114">skuId</span></span>|<span data-ttu-id="a60b9-115">Guid</span><span class="sxs-lookup"><span data-stu-id="a60b9-115">Guid</span></span>|<span data-ttu-id="a60b9-116">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a60b9-116">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a60b9-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a60b9-117">JSON representation</span></span>

<span data-ttu-id="a60b9-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a60b9-118">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/assignedlicense.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
