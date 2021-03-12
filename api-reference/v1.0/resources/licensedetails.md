---
title: licenseDetails 资源类型
description: 包含有关分配给用户的许可证的信息。
localization_priority: Normal
author: jpettere
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 64bc8532e399be729c85200ca66b2f6e99b95084
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722228"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="da9e6-103">licenseDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="da9e6-103">licenseDetails resource type</span></span>

<span data-ttu-id="da9e6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da9e6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da9e6-105">包含有关分配给用户的许可证的信息。</span><span class="sxs-lookup"><span data-stu-id="da9e6-105">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="da9e6-106">Methods</span><span class="sxs-lookup"><span data-stu-id="da9e6-106">Methods</span></span>

| <span data-ttu-id="da9e6-107">方法</span><span class="sxs-lookup"><span data-stu-id="da9e6-107">Method</span></span>           | <span data-ttu-id="da9e6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="da9e6-108">Return Type</span></span>    |<span data-ttu-id="da9e6-109">说明</span><span class="sxs-lookup"><span data-stu-id="da9e6-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="da9e6-110">List licenseDetails</span><span class="sxs-lookup"><span data-stu-id="da9e6-110">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="da9e6-111">licenseDetails 集合</span><span class="sxs-lookup"><span data-stu-id="da9e6-111">licenseDetails collection</span></span> |<span data-ttu-id="da9e6-112">检索用户的 licenseDetails 对象列表。</span><span class="sxs-lookup"><span data-stu-id="da9e6-112">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="da9e6-113">属性</span><span class="sxs-lookup"><span data-stu-id="da9e6-113">Properties</span></span>
| <span data-ttu-id="da9e6-114">属性</span><span class="sxs-lookup"><span data-stu-id="da9e6-114">Property</span></span>     | <span data-ttu-id="da9e6-115">类型</span><span class="sxs-lookup"><span data-stu-id="da9e6-115">Type</span></span>   |<span data-ttu-id="da9e6-116">说明</span><span class="sxs-lookup"><span data-stu-id="da9e6-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da9e6-117">id</span><span class="sxs-lookup"><span data-stu-id="da9e6-117">id</span></span>|<span data-ttu-id="da9e6-118">字符串</span><span class="sxs-lookup"><span data-stu-id="da9e6-118">String</span></span>| <span data-ttu-id="da9e6-119">许可证详细信息对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="da9e6-119">The unique identifier for the license detail object.</span></span> <span data-ttu-id="da9e6-120">只读、键、不可为 null</span><span class="sxs-lookup"><span data-stu-id="da9e6-120">Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="da9e6-121">servicePlans</span><span class="sxs-lookup"><span data-stu-id="da9e6-121">servicePlans</span></span>|<span data-ttu-id="da9e6-122">[servicePlanInfo](serviceplaninfo.md) collection</span><span class="sxs-lookup"><span data-stu-id="da9e6-122">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="da9e6-123">有关随许可证分配的服务计划的信息。</span><span class="sxs-lookup"><span data-stu-id="da9e6-123">Information about the service plans assigned with the license.</span></span> <span data-ttu-id="da9e6-124">只读，不可为 null</span><span class="sxs-lookup"><span data-stu-id="da9e6-124">Read-only, Not nullable</span></span> |
|<span data-ttu-id="da9e6-125">skuId</span><span class="sxs-lookup"><span data-stu-id="da9e6-125">skuId</span></span>|<span data-ttu-id="da9e6-126">Guid</span><span class="sxs-lookup"><span data-stu-id="da9e6-126">Guid</span></span>| <span data-ttu-id="da9e6-127">服务 SKU (GUID) 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="da9e6-127">Unique identifier (GUID) for the service SKU.</span></span> <span data-ttu-id="da9e6-128">等于相关 [SubscribedSku](subscribedsku.md) 对象的 skuId 属性。</span><span class="sxs-lookup"><span data-stu-id="da9e6-128">Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object.</span></span> <span data-ttu-id="da9e6-129">只读</span><span class="sxs-lookup"><span data-stu-id="da9e6-129">Read-only</span></span> |
|<span data-ttu-id="da9e6-130">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="da9e6-130">skuPartNumber</span></span>|<span data-ttu-id="da9e6-131">String</span><span class="sxs-lookup"><span data-stu-id="da9e6-131">String</span></span>| <span data-ttu-id="da9e6-132">唯一 SKU 显示名称。</span><span class="sxs-lookup"><span data-stu-id="da9e6-132">Unique SKU display name.</span></span> <span data-ttu-id="da9e6-133">等于相关 [SubscribedSku](subscribedsku.md) 对象上的 skuPartNumber;例如："AAD_Premium"。</span><span class="sxs-lookup"><span data-stu-id="da9e6-133">Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium".</span></span> <span data-ttu-id="da9e6-134">只读</span><span class="sxs-lookup"><span data-stu-id="da9e6-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="da9e6-135">关系</span><span class="sxs-lookup"><span data-stu-id="da9e6-135">Relationships</span></span>
<span data-ttu-id="da9e6-136">无</span><span class="sxs-lookup"><span data-stu-id="da9e6-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da9e6-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da9e6-137">JSON representation</span></span>
<span data-ttu-id="da9e6-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da9e6-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

