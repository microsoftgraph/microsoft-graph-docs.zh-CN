---
title: provisionedPlan 资源类型
description: '**用户** 实体和 组织 实体的 provisionedPlans 属性都是一个 **provisionedPlan** 集合。'
localization_priority: Normal
ms.openlocfilehash: 1d6bec5cdcd4caaf8990caac6614f2fa589d4c4c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344020"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="e877a-103">provisionedPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="e877a-103">provisionedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e877a-104">**用户** 实体和 [组织](user.md) 实体的 [provisionedPlans](organization.md) 属性都是一个 **provisionedPlan** 集合。</span><span class="sxs-lookup"><span data-stu-id="e877a-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="e877a-105">属性</span><span class="sxs-lookup"><span data-stu-id="e877a-105">Properties</span></span>
| <span data-ttu-id="e877a-106">属性</span><span class="sxs-lookup"><span data-stu-id="e877a-106">Property</span></span>     | <span data-ttu-id="e877a-107">类型</span><span class="sxs-lookup"><span data-stu-id="e877a-107">Type</span></span>   |<span data-ttu-id="e877a-108">说明</span><span class="sxs-lookup"><span data-stu-id="e877a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e877a-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="e877a-109">capabilityStatus</span></span>|<span data-ttu-id="e877a-110">String</span><span class="sxs-lookup"><span data-stu-id="e877a-110">String</span></span>|<span data-ttu-id="e877a-111">例如，“Enabled”。</span><span class="sxs-lookup"><span data-stu-id="e877a-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="e877a-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="e877a-112">provisioningStatus</span></span>|<span data-ttu-id="e877a-113">String</span><span class="sxs-lookup"><span data-stu-id="e877a-113">String</span></span>|<span data-ttu-id="e877a-114">例如，“Success”。</span><span class="sxs-lookup"><span data-stu-id="e877a-114">For example, “Success”.</span></span>|
|<span data-ttu-id="e877a-115">service</span><span class="sxs-lookup"><span data-stu-id="e877a-115">service</span></span>|<span data-ttu-id="e877a-116">String</span><span class="sxs-lookup"><span data-stu-id="e877a-116">String</span></span>|<span data-ttu-id="e877a-117">服务名称；例如，“AccessControlS2S”</span><span class="sxs-lookup"><span data-stu-id="e877a-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e877a-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e877a-118">JSON representation</span></span>

<span data-ttu-id="e877a-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e877a-119">Here is a JSON representation of the resource</span></span>

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
  "suppressions": []
}
-->
