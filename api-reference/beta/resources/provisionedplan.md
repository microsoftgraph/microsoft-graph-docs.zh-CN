---
title: provisionedPlan 资源类型
description: '**用户** 实体和 组织 实体的 provisionedPlans 属性都是一个 **provisionedPlan** 集合。'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 78ce5deac88c07a5f180c972d80a7c8e8798cab8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521346"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="025cd-103">provisionedPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="025cd-103">provisionedPlan resource type</span></span>

<span data-ttu-id="025cd-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="025cd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="025cd-105">**用户** 实体和 [组织](user.md) 实体的 [provisionedPlans](organization.md) 属性都是一个 **provisionedPlan** 集合。</span><span class="sxs-lookup"><span data-stu-id="025cd-105">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="025cd-106">属性</span><span class="sxs-lookup"><span data-stu-id="025cd-106">Properties</span></span>
| <span data-ttu-id="025cd-107">属性</span><span class="sxs-lookup"><span data-stu-id="025cd-107">Property</span></span>     | <span data-ttu-id="025cd-108">类型</span><span class="sxs-lookup"><span data-stu-id="025cd-108">Type</span></span>   |<span data-ttu-id="025cd-109">说明</span><span class="sxs-lookup"><span data-stu-id="025cd-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="025cd-110">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="025cd-110">capabilityStatus</span></span>|<span data-ttu-id="025cd-111">String</span><span class="sxs-lookup"><span data-stu-id="025cd-111">String</span></span>|<span data-ttu-id="025cd-112">例如，“Enabled”。</span><span class="sxs-lookup"><span data-stu-id="025cd-112">For example, “Enabled”.</span></span>|
|<span data-ttu-id="025cd-113">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="025cd-113">provisioningStatus</span></span>|<span data-ttu-id="025cd-114">String</span><span class="sxs-lookup"><span data-stu-id="025cd-114">String</span></span>|<span data-ttu-id="025cd-115">例如，“Success”。</span><span class="sxs-lookup"><span data-stu-id="025cd-115">For example, “Success”.</span></span>|
|<span data-ttu-id="025cd-116">service</span><span class="sxs-lookup"><span data-stu-id="025cd-116">service</span></span>|<span data-ttu-id="025cd-117">String</span><span class="sxs-lookup"><span data-stu-id="025cd-117">String</span></span>|<span data-ttu-id="025cd-118">服务名称；例如，“AccessControlS2S”</span><span class="sxs-lookup"><span data-stu-id="025cd-118">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="025cd-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="025cd-119">JSON representation</span></span>

<span data-ttu-id="025cd-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="025cd-120">Here is a JSON representation of the resource</span></span>

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
