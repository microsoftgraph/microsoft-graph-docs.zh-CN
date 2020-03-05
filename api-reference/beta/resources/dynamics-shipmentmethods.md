---
title: shipmentMethods 资源类型
description: Dynamics 365 Business Central 中的装运方法。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 94ebd10ef87946b5333ec5a06d5edccadc298158
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503570"
---
# <a name="shipmentmethods-resource-type"></a><span data-ttu-id="84c90-103">shipmentMethods 资源类型</span><span class="sxs-lookup"><span data-stu-id="84c90-103">shipmentMethods resource type</span></span>

<span data-ttu-id="84c90-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="84c90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84c90-105">代表 Dynamics 365 Business Central 中的送货方法，如 UPS、Fedex 和 DHL。</span><span class="sxs-lookup"><span data-stu-id="84c90-105">Represents a method of shipment in Dynamics 365 Business Central, such as UPS, Fedex, and DHL.</span></span>

## <a name="methods"></a><span data-ttu-id="84c90-106">方法</span><span class="sxs-lookup"><span data-stu-id="84c90-106">Methods</span></span>

| <span data-ttu-id="84c90-107">方法</span><span class="sxs-lookup"><span data-stu-id="84c90-107">Method</span></span>       | <span data-ttu-id="84c90-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="84c90-108">Return Type</span></span>  |<span data-ttu-id="84c90-109">说明</span><span class="sxs-lookup"><span data-stu-id="84c90-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="84c90-110">获取 shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="84c90-110">Get shipmentMethods</span></span>](../api/dynamics-shipmentmethods-get.md)|<span data-ttu-id="84c90-111">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="84c90-111">shipmentMethods</span></span>|<span data-ttu-id="84c90-112">获取装运方法。</span><span class="sxs-lookup"><span data-stu-id="84c90-112">Gets a shipment method.</span></span>|
|[<span data-ttu-id="84c90-113">Post shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="84c90-113">Post shipmentMethods</span></span>](../api/dynamics-create-shipmentmethods.md)|<span data-ttu-id="84c90-114">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="84c90-114">shipmentMethods</span></span>|<span data-ttu-id="84c90-115">创建装运方法。</span><span class="sxs-lookup"><span data-stu-id="84c90-115">Creates a shipment method.</span></span>|
|[<span data-ttu-id="84c90-116">修补程序 shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="84c90-116">Patch shipmentMethods</span></span>](../api/dynamics-shipmentmethods-update.md)|<span data-ttu-id="84c90-117">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="84c90-117">shipmentMethods</span></span>|<span data-ttu-id="84c90-118">更新装运方法。</span><span class="sxs-lookup"><span data-stu-id="84c90-118">Updates a shipment method.</span></span>|
|[<span data-ttu-id="84c90-119">删除 shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="84c90-119">Delete shipmentMethods</span></span>](../api/dynamics-shipmentmethods-delete.md)|<span data-ttu-id="84c90-120">无</span><span class="sxs-lookup"><span data-stu-id="84c90-120">none</span></span>|<span data-ttu-id="84c90-121">删除装运方法。</span><span class="sxs-lookup"><span data-stu-id="84c90-121">Deletes a shipment method.</span></span>|

## <a name="properties"></a><span data-ttu-id="84c90-122">属性</span><span class="sxs-lookup"><span data-stu-id="84c90-122">Properties</span></span>
| <span data-ttu-id="84c90-123">属性</span><span class="sxs-lookup"><span data-stu-id="84c90-123">Property</span></span>     | <span data-ttu-id="84c90-124">类型</span><span class="sxs-lookup"><span data-stu-id="84c90-124">Type</span></span>   |<span data-ttu-id="84c90-125">说明</span><span class="sxs-lookup"><span data-stu-id="84c90-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84c90-126">id</span><span class="sxs-lookup"><span data-stu-id="84c90-126">id</span></span>|<span data-ttu-id="84c90-127">GUID</span><span class="sxs-lookup"><span data-stu-id="84c90-127">GUID</span></span>|<span data-ttu-id="84c90-128">ShipmentMethod 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="84c90-128">The unique ID of the shipmentMethod.</span></span> <span data-ttu-id="84c90-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="84c90-129">Non-editable.</span></span>|
|<span data-ttu-id="84c90-130">code</span><span class="sxs-lookup"><span data-stu-id="84c90-130">code</span></span>|<span data-ttu-id="84c90-131">string</span><span class="sxs-lookup"><span data-stu-id="84c90-131">string</span></span>|<span data-ttu-id="84c90-132">指定装运方法代码。</span><span class="sxs-lookup"><span data-stu-id="84c90-132">Specifies the shipment method code.</span></span>|
|<span data-ttu-id="84c90-133">displayName</span><span class="sxs-lookup"><span data-stu-id="84c90-133">displayName</span></span>|<span data-ttu-id="84c90-134">string</span><span class="sxs-lookup"><span data-stu-id="84c90-134">string</span></span>|<span data-ttu-id="84c90-135">指定装运方法的显示名称。</span><span class="sxs-lookup"><span data-stu-id="84c90-135">Specifies the shipment method display name.</span></span>|
|<span data-ttu-id="84c90-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84c90-136">lastModifiedDateTime</span></span>|<span data-ttu-id="84c90-137">datetime</span><span class="sxs-lookup"><span data-stu-id="84c90-137">datetime</span></span>|<span data-ttu-id="84c90-138">最后一个日期/时间修改了运输方法。</span><span class="sxs-lookup"><span data-stu-id="84c90-138">The last datetime the shipment method was modified.</span></span> <span data-ttu-id="84c90-139">只读。</span><span class="sxs-lookup"><span data-stu-id="84c90-139">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="84c90-140">关系</span><span class="sxs-lookup"><span data-stu-id="84c90-140">Relationships</span></span>
<span data-ttu-id="84c90-141">无</span><span class="sxs-lookup"><span data-stu-id="84c90-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84c90-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84c90-142">JSON representation</span></span>

<span data-ttu-id="84c90-143">下面是 shipmentMethod 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84c90-143">Here is a JSON representation of the shipmentMethod.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


