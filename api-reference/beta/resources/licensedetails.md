---
title: licenseDetails 资源类型
description: 包含有关分配给用户的许可证的信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 12e0dcb86288eb27859b87a1029e89676a5d511b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966955"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="d86bd-103">licenseDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="d86bd-103">licenseDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d86bd-104">包含有关分配给用户的许可证的信息。</span><span class="sxs-lookup"><span data-stu-id="d86bd-104">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="d86bd-105">方法</span><span class="sxs-lookup"><span data-stu-id="d86bd-105">Methods</span></span>

| <span data-ttu-id="d86bd-106">方法</span><span class="sxs-lookup"><span data-stu-id="d86bd-106">Method</span></span>           | <span data-ttu-id="d86bd-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="d86bd-107">Return Type</span></span>    |<span data-ttu-id="d86bd-108">说明</span><span class="sxs-lookup"><span data-stu-id="d86bd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d86bd-109">List licenseDetails</span><span class="sxs-lookup"><span data-stu-id="d86bd-109">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="d86bd-110">licenseDetails 集合</span><span class="sxs-lookup"><span data-stu-id="d86bd-110">licenseDetails collection</span></span> |<span data-ttu-id="d86bd-111">检索用户的 licenseDetails 对象列表。</span><span class="sxs-lookup"><span data-stu-id="d86bd-111">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="d86bd-112">属性</span><span class="sxs-lookup"><span data-stu-id="d86bd-112">Properties</span></span>
| <span data-ttu-id="d86bd-113">属性</span><span class="sxs-lookup"><span data-stu-id="d86bd-113">Property</span></span>     | <span data-ttu-id="d86bd-114">类型</span><span class="sxs-lookup"><span data-stu-id="d86bd-114">Type</span></span>   |<span data-ttu-id="d86bd-115">说明</span><span class="sxs-lookup"><span data-stu-id="d86bd-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d86bd-116">id</span><span class="sxs-lookup"><span data-stu-id="d86bd-116">id</span></span>|<span data-ttu-id="d86bd-117">String</span><span class="sxs-lookup"><span data-stu-id="d86bd-117">String</span></span>| <span data-ttu-id="d86bd-118">许可证详细信息对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d86bd-118">The unique identifier for the license detail object.</span></span> <span data-ttu-id="d86bd-119">只读、键、不可为 null</span><span class="sxs-lookup"><span data-stu-id="d86bd-119">Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="d86bd-120">servicePlans</span><span class="sxs-lookup"><span data-stu-id="d86bd-120">servicePlans</span></span>|<span data-ttu-id="d86bd-121">[servicePlanInfo](serviceplaninfo.md) collection</span><span class="sxs-lookup"><span data-stu-id="d86bd-121">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="d86bd-122">有关使用许可证分配的服务计划的信息。</span><span class="sxs-lookup"><span data-stu-id="d86bd-122">Information about the service plans assigned with the license.</span></span> <span data-ttu-id="d86bd-123">只读, 不可为 null</span><span class="sxs-lookup"><span data-stu-id="d86bd-123">Read-only, Not nullable</span></span> |
|<span data-ttu-id="d86bd-124">skuId</span><span class="sxs-lookup"><span data-stu-id="d86bd-124">skuId</span></span>|<span data-ttu-id="d86bd-125">Guid</span><span class="sxs-lookup"><span data-stu-id="d86bd-125">Guid</span></span>| <span data-ttu-id="d86bd-126">服务 SKU 的唯一标识符 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="d86bd-126">Unique identifier (GUID) for the service SKU.</span></span> <span data-ttu-id="d86bd-127">等于相关[SubscribedSku](subscribedsku.md)对象的 skuId 属性。</span><span class="sxs-lookup"><span data-stu-id="d86bd-127">Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object.</span></span> <span data-ttu-id="d86bd-128">只读</span><span class="sxs-lookup"><span data-stu-id="d86bd-128">Read-only</span></span> |
|<span data-ttu-id="d86bd-129">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="d86bd-129">skuPartNumber</span></span>|<span data-ttu-id="d86bd-130">String</span><span class="sxs-lookup"><span data-stu-id="d86bd-130">String</span></span>| <span data-ttu-id="d86bd-131">唯一 SKU 显示名称。</span><span class="sxs-lookup"><span data-stu-id="d86bd-131">Unique SKU display name.</span></span> <span data-ttu-id="d86bd-132">等于相关[SubscribedSku](subscribedsku.md)对象上的 skuPartNumber;例如: "AAD_Premium"。</span><span class="sxs-lookup"><span data-stu-id="d86bd-132">Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium".</span></span> <span data-ttu-id="d86bd-133">只读</span><span class="sxs-lookup"><span data-stu-id="d86bd-133">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="d86bd-134">关系</span><span class="sxs-lookup"><span data-stu-id="d86bd-134">Relationships</span></span>
<span data-ttu-id="d86bd-135">无</span><span class="sxs-lookup"><span data-stu-id="d86bd-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d86bd-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d86bd-136">JSON representation</span></span>
<span data-ttu-id="d86bd-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d86bd-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
