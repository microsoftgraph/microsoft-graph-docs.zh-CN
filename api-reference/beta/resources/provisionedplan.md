---
title: provisionedPlan 资源类型
description: 用户 实体和 组织 实体的 **provisionedPlans** 属性都是一个 **provisionedPlan** 集合。
localization_priority: Normal
ms.openlocfilehash: 5f9d9c5b2dfffb86643c5e355799f46382bc38cd
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643368"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="06576-103">provisionedPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="06576-103">provisionedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06576-104">[用户](user.md) 实体和 [组织](organization.md) 实体的 **provisionedPlans** 属性都是一个 **provisionedPlan** 集合。</span><span class="sxs-lookup"><span data-stu-id="06576-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="06576-105">属性</span><span class="sxs-lookup"><span data-stu-id="06576-105">Properties</span></span>
| <span data-ttu-id="06576-106">属性</span><span class="sxs-lookup"><span data-stu-id="06576-106">Property</span></span>     | <span data-ttu-id="06576-107">类型</span><span class="sxs-lookup"><span data-stu-id="06576-107">Type</span></span>   |<span data-ttu-id="06576-108">说明</span><span class="sxs-lookup"><span data-stu-id="06576-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06576-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="06576-109">capabilityStatus</span></span>|<span data-ttu-id="06576-110">String</span><span class="sxs-lookup"><span data-stu-id="06576-110">String</span></span>|<span data-ttu-id="06576-111">例如，“Enabled”。</span><span class="sxs-lookup"><span data-stu-id="06576-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="06576-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="06576-112">provisioningStatus</span></span>|<span data-ttu-id="06576-113">String</span><span class="sxs-lookup"><span data-stu-id="06576-113">String</span></span>|<span data-ttu-id="06576-114">例如，“Success”。</span><span class="sxs-lookup"><span data-stu-id="06576-114">For example, “Success”.</span></span>|
|<span data-ttu-id="06576-115">service</span><span class="sxs-lookup"><span data-stu-id="06576-115">service</span></span>|<span data-ttu-id="06576-116">String</span><span class="sxs-lookup"><span data-stu-id="06576-116">String</span></span>|<span data-ttu-id="06576-117">服务名称；例如，“AccessControlS2S”</span><span class="sxs-lookup"><span data-stu-id="06576-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06576-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06576-118">JSON representation</span></span>

<span data-ttu-id="06576-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06576-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedplan"
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
