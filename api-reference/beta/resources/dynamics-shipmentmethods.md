---
title: shipmentMethods 资源类型
description: Dynamics 365 Business Central 中的装运方法。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 2f7ef9611fc85c13ac24c79b292e06a6bdc5d587
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365498"
---
# <a name="shipmentmethods-resource-type"></a><span data-ttu-id="72bca-103">shipmentMethods 资源类型</span><span class="sxs-lookup"><span data-stu-id="72bca-103">shipmentMethods resource type</span></span>
<span data-ttu-id="72bca-104">代表 Dynamics 365 Business Central 中的送货方法, 如 UPS、Fedex 和 DHL。</span><span class="sxs-lookup"><span data-stu-id="72bca-104">Represents a method of shipment in Dynamics 365 Business Central, such as UPS, Fedex, and DHL.</span></span>

## <a name="methods"></a><span data-ttu-id="72bca-105">方法</span><span class="sxs-lookup"><span data-stu-id="72bca-105">Methods</span></span>

| <span data-ttu-id="72bca-106">方法</span><span class="sxs-lookup"><span data-stu-id="72bca-106">Method</span></span>       | <span data-ttu-id="72bca-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="72bca-107">Return Type</span></span>  |<span data-ttu-id="72bca-108">说明</span><span class="sxs-lookup"><span data-stu-id="72bca-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="72bca-109">获取 shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="72bca-109">Get shipmentMethods</span></span>](../api/dynamics-shipmentmethods-get.md)|<span data-ttu-id="72bca-110">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="72bca-110">shipmentMethods</span></span>|<span data-ttu-id="72bca-111">获取装运方法。</span><span class="sxs-lookup"><span data-stu-id="72bca-111">Gets a shipment method.</span></span>|
|[<span data-ttu-id="72bca-112">Post shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="72bca-112">Post shipmentMethods</span></span>](../api/dynamics-create-shipmentmethods.md)|<span data-ttu-id="72bca-113">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="72bca-113">shipmentMethods</span></span>|<span data-ttu-id="72bca-114">创建装运方法。</span><span class="sxs-lookup"><span data-stu-id="72bca-114">Creates a shipment method.</span></span>|
|[<span data-ttu-id="72bca-115">修补程序 shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="72bca-115">Patch shipmentMethods</span></span>](../api/dynamics-shipmentmethods-update.md)|<span data-ttu-id="72bca-116">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="72bca-116">shipmentMethods</span></span>|<span data-ttu-id="72bca-117">更新装运方法。</span><span class="sxs-lookup"><span data-stu-id="72bca-117">Updates a shipment method.</span></span>|
|[<span data-ttu-id="72bca-118">删除 shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="72bca-118">Delete shipmentMethods</span></span>](../api/dynamics-shipmentmethods-delete.md)|<span data-ttu-id="72bca-119">无</span><span class="sxs-lookup"><span data-stu-id="72bca-119">none</span></span>|<span data-ttu-id="72bca-120">删除装运方法。</span><span class="sxs-lookup"><span data-stu-id="72bca-120">Deletes a shipment method.</span></span>|

## <a name="properties"></a><span data-ttu-id="72bca-121">属性</span><span class="sxs-lookup"><span data-stu-id="72bca-121">Properties</span></span>
| <span data-ttu-id="72bca-122">属性</span><span class="sxs-lookup"><span data-stu-id="72bca-122">Property</span></span>     | <span data-ttu-id="72bca-123">类型</span><span class="sxs-lookup"><span data-stu-id="72bca-123">Type</span></span>   |<span data-ttu-id="72bca-124">说明</span><span class="sxs-lookup"><span data-stu-id="72bca-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72bca-125">id</span><span class="sxs-lookup"><span data-stu-id="72bca-125">id</span></span>|<span data-ttu-id="72bca-126">GUID</span><span class="sxs-lookup"><span data-stu-id="72bca-126">GUID</span></span>|<span data-ttu-id="72bca-127">shipmentMethod 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="72bca-127">The unique ID of the shipmentMethod.</span></span> <span data-ttu-id="72bca-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="72bca-128">Non-editable.</span></span>|
|<span data-ttu-id="72bca-129">code</span><span class="sxs-lookup"><span data-stu-id="72bca-129">code</span></span>|<span data-ttu-id="72bca-130">字符串</span><span class="sxs-lookup"><span data-stu-id="72bca-130">string</span></span>|<span data-ttu-id="72bca-131">指定装运方法代码。</span><span class="sxs-lookup"><span data-stu-id="72bca-131">Specifies the shipment method code.</span></span>|
|<span data-ttu-id="72bca-132">displayName</span><span class="sxs-lookup"><span data-stu-id="72bca-132">displayName</span></span>|<span data-ttu-id="72bca-133">string</span><span class="sxs-lookup"><span data-stu-id="72bca-133">string</span></span>|<span data-ttu-id="72bca-134">指定装运方法的显示名称。</span><span class="sxs-lookup"><span data-stu-id="72bca-134">Specifies the shipment method display name.</span></span>|
|<span data-ttu-id="72bca-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72bca-135">lastModifiedDateTime</span></span>|<span data-ttu-id="72bca-136">datetime</span><span class="sxs-lookup"><span data-stu-id="72bca-136">datetime</span></span>|<span data-ttu-id="72bca-137">最后一个日期/时间修改了运输方法。</span><span class="sxs-lookup"><span data-stu-id="72bca-137">The last datetime the shipment method was modified.</span></span> <span data-ttu-id="72bca-138">只读。</span><span class="sxs-lookup"><span data-stu-id="72bca-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="72bca-139">关系</span><span class="sxs-lookup"><span data-stu-id="72bca-139">Relationships</span></span>
<span data-ttu-id="72bca-140">无</span><span class="sxs-lookup"><span data-stu-id="72bca-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72bca-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72bca-141">JSON representation</span></span>

<span data-ttu-id="72bca-142">下面是 shipmentMethod 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72bca-142">Here is a JSON representation of the shipmentMethod.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


