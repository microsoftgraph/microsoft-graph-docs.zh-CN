---
title: licenseDetails 资源类型
description: 包含有关分配给用户的许可证的信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9bdf5456cd0e807ca2a2eaaef8f1d0eab302f23c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522972"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="7e525-103">licenseDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e525-103">licenseDetails resource type</span></span>

<span data-ttu-id="7e525-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7e525-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e525-105">包含有关分配给用户的许可证的信息。</span><span class="sxs-lookup"><span data-stu-id="7e525-105">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="7e525-106">方法</span><span class="sxs-lookup"><span data-stu-id="7e525-106">Methods</span></span>

| <span data-ttu-id="7e525-107">方法</span><span class="sxs-lookup"><span data-stu-id="7e525-107">Method</span></span>           | <span data-ttu-id="7e525-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="7e525-108">Return Type</span></span>    |<span data-ttu-id="7e525-109">说明</span><span class="sxs-lookup"><span data-stu-id="7e525-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7e525-110">List licenseDetails</span><span class="sxs-lookup"><span data-stu-id="7e525-110">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="7e525-111">licenseDetails 集合</span><span class="sxs-lookup"><span data-stu-id="7e525-111">licenseDetails collection</span></span> |<span data-ttu-id="7e525-112">检索用户的 licenseDetails 对象列表。</span><span class="sxs-lookup"><span data-stu-id="7e525-112">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="7e525-113">属性</span><span class="sxs-lookup"><span data-stu-id="7e525-113">Properties</span></span>
| <span data-ttu-id="7e525-114">属性</span><span class="sxs-lookup"><span data-stu-id="7e525-114">Property</span></span>     | <span data-ttu-id="7e525-115">类型</span><span class="sxs-lookup"><span data-stu-id="7e525-115">Type</span></span>   |<span data-ttu-id="7e525-116">说明</span><span class="sxs-lookup"><span data-stu-id="7e525-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e525-117">id</span><span class="sxs-lookup"><span data-stu-id="7e525-117">id</span></span>|<span data-ttu-id="7e525-118">String</span><span class="sxs-lookup"><span data-stu-id="7e525-118">String</span></span>| <span data-ttu-id="7e525-119">许可证详细信息对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7e525-119">The unique identifier for the license detail object.</span></span> <span data-ttu-id="7e525-120">只读、键、不可为 null</span><span class="sxs-lookup"><span data-stu-id="7e525-120">Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="7e525-121">servicePlans</span><span class="sxs-lookup"><span data-stu-id="7e525-121">servicePlans</span></span>|<span data-ttu-id="7e525-122">[servicePlanInfo](serviceplaninfo.md) collection</span><span class="sxs-lookup"><span data-stu-id="7e525-122">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="7e525-123">有关使用许可证分配的服务计划的信息。</span><span class="sxs-lookup"><span data-stu-id="7e525-123">Information about the service plans assigned with the license.</span></span> <span data-ttu-id="7e525-124">只读，不可为 null</span><span class="sxs-lookup"><span data-stu-id="7e525-124">Read-only, Not nullable</span></span> |
|<span data-ttu-id="7e525-125">skuId</span><span class="sxs-lookup"><span data-stu-id="7e525-125">skuId</span></span>|<span data-ttu-id="7e525-126">Guid</span><span class="sxs-lookup"><span data-stu-id="7e525-126">Guid</span></span>| <span data-ttu-id="7e525-127">服务 SKU 的唯一标识符（GUID）。</span><span class="sxs-lookup"><span data-stu-id="7e525-127">Unique identifier (GUID) for the service SKU.</span></span> <span data-ttu-id="7e525-128">等于相关[SubscribedSku](subscribedsku.md)对象的 skuId 属性。</span><span class="sxs-lookup"><span data-stu-id="7e525-128">Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object.</span></span> <span data-ttu-id="7e525-129">只读</span><span class="sxs-lookup"><span data-stu-id="7e525-129">Read-only</span></span> |
|<span data-ttu-id="7e525-130">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="7e525-130">skuPartNumber</span></span>|<span data-ttu-id="7e525-131">String</span><span class="sxs-lookup"><span data-stu-id="7e525-131">String</span></span>| <span data-ttu-id="7e525-132">唯一 SKU 显示名称。</span><span class="sxs-lookup"><span data-stu-id="7e525-132">Unique SKU display name.</span></span> <span data-ttu-id="7e525-133">等于相关[SubscribedSku](subscribedsku.md)对象上的 skuPartNumber;例如： "AAD_Premium"。</span><span class="sxs-lookup"><span data-stu-id="7e525-133">Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium".</span></span> <span data-ttu-id="7e525-134">只读</span><span class="sxs-lookup"><span data-stu-id="7e525-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="7e525-135">关系</span><span class="sxs-lookup"><span data-stu-id="7e525-135">Relationships</span></span>
<span data-ttu-id="7e525-136">无</span><span class="sxs-lookup"><span data-stu-id="7e525-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e525-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e525-137">JSON representation</span></span>
<span data-ttu-id="7e525-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e525-138">Here is a JSON representation of the resource.</span></span>

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
