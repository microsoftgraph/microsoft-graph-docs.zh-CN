---
title: provisionedPlan 资源类型
description: 用户 实体和 组织 实体的 **provisionedPlans** 属性都是一个 **provisionedPlan** 集合。
localization_priority: Normal
ms.openlocfilehash: be19bb49409751ae5d7a0f11387e74770fde333b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572547"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="a47f6-103">provisionedPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="a47f6-103">provisionedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a47f6-104">[用户](user.md) 实体和 [组织](organization.md) 实体的 **provisionedPlans** 属性都是一个 **provisionedPlan** 集合。</span><span class="sxs-lookup"><span data-stu-id="a47f6-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="a47f6-105">属性</span><span class="sxs-lookup"><span data-stu-id="a47f6-105">Properties</span></span>
| <span data-ttu-id="a47f6-106">属性</span><span class="sxs-lookup"><span data-stu-id="a47f6-106">Property</span></span>     | <span data-ttu-id="a47f6-107">类型</span><span class="sxs-lookup"><span data-stu-id="a47f6-107">Type</span></span>   |<span data-ttu-id="a47f6-108">说明</span><span class="sxs-lookup"><span data-stu-id="a47f6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a47f6-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="a47f6-109">capabilityStatus</span></span>|<span data-ttu-id="a47f6-110">String</span><span class="sxs-lookup"><span data-stu-id="a47f6-110">String</span></span>|<span data-ttu-id="a47f6-111">例如，“Enabled”。</span><span class="sxs-lookup"><span data-stu-id="a47f6-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="a47f6-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="a47f6-112">provisioningStatus</span></span>|<span data-ttu-id="a47f6-113">String</span><span class="sxs-lookup"><span data-stu-id="a47f6-113">String</span></span>|<span data-ttu-id="a47f6-114">例如，“Success”。</span><span class="sxs-lookup"><span data-stu-id="a47f6-114">For example, “Success”.</span></span>|
|<span data-ttu-id="a47f6-115">service</span><span class="sxs-lookup"><span data-stu-id="a47f6-115">service</span></span>|<span data-ttu-id="a47f6-116">String</span><span class="sxs-lookup"><span data-stu-id="a47f6-116">String</span></span>|<span data-ttu-id="a47f6-117">服务名称；例如，“AccessControlS2S”</span><span class="sxs-lookup"><span data-stu-id="a47f6-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a47f6-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a47f6-118">JSON representation</span></span>

<span data-ttu-id="a47f6-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a47f6-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedPlan"
}-->

```json
{
  "capabilityStatus": "string",
  "provisioningStatus": "string",
  "service": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/provisionedplan.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
