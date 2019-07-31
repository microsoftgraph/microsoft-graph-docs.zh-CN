---
title: shipmentMethods 资源类型
description: Dynamics 365 Business Central 中的装运方法。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: e8d25294b219815c8aa569c7a8c7fab7ec68830c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006610"
---
# <a name="shipmentmethods-resource-type"></a><span data-ttu-id="3a042-103">shipmentMethods 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a042-103">shipmentMethods resource type</span></span>
<span data-ttu-id="3a042-104">代表 Dynamics 365 Business Central 中的送货方法, 如 UPS、Fedex 和 DHL。</span><span class="sxs-lookup"><span data-stu-id="3a042-104">Represents a method of shipment in Dynamics 365 Business Central, such as UPS, Fedex, and DHL.</span></span>

## <a name="methods"></a><span data-ttu-id="3a042-105">方法</span><span class="sxs-lookup"><span data-stu-id="3a042-105">Methods</span></span>

| <span data-ttu-id="3a042-106">方法</span><span class="sxs-lookup"><span data-stu-id="3a042-106">Method</span></span>       | <span data-ttu-id="3a042-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="3a042-107">Return Type</span></span>  |<span data-ttu-id="3a042-108">说明</span><span class="sxs-lookup"><span data-stu-id="3a042-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3a042-109">获取 shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="3a042-109">Get shipmentMethods</span></span>](../api/dynamics-shipmentmethods-get.md)|<span data-ttu-id="3a042-110">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="3a042-110">shipmentMethods</span></span>|<span data-ttu-id="3a042-111">获取装运方法。</span><span class="sxs-lookup"><span data-stu-id="3a042-111">Gets a shipment method.</span></span>|
|[<span data-ttu-id="3a042-112">Post shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="3a042-112">Post shipmentMethods</span></span>](../api/dynamics-create-shipmentmethods.md)|<span data-ttu-id="3a042-113">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="3a042-113">shipmentMethods</span></span>|<span data-ttu-id="3a042-114">创建装运方法。</span><span class="sxs-lookup"><span data-stu-id="3a042-114">Creates a shipment method.</span></span>|
|[<span data-ttu-id="3a042-115">修补程序 shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="3a042-115">Patch shipmentMethods</span></span>](../api/dynamics-shipmentmethods-update.md)|<span data-ttu-id="3a042-116">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="3a042-116">shipmentMethods</span></span>|<span data-ttu-id="3a042-117">更新装运方法。</span><span class="sxs-lookup"><span data-stu-id="3a042-117">Updates a shipment method.</span></span>|
|[<span data-ttu-id="3a042-118">删除 shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="3a042-118">Delete shipmentMethods</span></span>](../api/dynamics-shipmentmethods-delete.md)|<span data-ttu-id="3a042-119">无</span><span class="sxs-lookup"><span data-stu-id="3a042-119">none</span></span>|<span data-ttu-id="3a042-120">删除装运方法。</span><span class="sxs-lookup"><span data-stu-id="3a042-120">Deletes a shipment method.</span></span>|

## <a name="properties"></a><span data-ttu-id="3a042-121">属性</span><span class="sxs-lookup"><span data-stu-id="3a042-121">Properties</span></span>
| <span data-ttu-id="3a042-122">属性</span><span class="sxs-lookup"><span data-stu-id="3a042-122">Property</span></span>     | <span data-ttu-id="3a042-123">类型</span><span class="sxs-lookup"><span data-stu-id="3a042-123">Type</span></span>   |<span data-ttu-id="3a042-124">说明</span><span class="sxs-lookup"><span data-stu-id="3a042-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a042-125">id</span><span class="sxs-lookup"><span data-stu-id="3a042-125">id</span></span>|<span data-ttu-id="3a042-126">GUID</span><span class="sxs-lookup"><span data-stu-id="3a042-126">GUID</span></span>|<span data-ttu-id="3a042-127">ShipmentMethod 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="3a042-127">The unique ID of the shipmentMethod.</span></span> <span data-ttu-id="3a042-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="3a042-128">Non-editable.</span></span>|
|<span data-ttu-id="3a042-129">code</span><span class="sxs-lookup"><span data-stu-id="3a042-129">code</span></span>|<span data-ttu-id="3a042-130">string</span><span class="sxs-lookup"><span data-stu-id="3a042-130">string</span></span>|<span data-ttu-id="3a042-131">指定装运方法代码。</span><span class="sxs-lookup"><span data-stu-id="3a042-131">Specifies the shipment method code.</span></span>|
|<span data-ttu-id="3a042-132">displayName</span><span class="sxs-lookup"><span data-stu-id="3a042-132">displayName</span></span>|<span data-ttu-id="3a042-133">string</span><span class="sxs-lookup"><span data-stu-id="3a042-133">string</span></span>|<span data-ttu-id="3a042-134">指定装运方法的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3a042-134">Specifies the shipment method display name.</span></span>|
|<span data-ttu-id="3a042-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a042-135">lastModifiedDateTime</span></span>|<span data-ttu-id="3a042-136">datetime</span><span class="sxs-lookup"><span data-stu-id="3a042-136">datetime</span></span>|<span data-ttu-id="3a042-137">最后一个日期/时间修改了运输方法。</span><span class="sxs-lookup"><span data-stu-id="3a042-137">The last datetime the shipment method was modified.</span></span> <span data-ttu-id="3a042-138">只读。</span><span class="sxs-lookup"><span data-stu-id="3a042-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="3a042-139">关系</span><span class="sxs-lookup"><span data-stu-id="3a042-139">Relationships</span></span>
<span data-ttu-id="3a042-140">无</span><span class="sxs-lookup"><span data-stu-id="3a042-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a042-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a042-141">JSON representation</span></span>

<span data-ttu-id="3a042-142">下面是 shipmentMethod 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a042-142">Here is a JSON representation of the shipmentMethod.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


