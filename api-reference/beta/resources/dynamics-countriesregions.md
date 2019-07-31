---
title: countriesRegions 资源类型
description: Dynamics 365 Business Central 中的国家/地区对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 73f60a48e1b7b3564851271209e195ecbbf171e2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012630"
---
# <a name="countriesregions-resource-type"></a><span data-ttu-id="1b87e-103">countriesRegions 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b87e-103">countriesRegions resource type</span></span>
<span data-ttu-id="1b87e-104">代表 Dynamics 365 业务中心中的 countriesRegions 对象, 该业务中心是地址的一部分。</span><span class="sxs-lookup"><span data-stu-id="1b87e-104">Represents a countriesRegions object in Dynamics 365 Business Central, which is part of an address.</span></span>

## <a name="methods"></a><span data-ttu-id="1b87e-105">方法</span><span class="sxs-lookup"><span data-stu-id="1b87e-105">Methods</span></span>

| <span data-ttu-id="1b87e-106">方法</span><span class="sxs-lookup"><span data-stu-id="1b87e-106">Method</span></span>                                                              | <span data-ttu-id="1b87e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="1b87e-107">Return Type</span></span>    |<span data-ttu-id="1b87e-108">说明</span><span class="sxs-lookup"><span data-stu-id="1b87e-108">Description</span></span>                |
|:--------------------------------------------------------------------|:---------------|:--------------------------|
|[<span data-ttu-id="1b87e-109">获取 countriesRegions</span><span class="sxs-lookup"><span data-stu-id="1b87e-109">Get countriesRegions</span></span>](../api/dynamics-countriesregions-get.md)      |<span data-ttu-id="1b87e-110">countriesRegions</span><span class="sxs-lookup"><span data-stu-id="1b87e-110">countriesRegions</span></span>|<span data-ttu-id="1b87e-111">获取国家/地区。</span><span class="sxs-lookup"><span data-stu-id="1b87e-111">Get a Countries/Regions.</span></span>   |
|[<span data-ttu-id="1b87e-112">Post countriesRegions</span><span class="sxs-lookup"><span data-stu-id="1b87e-112">Post countriesRegions</span></span>](../api/dynamics-create-countriesregions.md)  |<span data-ttu-id="1b87e-113">countriesRegions</span><span class="sxs-lookup"><span data-stu-id="1b87e-113">countriesRegions</span></span>|<span data-ttu-id="1b87e-114">创建国家/地区。</span><span class="sxs-lookup"><span data-stu-id="1b87e-114">Create a Countries/Regions.</span></span>|
|[<span data-ttu-id="1b87e-115">修补程序 countriesRegions</span><span class="sxs-lookup"><span data-stu-id="1b87e-115">Patch countriesRegions</span></span>](../api/dynamics-countriesregions-update.md) |<span data-ttu-id="1b87e-116">countriesRegions</span><span class="sxs-lookup"><span data-stu-id="1b87e-116">countriesRegions</span></span>|<span data-ttu-id="1b87e-117">更新国家/地区。</span><span class="sxs-lookup"><span data-stu-id="1b87e-117">Update a Countries/Regions.</span></span>|
|[<span data-ttu-id="1b87e-118">删除 countriesRegions</span><span class="sxs-lookup"><span data-stu-id="1b87e-118">Delete countriesRegions</span></span>](../api/dynamics-countriesregions-delete.md)|<span data-ttu-id="1b87e-119">无</span><span class="sxs-lookup"><span data-stu-id="1b87e-119">none</span></span>            |<span data-ttu-id="1b87e-120">删除国家/地区。</span><span class="sxs-lookup"><span data-stu-id="1b87e-120">Delete a Countries/Regions.</span></span>|

## <a name="properties"></a><span data-ttu-id="1b87e-121">属性</span><span class="sxs-lookup"><span data-stu-id="1b87e-121">Properties</span></span>
| <span data-ttu-id="1b87e-122">属性</span><span class="sxs-lookup"><span data-stu-id="1b87e-122">Property</span></span>       | <span data-ttu-id="1b87e-123">类型</span><span class="sxs-lookup"><span data-stu-id="1b87e-123">Type</span></span>       |<span data-ttu-id="1b87e-124">说明</span><span class="sxs-lookup"><span data-stu-id="1b87e-124">Description</span></span>                                                  |
|:---------------|:-----------|:------------------------------------------------------------|
|<span data-ttu-id="1b87e-125">id</span><span class="sxs-lookup"><span data-stu-id="1b87e-125">id</span></span>              |<span data-ttu-id="1b87e-126">GUID</span><span class="sxs-lookup"><span data-stu-id="1b87e-126">GUID</span></span>        |<span data-ttu-id="1b87e-127">国家/地区的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="1b87e-127">The unique ID of the country/region.</span></span> <span data-ttu-id="1b87e-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="1b87e-128">Non-editable.</span></span>           |
|<span data-ttu-id="1b87e-129">code</span><span class="sxs-lookup"><span data-stu-id="1b87e-129">code</span></span>            |<span data-ttu-id="1b87e-130">string</span><span class="sxs-lookup"><span data-stu-id="1b87e-130">string</span></span>      |<span data-ttu-id="1b87e-131">指定国家/地区的代码。</span><span class="sxs-lookup"><span data-stu-id="1b87e-131">Specifies the code of the country/region.</span></span>                    |
|<span data-ttu-id="1b87e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="1b87e-132">displayName</span></span>     |<span data-ttu-id="1b87e-133">string</span><span class="sxs-lookup"><span data-stu-id="1b87e-133">string</span></span>      |<span data-ttu-id="1b87e-134">指定国家/地区的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1b87e-134">Specifies the display name of the country/region.</span></span>            |
|<span data-ttu-id="1b87e-135">addressFormat</span><span class="sxs-lookup"><span data-stu-id="1b87e-135">addressFormat</span></span>   |<span data-ttu-id="1b87e-136">string</span><span class="sxs-lookup"><span data-stu-id="1b87e-136">string</span></span>      |<span data-ttu-id="1b87e-137">指定在面向外部的文档上显示的地址的格式。</span><span class="sxs-lookup"><span data-stu-id="1b87e-137">Specifies the format of the address that is displayed on external-facing documents.</span></span> <span data-ttu-id="1b87e-138">将地址格式链接到国家/地区代码, 以便基于包含该国家/地区代码的卡片或文档的面向外部的文档使用指定的地址格式。</span><span class="sxs-lookup"><span data-stu-id="1b87e-138">You link an address format to a country/region code so that external-facing documents based on cards or documents with that country/region code use the specified address format.</span></span>|
|<span data-ttu-id="1b87e-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b87e-139">lastModifiedDateTime</span></span>|<span data-ttu-id="1b87e-140">datetime</span><span class="sxs-lookup"><span data-stu-id="1b87e-140">datetime</span></span>|<span data-ttu-id="1b87e-141">国家/地区的最后修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="1b87e-141">The last datetime the country/region was modified.</span></span> <span data-ttu-id="1b87e-142">只读。</span><span class="sxs-lookup"><span data-stu-id="1b87e-142">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="1b87e-143">关系</span><span class="sxs-lookup"><span data-stu-id="1b87e-143">Relationships</span></span>
<span data-ttu-id="1b87e-144">无</span><span class="sxs-lookup"><span data-stu-id="1b87e-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b87e-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b87e-145">JSON representation</span></span>

<span data-ttu-id="1b87e-146">下面是 countriesRegions 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b87e-146">Here is a JSON representation of the countriesRegions.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "addressFormat": "string",
  "lastModifiedDateTime": "datetime"
}

```


