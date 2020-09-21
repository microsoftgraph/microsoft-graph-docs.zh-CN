---
title: licenseDetails 资源类型
description: 包含有关分配给用户的许可证的信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: krbain
ms.openlocfilehash: 5236a73697ea6969698fa0cdb6a8368188d0271c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029195"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="cf9bd-103">licenseDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf9bd-103">licenseDetails resource type</span></span>

<span data-ttu-id="cf9bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf9bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf9bd-105">包含有关分配给用户的许可证的信息。</span><span class="sxs-lookup"><span data-stu-id="cf9bd-105">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="cf9bd-106">方法</span><span class="sxs-lookup"><span data-stu-id="cf9bd-106">Methods</span></span>

| <span data-ttu-id="cf9bd-107">方法</span><span class="sxs-lookup"><span data-stu-id="cf9bd-107">Method</span></span>           | <span data-ttu-id="cf9bd-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="cf9bd-108">Return Type</span></span>    |<span data-ttu-id="cf9bd-109">说明</span><span class="sxs-lookup"><span data-stu-id="cf9bd-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cf9bd-110">List licenseDetails</span><span class="sxs-lookup"><span data-stu-id="cf9bd-110">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="cf9bd-111">licenseDetails 集合</span><span class="sxs-lookup"><span data-stu-id="cf9bd-111">licenseDetails collection</span></span> |<span data-ttu-id="cf9bd-112">检索用户的 licenseDetails 对象列表。</span><span class="sxs-lookup"><span data-stu-id="cf9bd-112">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="cf9bd-113">属性</span><span class="sxs-lookup"><span data-stu-id="cf9bd-113">Properties</span></span>
| <span data-ttu-id="cf9bd-114">属性</span><span class="sxs-lookup"><span data-stu-id="cf9bd-114">Property</span></span>     | <span data-ttu-id="cf9bd-115">类型</span><span class="sxs-lookup"><span data-stu-id="cf9bd-115">Type</span></span>   |<span data-ttu-id="cf9bd-116">说明</span><span class="sxs-lookup"><span data-stu-id="cf9bd-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf9bd-117">id</span><span class="sxs-lookup"><span data-stu-id="cf9bd-117">id</span></span>|<span data-ttu-id="cf9bd-118">String</span><span class="sxs-lookup"><span data-stu-id="cf9bd-118">String</span></span>| <span data-ttu-id="cf9bd-119">许可证详细信息对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cf9bd-119">The unique identifier for the license detail object.</span></span> <span data-ttu-id="cf9bd-120">只读、键、不可为 null</span><span class="sxs-lookup"><span data-stu-id="cf9bd-120">Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="cf9bd-121">servicePlans</span><span class="sxs-lookup"><span data-stu-id="cf9bd-121">servicePlans</span></span>|<span data-ttu-id="cf9bd-122">[servicePlanInfo](serviceplaninfo.md) collection</span><span class="sxs-lookup"><span data-stu-id="cf9bd-122">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="cf9bd-123">有关使用许可证分配的服务计划的信息。</span><span class="sxs-lookup"><span data-stu-id="cf9bd-123">Information about the service plans assigned with the license.</span></span> <span data-ttu-id="cf9bd-124">只读，不可为 null</span><span class="sxs-lookup"><span data-stu-id="cf9bd-124">Read-only, Not nullable</span></span> |
|<span data-ttu-id="cf9bd-125">skuId</span><span class="sxs-lookup"><span data-stu-id="cf9bd-125">skuId</span></span>|<span data-ttu-id="cf9bd-126">Guid</span><span class="sxs-lookup"><span data-stu-id="cf9bd-126">Guid</span></span>| <span data-ttu-id="cf9bd-127">服务 SKU (GUID) 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cf9bd-127">Unique identifier (GUID) for the service SKU.</span></span> <span data-ttu-id="cf9bd-128">等于相关 [SubscribedSku](subscribedsku.md) 对象的 skuId 属性。</span><span class="sxs-lookup"><span data-stu-id="cf9bd-128">Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object.</span></span> <span data-ttu-id="cf9bd-129">只读</span><span class="sxs-lookup"><span data-stu-id="cf9bd-129">Read-only</span></span> |
|<span data-ttu-id="cf9bd-130">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="cf9bd-130">skuPartNumber</span></span>|<span data-ttu-id="cf9bd-131">String</span><span class="sxs-lookup"><span data-stu-id="cf9bd-131">String</span></span>| <span data-ttu-id="cf9bd-132">唯一 SKU 显示名称。</span><span class="sxs-lookup"><span data-stu-id="cf9bd-132">Unique SKU display name.</span></span> <span data-ttu-id="cf9bd-133">等于相关 [SubscribedSku](subscribedsku.md) 对象上的 skuPartNumber;例如： "AAD_Premium"。</span><span class="sxs-lookup"><span data-stu-id="cf9bd-133">Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium".</span></span> <span data-ttu-id="cf9bd-134">只读</span><span class="sxs-lookup"><span data-stu-id="cf9bd-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="cf9bd-135">关系</span><span class="sxs-lookup"><span data-stu-id="cf9bd-135">Relationships</span></span>
<span data-ttu-id="cf9bd-136">无</span><span class="sxs-lookup"><span data-stu-id="cf9bd-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf9bd-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf9bd-137">JSON representation</span></span>
<span data-ttu-id="cf9bd-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf9bd-138">Here is a JSON representation of the resource.</span></span>

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


