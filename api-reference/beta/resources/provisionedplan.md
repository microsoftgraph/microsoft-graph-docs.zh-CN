---
title: provisionedPlan 资源类型
description: '**用户** 实体和 组织 实体的 provisionedPlans 属性都是一个 **provisionedPlan** 集合。'
localization_priority: Normal
ms.openlocfilehash: 5f9d9c5b2dfffb86643c5e355799f46382bc38cd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563310"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="227f3-103">provisionedPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="227f3-103">provisionedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="227f3-104">**用户** 实体和 [组织](user.md) 实体的 [provisionedPlans](organization.md) 属性都是一个 **provisionedPlan** 集合。</span><span class="sxs-lookup"><span data-stu-id="227f3-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="227f3-105">属性</span><span class="sxs-lookup"><span data-stu-id="227f3-105">Properties</span></span>
| <span data-ttu-id="227f3-106">属性</span><span class="sxs-lookup"><span data-stu-id="227f3-106">Property</span></span>     | <span data-ttu-id="227f3-107">类型</span><span class="sxs-lookup"><span data-stu-id="227f3-107">Type</span></span>   |<span data-ttu-id="227f3-108">说明</span><span class="sxs-lookup"><span data-stu-id="227f3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="227f3-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="227f3-109">capabilityStatus</span></span>|<span data-ttu-id="227f3-110">String</span><span class="sxs-lookup"><span data-stu-id="227f3-110">String</span></span>|<span data-ttu-id="227f3-111">例如，“Enabled”。</span><span class="sxs-lookup"><span data-stu-id="227f3-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="227f3-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="227f3-112">provisioningStatus</span></span>|<span data-ttu-id="227f3-113">String</span><span class="sxs-lookup"><span data-stu-id="227f3-113">String</span></span>|<span data-ttu-id="227f3-114">例如，“Success”。</span><span class="sxs-lookup"><span data-stu-id="227f3-114">For example, “Success”.</span></span>|
|<span data-ttu-id="227f3-115">service</span><span class="sxs-lookup"><span data-stu-id="227f3-115">service</span></span>|<span data-ttu-id="227f3-116">String</span><span class="sxs-lookup"><span data-stu-id="227f3-116">String</span></span>|<span data-ttu-id="227f3-117">服务名称；例如，“AccessControlS2S”</span><span class="sxs-lookup"><span data-stu-id="227f3-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="227f3-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="227f3-118">JSON representation</span></span>

<span data-ttu-id="227f3-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="227f3-119">Here is a JSON representation of the resource</span></span>

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
