---
title: taxAreas 资源类型
description: 税务区域。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 140470f0e293b41770779628280f0117d8bb6a89
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027053"
---
# <a name="taxareas-resource-type"></a><span data-ttu-id="29fdb-103">taxAreas 资源类型</span><span class="sxs-lookup"><span data-stu-id="29fdb-103">taxAreas resource type</span></span>

<span data-ttu-id="29fdb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29fdb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29fdb-105">表示 Dynamics 365 Business Central 中的税务区域资源类型。</span><span class="sxs-lookup"><span data-stu-id="29fdb-105">Represents a tax area resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="29fdb-106">方法</span><span class="sxs-lookup"><span data-stu-id="29fdb-106">Methods</span></span>
| <span data-ttu-id="29fdb-107">方法</span><span class="sxs-lookup"><span data-stu-id="29fdb-107">Method</span></span>       | <span data-ttu-id="29fdb-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="29fdb-108">Return Type</span></span>  |<span data-ttu-id="29fdb-109">说明</span><span class="sxs-lookup"><span data-stu-id="29fdb-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="29fdb-110">获取 taxAreas</span><span class="sxs-lookup"><span data-stu-id="29fdb-110">Get taxAreas</span></span>](../api/dynamics-taxarea-get.md)|<span data-ttu-id="29fdb-111">taxAreas</span><span class="sxs-lookup"><span data-stu-id="29fdb-111">taxAreas</span></span>|<span data-ttu-id="29fdb-112">获取税务区域对象。</span><span class="sxs-lookup"><span data-stu-id="29fdb-112">Gets a tax area object.</span></span>|
|[<span data-ttu-id="29fdb-113">Post taxAreas</span><span class="sxs-lookup"><span data-stu-id="29fdb-113">Post taxAreas</span></span>](../api/dynamics-create-taxarea.md)|<span data-ttu-id="29fdb-114">taxAreas</span><span class="sxs-lookup"><span data-stu-id="29fdb-114">taxAreas</span></span>|<span data-ttu-id="29fdb-115">创建税务区域对象。</span><span class="sxs-lookup"><span data-stu-id="29fdb-115">Creates a tax area object.</span></span>|
|[<span data-ttu-id="29fdb-116">修补程序 taxAreas</span><span class="sxs-lookup"><span data-stu-id="29fdb-116">Patch taxAreas</span></span>](../api/dynamics-taxarea-update.md)|<span data-ttu-id="29fdb-117">taxAreas</span><span class="sxs-lookup"><span data-stu-id="29fdb-117">taxAreas</span></span>|<span data-ttu-id="29fdb-118">更新税务区域对象。</span><span class="sxs-lookup"><span data-stu-id="29fdb-118">Updates a tax area object.</span></span>|
|[<span data-ttu-id="29fdb-119">删除 taxAreas</span><span class="sxs-lookup"><span data-stu-id="29fdb-119">Delete taxAreas</span></span>](../api/dynamics-taxarea-delete.md)|<span data-ttu-id="29fdb-120">无</span><span class="sxs-lookup"><span data-stu-id="29fdb-120">none</span></span>|<span data-ttu-id="29fdb-121">删除税务区域对象。</span><span class="sxs-lookup"><span data-stu-id="29fdb-121">Deletes a tax area object.</span></span>|

## <a name="properties"></a><span data-ttu-id="29fdb-122">属性</span><span class="sxs-lookup"><span data-stu-id="29fdb-122">Properties</span></span>
| <span data-ttu-id="29fdb-123">属性</span><span class="sxs-lookup"><span data-stu-id="29fdb-123">Property</span></span>     | <span data-ttu-id="29fdb-124">类型</span><span class="sxs-lookup"><span data-stu-id="29fdb-124">Type</span></span>   |<span data-ttu-id="29fdb-125">说明</span><span class="sxs-lookup"><span data-stu-id="29fdb-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29fdb-126">id</span><span class="sxs-lookup"><span data-stu-id="29fdb-126">id</span></span>|<span data-ttu-id="29fdb-127">GUID</span><span class="sxs-lookup"><span data-stu-id="29fdb-127">GUID</span></span>|<span data-ttu-id="29fdb-128">税务区域的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="29fdb-128">The unique ID of the tax area.</span></span> <span data-ttu-id="29fdb-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="29fdb-129">Non-editable.</span></span>|
|<span data-ttu-id="29fdb-130">code</span><span class="sxs-lookup"><span data-stu-id="29fdb-130">code</span></span>|<span data-ttu-id="29fdb-131">字符串，最大大小为20</span><span class="sxs-lookup"><span data-stu-id="29fdb-131">string, maximum size 20</span></span>| <span data-ttu-id="29fdb-132">税务区域的代码。</span><span class="sxs-lookup"><span data-stu-id="29fdb-132">The code of the tax area.</span></span>|
|<span data-ttu-id="29fdb-133">displayName</span><span class="sxs-lookup"><span data-stu-id="29fdb-133">displayName</span></span>|<span data-ttu-id="29fdb-134">字符串，最大大小为50</span><span class="sxs-lookup"><span data-stu-id="29fdb-134">string, maximum size 50</span></span>| <span data-ttu-id="29fdb-135">税务区域的显示名称。</span><span class="sxs-lookup"><span data-stu-id="29fdb-135">The display name of the tax area.</span></span>|
|<span data-ttu-id="29fdb-136">taxType</span><span class="sxs-lookup"><span data-stu-id="29fdb-136">taxType</span></span>|<span data-ttu-id="29fdb-137">string</span><span class="sxs-lookup"><span data-stu-id="29fdb-137">string</span></span>|<span data-ttu-id="29fdb-138">税务区域的税金类型。</span><span class="sxs-lookup"><span data-stu-id="29fdb-138">The tax type of the tax area.</span></span>|
|<span data-ttu-id="29fdb-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29fdb-139">lastModifiedDateTime</span></span>|<span data-ttu-id="29fdb-140">datetime</span><span class="sxs-lookup"><span data-stu-id="29fdb-140">datetime</span></span>|<span data-ttu-id="29fdb-141">税区域的最后修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="29fdb-141">The last datetime the tax area was modified.</span></span> <span data-ttu-id="29fdb-142">只读。</span><span class="sxs-lookup"><span data-stu-id="29fdb-142">Read-Only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29fdb-143">关系</span><span class="sxs-lookup"><span data-stu-id="29fdb-143">Relationships</span></span>

## <a name="json-representation"></a><span data-ttu-id="29fdb-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29fdb-144">JSON representation</span></span>

<span data-ttu-id="29fdb-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29fdb-145">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "datetime"
}
```




