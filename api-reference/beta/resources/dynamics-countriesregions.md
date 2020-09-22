---
title: countriesRegions 资源类型
description: Dynamics 365 Business Central 中的国家/地区对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 490fa240cda525b517bf4e8dcec3e89aedbcc201
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049807"
---
# <a name="countriesregions-resource-type"></a><span data-ttu-id="16023-103">countriesRegions 资源类型</span><span class="sxs-lookup"><span data-stu-id="16023-103">countriesRegions resource type</span></span>

<span data-ttu-id="16023-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16023-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16023-105">代表 Dynamics 365 业务中心中的 countriesRegions 对象，该业务中心是地址的一部分。</span><span class="sxs-lookup"><span data-stu-id="16023-105">Represents a countriesRegions object in Dynamics 365 Business Central, which is part of an address.</span></span>

## <a name="methods"></a><span data-ttu-id="16023-106">方法</span><span class="sxs-lookup"><span data-stu-id="16023-106">Methods</span></span>

| <span data-ttu-id="16023-107">方法</span><span class="sxs-lookup"><span data-stu-id="16023-107">Method</span></span>                                                              | <span data-ttu-id="16023-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="16023-108">Return Type</span></span>    |<span data-ttu-id="16023-109">说明</span><span class="sxs-lookup"><span data-stu-id="16023-109">Description</span></span>                |
|:--------------------------------------------------------------------|:---------------|:--------------------------|
|[<span data-ttu-id="16023-110">获取 countriesRegions</span><span class="sxs-lookup"><span data-stu-id="16023-110">Get countriesRegions</span></span>](../api/dynamics-countriesregions-get.md)      |<span data-ttu-id="16023-111">countriesRegions</span><span class="sxs-lookup"><span data-stu-id="16023-111">countriesRegions</span></span>|<span data-ttu-id="16023-112">获取国家/地区。</span><span class="sxs-lookup"><span data-stu-id="16023-112">Get a Countries/Regions.</span></span>   |
|[<span data-ttu-id="16023-113">Post countriesRegions</span><span class="sxs-lookup"><span data-stu-id="16023-113">Post countriesRegions</span></span>](../api/dynamics-create-countriesregions.md)  |<span data-ttu-id="16023-114">countriesRegions</span><span class="sxs-lookup"><span data-stu-id="16023-114">countriesRegions</span></span>|<span data-ttu-id="16023-115">创建国家/地区。</span><span class="sxs-lookup"><span data-stu-id="16023-115">Create a Countries/Regions.</span></span>|
|[<span data-ttu-id="16023-116">修补程序 countriesRegions</span><span class="sxs-lookup"><span data-stu-id="16023-116">Patch countriesRegions</span></span>](../api/dynamics-countriesregions-update.md) |<span data-ttu-id="16023-117">countriesRegions</span><span class="sxs-lookup"><span data-stu-id="16023-117">countriesRegions</span></span>|<span data-ttu-id="16023-118">更新国家/地区。</span><span class="sxs-lookup"><span data-stu-id="16023-118">Update a Countries/Regions.</span></span>|
|[<span data-ttu-id="16023-119">删除 countriesRegions</span><span class="sxs-lookup"><span data-stu-id="16023-119">Delete countriesRegions</span></span>](../api/dynamics-countriesregions-delete.md)|<span data-ttu-id="16023-120">无</span><span class="sxs-lookup"><span data-stu-id="16023-120">none</span></span>            |<span data-ttu-id="16023-121">删除国家/地区。</span><span class="sxs-lookup"><span data-stu-id="16023-121">Delete a Countries/Regions.</span></span>|

## <a name="properties"></a><span data-ttu-id="16023-122">属性</span><span class="sxs-lookup"><span data-stu-id="16023-122">Properties</span></span>
| <span data-ttu-id="16023-123">属性</span><span class="sxs-lookup"><span data-stu-id="16023-123">Property</span></span>       | <span data-ttu-id="16023-124">类型</span><span class="sxs-lookup"><span data-stu-id="16023-124">Type</span></span>       |<span data-ttu-id="16023-125">说明</span><span class="sxs-lookup"><span data-stu-id="16023-125">Description</span></span>                                                  |
|:---------------|:-----------|:------------------------------------------------------------|
|<span data-ttu-id="16023-126">id</span><span class="sxs-lookup"><span data-stu-id="16023-126">id</span></span>              |<span data-ttu-id="16023-127">GUID</span><span class="sxs-lookup"><span data-stu-id="16023-127">GUID</span></span>        |<span data-ttu-id="16023-128">国家/地区的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="16023-128">The unique ID of the country/region.</span></span> <span data-ttu-id="16023-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="16023-129">Non-editable.</span></span>           |
|<span data-ttu-id="16023-130">code</span><span class="sxs-lookup"><span data-stu-id="16023-130">code</span></span>            |<span data-ttu-id="16023-131">string</span><span class="sxs-lookup"><span data-stu-id="16023-131">string</span></span>      |<span data-ttu-id="16023-132">指定国家/地区的代码。</span><span class="sxs-lookup"><span data-stu-id="16023-132">Specifies the code of the country/region.</span></span>                    |
|<span data-ttu-id="16023-133">displayName</span><span class="sxs-lookup"><span data-stu-id="16023-133">displayName</span></span>     |<span data-ttu-id="16023-134">string</span><span class="sxs-lookup"><span data-stu-id="16023-134">string</span></span>      |<span data-ttu-id="16023-135">指定国家/地区的显示名称。</span><span class="sxs-lookup"><span data-stu-id="16023-135">Specifies the display name of the country/region.</span></span>            |
|<span data-ttu-id="16023-136">addressFormat</span><span class="sxs-lookup"><span data-stu-id="16023-136">addressFormat</span></span>   |<span data-ttu-id="16023-137">string</span><span class="sxs-lookup"><span data-stu-id="16023-137">string</span></span>      |<span data-ttu-id="16023-138">指定在面向外部的文档上显示的地址的格式。</span><span class="sxs-lookup"><span data-stu-id="16023-138">Specifies the format of the address that is displayed on external-facing documents.</span></span> <span data-ttu-id="16023-139">将地址格式链接到国家/地区代码，以便基于包含该国家/地区代码的卡片或文档的面向外部的文档使用指定的地址格式。</span><span class="sxs-lookup"><span data-stu-id="16023-139">You link an address format to a country/region code so that external-facing documents based on cards or documents with that country/region code use the specified address format.</span></span>|
|<span data-ttu-id="16023-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16023-140">lastModifiedDateTime</span></span>|<span data-ttu-id="16023-141">datetime</span><span class="sxs-lookup"><span data-stu-id="16023-141">datetime</span></span>|<span data-ttu-id="16023-142">国家/地区的最后修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="16023-142">The last datetime the country/region was modified.</span></span> <span data-ttu-id="16023-143">只读。</span><span class="sxs-lookup"><span data-stu-id="16023-143">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="16023-144">关系</span><span class="sxs-lookup"><span data-stu-id="16023-144">Relationships</span></span>
<span data-ttu-id="16023-145">无</span><span class="sxs-lookup"><span data-stu-id="16023-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16023-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16023-146">JSON representation</span></span>

<span data-ttu-id="16023-147">下面是 countriesRegions 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16023-147">Here is a JSON representation of the countriesRegions.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "addressFormat": "string",
  "lastModifiedDateTime": "datetime"
}

```




