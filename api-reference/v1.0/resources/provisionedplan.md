---
title: provisionedPlan 资源类型
description: '**用户** 实体和 组织 实体的 provisionedPlans 属性都是一个 **provisionedPlan** 集合。'
localization_priority: Normal
author: Jumaodhiss
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6b8236a6948b0941cfe3c6f304a037c8cfc41a7e
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469421"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="45c13-103">provisionedPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="45c13-103">provisionedPlan resource type</span></span>

<span data-ttu-id="45c13-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45c13-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="45c13-105">**用户** 实体和 [组织](user.md) 实体的 [provisionedPlans](organization.md) 属性都是一个 **provisionedPlan** 集合。</span><span class="sxs-lookup"><span data-stu-id="45c13-105">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="45c13-106">属性</span><span class="sxs-lookup"><span data-stu-id="45c13-106">Properties</span></span>
| <span data-ttu-id="45c13-107">属性</span><span class="sxs-lookup"><span data-stu-id="45c13-107">Property</span></span>     | <span data-ttu-id="45c13-108">类型</span><span class="sxs-lookup"><span data-stu-id="45c13-108">Type</span></span>   |<span data-ttu-id="45c13-109">说明</span><span class="sxs-lookup"><span data-stu-id="45c13-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45c13-110">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="45c13-110">capabilityStatus</span></span>|<span data-ttu-id="45c13-111">String</span><span class="sxs-lookup"><span data-stu-id="45c13-111">String</span></span>|<span data-ttu-id="45c13-112">例如，“Enabled”。</span><span class="sxs-lookup"><span data-stu-id="45c13-112">For example, “Enabled”.</span></span>|
|<span data-ttu-id="45c13-113">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="45c13-113">provisioningStatus</span></span>|<span data-ttu-id="45c13-114">String</span><span class="sxs-lookup"><span data-stu-id="45c13-114">String</span></span>|<span data-ttu-id="45c13-115">例如，“Success”。</span><span class="sxs-lookup"><span data-stu-id="45c13-115">For example, “Success”.</span></span>|
|<span data-ttu-id="45c13-116">service</span><span class="sxs-lookup"><span data-stu-id="45c13-116">service</span></span>|<span data-ttu-id="45c13-117">String</span><span class="sxs-lookup"><span data-stu-id="45c13-117">String</span></span>|<span data-ttu-id="45c13-118">服务名称；例如，“AccessControlS2S”</span><span class="sxs-lookup"><span data-stu-id="45c13-118">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45c13-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45c13-119">JSON representation</span></span>

<span data-ttu-id="45c13-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45c13-120">Here is a JSON representation of the resource</span></span>

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

