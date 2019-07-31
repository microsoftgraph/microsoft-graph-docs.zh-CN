---
title: unitsOfMeasure 资源类型
description: Dynamics 365 Business Central 中的度量单位对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 3658c4c510194d3cc950094ec9e46db31589bc03
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972864"
---
# <a name="unitsofmeasure-resource-type"></a><span data-ttu-id="67544-103">unitsOfMeasure 资源类型</span><span class="sxs-lookup"><span data-stu-id="67544-103">unitsOfMeasure resource type</span></span>
<span data-ttu-id="67544-104">表示一个度量单位, 它是量的标准度量单位, 在 Dynamics 365 Business Central 中。</span><span class="sxs-lookup"><span data-stu-id="67544-104">Represents a unit of measure, which is a standard of measurement of a quantity, in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="67544-105">方法</span><span class="sxs-lookup"><span data-stu-id="67544-105">Methods</span></span>

| <span data-ttu-id="67544-106">方法</span><span class="sxs-lookup"><span data-stu-id="67544-106">Method</span></span>       | <span data-ttu-id="67544-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="67544-107">Return Type</span></span>  |<span data-ttu-id="67544-108">说明</span><span class="sxs-lookup"><span data-stu-id="67544-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="67544-109">获取 unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="67544-109">Get unitsOfMeasure</span></span>](../api/dynamics-unitsofmeasure-get.md)|<span data-ttu-id="67544-110">unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="67544-110">unitsOfMeasure</span></span>|<span data-ttu-id="67544-111">获取度量单位对象。</span><span class="sxs-lookup"><span data-stu-id="67544-111">Gets a unit of measure object.</span></span>|
|[<span data-ttu-id="67544-112">Post unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="67544-112">Post unitsOfMeasure</span></span>](../api/dynamics-create-unitsofmeasure.md)|<span data-ttu-id="67544-113">unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="67544-113">unitsOfMeasure</span></span>|<span data-ttu-id="67544-114">创建一个度量单位对象。</span><span class="sxs-lookup"><span data-stu-id="67544-114">Creates a unit of measure object.</span></span>|
|[<span data-ttu-id="67544-115">修补程序 unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="67544-115">Patch unitsOfMeasure</span></span>](../api/dynamics-unitsofmeasure-update.md)|<span data-ttu-id="67544-116">unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="67544-116">unitsOfMeasure</span></span>|<span data-ttu-id="67544-117">更新度量单位对象。</span><span class="sxs-lookup"><span data-stu-id="67544-117">Updates a unit of measure object.</span></span>|
|[<span data-ttu-id="67544-118">删除 unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="67544-118">Delete unitsOfMeasure</span></span>](../api/dynamics-unitsofmeasure-delete.md)|<span data-ttu-id="67544-119">无</span><span class="sxs-lookup"><span data-stu-id="67544-119">none</span></span>|<span data-ttu-id="67544-120">删除度量单位对象。</span><span class="sxs-lookup"><span data-stu-id="67544-120">Deletes a unit of measure object.</span></span>|

## <a name="properties"></a><span data-ttu-id="67544-121">属性</span><span class="sxs-lookup"><span data-stu-id="67544-121">Properties</span></span>
| <span data-ttu-id="67544-122">属性</span><span class="sxs-lookup"><span data-stu-id="67544-122">Property</span></span>     | <span data-ttu-id="67544-123">类型</span><span class="sxs-lookup"><span data-stu-id="67544-123">Type</span></span>   |<span data-ttu-id="67544-124">说明</span><span class="sxs-lookup"><span data-stu-id="67544-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67544-125">id</span><span class="sxs-lookup"><span data-stu-id="67544-125">id</span></span>|<span data-ttu-id="67544-126">GUID</span><span class="sxs-lookup"><span data-stu-id="67544-126">GUID</span></span>|<span data-ttu-id="67544-127">UnitsOfMeasure 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="67544-127">The unique ID of the unitsOfMeasure.</span></span> <span data-ttu-id="67544-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="67544-128">Non-editable.</span></span>|
|<span data-ttu-id="67544-129">code</span><span class="sxs-lookup"><span data-stu-id="67544-129">code</span></span>|<span data-ttu-id="67544-130">string</span><span class="sxs-lookup"><span data-stu-id="67544-130">string</span></span>|<span data-ttu-id="67544-131">指定度量单位的代码。</span><span class="sxs-lookup"><span data-stu-id="67544-131">Specifies the code for the unit of measure.</span></span>|
|<span data-ttu-id="67544-132">displayName</span><span class="sxs-lookup"><span data-stu-id="67544-132">displayName</span></span>|<span data-ttu-id="67544-133">string</span><span class="sxs-lookup"><span data-stu-id="67544-133">string</span></span>|<span data-ttu-id="67544-134">指定度量单位的显示名称。</span><span class="sxs-lookup"><span data-stu-id="67544-134">Specifies the unit of measure's display name.</span></span>|
|<span data-ttu-id="67544-135">internationalStandardCode</span><span class="sxs-lookup"><span data-stu-id="67544-135">internationalStandardCode</span></span>|<span data-ttu-id="67544-136">string</span><span class="sxs-lookup"><span data-stu-id="67544-136">string</span></span>|<span data-ttu-id="67544-137">根据与电子发送销售文档的连接的 UNECE Rec20 标准, 指定度量单位代码 (表示)。</span><span class="sxs-lookup"><span data-stu-id="67544-137">Specifies the unit of measure code expressed according to the UNECE Rec20 standard in connection with electronic sending of sales documents.</span></span>|
|<span data-ttu-id="67544-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67544-138">lastModifiedDateTime</span></span>|<span data-ttu-id="67544-139">datetime</span><span class="sxs-lookup"><span data-stu-id="67544-139">datetime</span></span>|<span data-ttu-id="67544-140">最后一个 datetime 的度量单位已修改。</span><span class="sxs-lookup"><span data-stu-id="67544-140">The last datetime the unit of measure was modified.</span></span> <span data-ttu-id="67544-141">只读。</span><span class="sxs-lookup"><span data-stu-id="67544-141">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="67544-142">关系</span><span class="sxs-lookup"><span data-stu-id="67544-142">Relationships</span></span>
<span data-ttu-id="67544-143">无</span><span class="sxs-lookup"><span data-stu-id="67544-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67544-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67544-144">JSON representation</span></span>

<span data-ttu-id="67544-145">下面是**unitsOfMeasure**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67544-145">Here is a JSON representation of the **unitsOfMeasure** resource.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "internationalStandardCode": "string",
  "lastModifiedDateTime": "datetime"
}

```
