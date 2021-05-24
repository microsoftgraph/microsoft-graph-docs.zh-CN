---
title: licenseDetails 资源类型
description: 包含有关分配给用户的许可证的信息。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 4e23dfcd15dc2b05a9d1c7356a532e6faf487662
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547188"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="37642-103">licenseDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="37642-103">licenseDetails resource type</span></span>

<span data-ttu-id="37642-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37642-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37642-105">包含有关分配给用户的许可证的信息。</span><span class="sxs-lookup"><span data-stu-id="37642-105">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="37642-106">方法</span><span class="sxs-lookup"><span data-stu-id="37642-106">Methods</span></span>

| <span data-ttu-id="37642-107">方法</span><span class="sxs-lookup"><span data-stu-id="37642-107">Method</span></span>           | <span data-ttu-id="37642-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="37642-108">Return Type</span></span>    |<span data-ttu-id="37642-109">说明</span><span class="sxs-lookup"><span data-stu-id="37642-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="37642-110">List licenseDetails</span><span class="sxs-lookup"><span data-stu-id="37642-110">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="37642-111">licenseDetails 集合</span><span class="sxs-lookup"><span data-stu-id="37642-111">licenseDetails collection</span></span> |<span data-ttu-id="37642-112">检索用户的 licenseDetails 对象列表。</span><span class="sxs-lookup"><span data-stu-id="37642-112">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="37642-113">属性</span><span class="sxs-lookup"><span data-stu-id="37642-113">Properties</span></span>
| <span data-ttu-id="37642-114">属性</span><span class="sxs-lookup"><span data-stu-id="37642-114">Property</span></span>     | <span data-ttu-id="37642-115">类型</span><span class="sxs-lookup"><span data-stu-id="37642-115">Type</span></span>   |<span data-ttu-id="37642-116">说明</span><span class="sxs-lookup"><span data-stu-id="37642-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37642-117">id</span><span class="sxs-lookup"><span data-stu-id="37642-117">id</span></span>|<span data-ttu-id="37642-118">字符串</span><span class="sxs-lookup"><span data-stu-id="37642-118">String</span></span>| <span data-ttu-id="37642-119">许可证详细信息对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="37642-119">The unique identifier for the license detail object.</span></span> <span data-ttu-id="37642-120">只读、键、不可为 null</span><span class="sxs-lookup"><span data-stu-id="37642-120">Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="37642-121">servicePlans</span><span class="sxs-lookup"><span data-stu-id="37642-121">servicePlans</span></span>|<span data-ttu-id="37642-122">[servicePlanInfo](serviceplaninfo.md) collection</span><span class="sxs-lookup"><span data-stu-id="37642-122">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="37642-123">有关随许可证分配的服务计划的信息。</span><span class="sxs-lookup"><span data-stu-id="37642-123">Information about the service plans assigned with the license.</span></span> <span data-ttu-id="37642-124">只读，不可为 null</span><span class="sxs-lookup"><span data-stu-id="37642-124">Read-only, Not nullable</span></span> |
|<span data-ttu-id="37642-125">skuId</span><span class="sxs-lookup"><span data-stu-id="37642-125">skuId</span></span>|<span data-ttu-id="37642-126">Guid</span><span class="sxs-lookup"><span data-stu-id="37642-126">Guid</span></span>| <span data-ttu-id="37642-127">服务 SKU (GUID) 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="37642-127">Unique identifier (GUID) for the service SKU.</span></span> <span data-ttu-id="37642-128">等于相关 [SubscribedSku](subscribedsku.md) 对象的 skuId 属性。</span><span class="sxs-lookup"><span data-stu-id="37642-128">Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object.</span></span> <span data-ttu-id="37642-129">只读</span><span class="sxs-lookup"><span data-stu-id="37642-129">Read-only</span></span> |
|<span data-ttu-id="37642-130">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="37642-130">skuPartNumber</span></span>|<span data-ttu-id="37642-131">String</span><span class="sxs-lookup"><span data-stu-id="37642-131">String</span></span>| <span data-ttu-id="37642-132">唯一 SKU 显示名称。</span><span class="sxs-lookup"><span data-stu-id="37642-132">Unique SKU display name.</span></span> <span data-ttu-id="37642-133">等于相关 [SubscribedSku](subscribedsku.md) 对象上的 skuPartNumber;例如："AAD_Premium"。</span><span class="sxs-lookup"><span data-stu-id="37642-133">Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium".</span></span> <span data-ttu-id="37642-134">只读</span><span class="sxs-lookup"><span data-stu-id="37642-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="37642-135">关系</span><span class="sxs-lookup"><span data-stu-id="37642-135">Relationships</span></span>
<span data-ttu-id="37642-136">无</span><span class="sxs-lookup"><span data-stu-id="37642-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37642-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37642-137">JSON representation</span></span>
<span data-ttu-id="37642-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37642-138">Here is a JSON representation of the resource.</span></span>

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

