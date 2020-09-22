---
title: shipmentMethods 资源类型
description: Dynamics 365 Business Central 中的装运方法。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d45153a08572f32f29128fd4d3f51638d71c951b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027067"
---
# <a name="shipmentmethods-resource-type"></a><span data-ttu-id="426a8-103">shipmentMethods 资源类型</span><span class="sxs-lookup"><span data-stu-id="426a8-103">shipmentMethods resource type</span></span>

<span data-ttu-id="426a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="426a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="426a8-105">代表 Dynamics 365 Business Central 中的送货方法，如 UPS、Fedex 和 DHL。</span><span class="sxs-lookup"><span data-stu-id="426a8-105">Represents a method of shipment in Dynamics 365 Business Central, such as UPS, Fedex, and DHL.</span></span>

## <a name="methods"></a><span data-ttu-id="426a8-106">方法</span><span class="sxs-lookup"><span data-stu-id="426a8-106">Methods</span></span>

| <span data-ttu-id="426a8-107">方法</span><span class="sxs-lookup"><span data-stu-id="426a8-107">Method</span></span>       | <span data-ttu-id="426a8-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="426a8-108">Return Type</span></span>  |<span data-ttu-id="426a8-109">说明</span><span class="sxs-lookup"><span data-stu-id="426a8-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="426a8-110">获取 shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="426a8-110">Get shipmentMethods</span></span>](../api/dynamics-shipmentmethods-get.md)|<span data-ttu-id="426a8-111">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="426a8-111">shipmentMethods</span></span>|<span data-ttu-id="426a8-112">获取装运方法。</span><span class="sxs-lookup"><span data-stu-id="426a8-112">Gets a shipment method.</span></span>|
|[<span data-ttu-id="426a8-113">Post shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="426a8-113">Post shipmentMethods</span></span>](../api/dynamics-create-shipmentmethods.md)|<span data-ttu-id="426a8-114">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="426a8-114">shipmentMethods</span></span>|<span data-ttu-id="426a8-115">创建装运方法。</span><span class="sxs-lookup"><span data-stu-id="426a8-115">Creates a shipment method.</span></span>|
|[<span data-ttu-id="426a8-116">修补程序 shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="426a8-116">Patch shipmentMethods</span></span>](../api/dynamics-shipmentmethods-update.md)|<span data-ttu-id="426a8-117">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="426a8-117">shipmentMethods</span></span>|<span data-ttu-id="426a8-118">更新装运方法。</span><span class="sxs-lookup"><span data-stu-id="426a8-118">Updates a shipment method.</span></span>|
|[<span data-ttu-id="426a8-119">删除 shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="426a8-119">Delete shipmentMethods</span></span>](../api/dynamics-shipmentmethods-delete.md)|<span data-ttu-id="426a8-120">无</span><span class="sxs-lookup"><span data-stu-id="426a8-120">none</span></span>|<span data-ttu-id="426a8-121">删除装运方法。</span><span class="sxs-lookup"><span data-stu-id="426a8-121">Deletes a shipment method.</span></span>|

## <a name="properties"></a><span data-ttu-id="426a8-122">属性</span><span class="sxs-lookup"><span data-stu-id="426a8-122">Properties</span></span>
| <span data-ttu-id="426a8-123">属性</span><span class="sxs-lookup"><span data-stu-id="426a8-123">Property</span></span>     | <span data-ttu-id="426a8-124">类型</span><span class="sxs-lookup"><span data-stu-id="426a8-124">Type</span></span>   |<span data-ttu-id="426a8-125">说明</span><span class="sxs-lookup"><span data-stu-id="426a8-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="426a8-126">id</span><span class="sxs-lookup"><span data-stu-id="426a8-126">id</span></span>|<span data-ttu-id="426a8-127">GUID</span><span class="sxs-lookup"><span data-stu-id="426a8-127">GUID</span></span>|<span data-ttu-id="426a8-128">ShipmentMethod 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="426a8-128">The unique ID of the shipmentMethod.</span></span> <span data-ttu-id="426a8-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="426a8-129">Non-editable.</span></span>|
|<span data-ttu-id="426a8-130">code</span><span class="sxs-lookup"><span data-stu-id="426a8-130">code</span></span>|<span data-ttu-id="426a8-131">string</span><span class="sxs-lookup"><span data-stu-id="426a8-131">string</span></span>|<span data-ttu-id="426a8-132">指定装运方法代码。</span><span class="sxs-lookup"><span data-stu-id="426a8-132">Specifies the shipment method code.</span></span>|
|<span data-ttu-id="426a8-133">displayName</span><span class="sxs-lookup"><span data-stu-id="426a8-133">displayName</span></span>|<span data-ttu-id="426a8-134">string</span><span class="sxs-lookup"><span data-stu-id="426a8-134">string</span></span>|<span data-ttu-id="426a8-135">指定装运方法的显示名称。</span><span class="sxs-lookup"><span data-stu-id="426a8-135">Specifies the shipment method display name.</span></span>|
|<span data-ttu-id="426a8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="426a8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="426a8-137">datetime</span><span class="sxs-lookup"><span data-stu-id="426a8-137">datetime</span></span>|<span data-ttu-id="426a8-138">最后一个日期/时间修改了运输方法。</span><span class="sxs-lookup"><span data-stu-id="426a8-138">The last datetime the shipment method was modified.</span></span> <span data-ttu-id="426a8-139">只读。</span><span class="sxs-lookup"><span data-stu-id="426a8-139">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="426a8-140">关系</span><span class="sxs-lookup"><span data-stu-id="426a8-140">Relationships</span></span>
<span data-ttu-id="426a8-141">无</span><span class="sxs-lookup"><span data-stu-id="426a8-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="426a8-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="426a8-142">JSON representation</span></span>

<span data-ttu-id="426a8-143">下面是 shipmentMethod 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="426a8-143">Here is a JSON representation of the shipmentMethod.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```




