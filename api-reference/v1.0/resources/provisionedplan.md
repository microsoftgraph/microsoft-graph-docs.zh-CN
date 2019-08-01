---
title: provisionedPlan 资源类型
description: '**用户** 实体和 组织 实体的 provisionedPlans 属性都是一个 **provisionedPlan** 集合。'
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3560aab132448a0d13c4b4abe2590d4802cdf9f3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034991"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="29f40-103">provisionedPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="29f40-103">provisionedPlan resource type</span></span>

<span data-ttu-id="29f40-104">**用户** 实体和 [组织](user.md) 实体的 [provisionedPlans](organization.md) 属性都是一个 **provisionedPlan** 集合。</span><span class="sxs-lookup"><span data-stu-id="29f40-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="29f40-105">属性</span><span class="sxs-lookup"><span data-stu-id="29f40-105">Properties</span></span>
| <span data-ttu-id="29f40-106">属性</span><span class="sxs-lookup"><span data-stu-id="29f40-106">Property</span></span>     | <span data-ttu-id="29f40-107">类型</span><span class="sxs-lookup"><span data-stu-id="29f40-107">Type</span></span>   |<span data-ttu-id="29f40-108">说明</span><span class="sxs-lookup"><span data-stu-id="29f40-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29f40-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="29f40-109">capabilityStatus</span></span>|<span data-ttu-id="29f40-110">String</span><span class="sxs-lookup"><span data-stu-id="29f40-110">String</span></span>|<span data-ttu-id="29f40-111">例如，“Enabled”。</span><span class="sxs-lookup"><span data-stu-id="29f40-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="29f40-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="29f40-112">provisioningStatus</span></span>|<span data-ttu-id="29f40-113">String</span><span class="sxs-lookup"><span data-stu-id="29f40-113">String</span></span>|<span data-ttu-id="29f40-114">例如，“Success”。</span><span class="sxs-lookup"><span data-stu-id="29f40-114">For example, “Success”.</span></span>|
|<span data-ttu-id="29f40-115">service</span><span class="sxs-lookup"><span data-stu-id="29f40-115">service</span></span>|<span data-ttu-id="29f40-116">String</span><span class="sxs-lookup"><span data-stu-id="29f40-116">String</span></span>|<span data-ttu-id="29f40-117">服务名称；例如，“AccessControlS2S”</span><span class="sxs-lookup"><span data-stu-id="29f40-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29f40-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29f40-118">JSON representation</span></span>

<span data-ttu-id="29f40-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29f40-119">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
