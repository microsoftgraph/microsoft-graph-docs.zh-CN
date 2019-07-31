---
title: taxAreas 资源类型
description: 税务区域。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 09c1c51fed961489d824136f28aaa2f5b3859b44
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972892"
---
# <a name="taxareas-resource-type"></a><span data-ttu-id="aff29-103">taxAreas 资源类型</span><span class="sxs-lookup"><span data-stu-id="aff29-103">taxAreas resource type</span></span>
<span data-ttu-id="aff29-104">表示 Dynamics 365 Business Central 中的税务区域资源类型。</span><span class="sxs-lookup"><span data-stu-id="aff29-104">Represents a tax area resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="aff29-105">方法</span><span class="sxs-lookup"><span data-stu-id="aff29-105">Methods</span></span>
| <span data-ttu-id="aff29-106">方法</span><span class="sxs-lookup"><span data-stu-id="aff29-106">Method</span></span>       | <span data-ttu-id="aff29-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="aff29-107">Return Type</span></span>  |<span data-ttu-id="aff29-108">说明</span><span class="sxs-lookup"><span data-stu-id="aff29-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aff29-109">获取 taxAreas</span><span class="sxs-lookup"><span data-stu-id="aff29-109">Get taxAreas</span></span>](../api/dynamics-taxarea-get.md)|<span data-ttu-id="aff29-110">taxAreas</span><span class="sxs-lookup"><span data-stu-id="aff29-110">taxAreas</span></span>|<span data-ttu-id="aff29-111">获取税务区域对象。</span><span class="sxs-lookup"><span data-stu-id="aff29-111">Gets a tax area object.</span></span>|
|[<span data-ttu-id="aff29-112">Post taxAreas</span><span class="sxs-lookup"><span data-stu-id="aff29-112">Post taxAreas</span></span>](../api/dynamics-create-taxarea.md)|<span data-ttu-id="aff29-113">taxAreas</span><span class="sxs-lookup"><span data-stu-id="aff29-113">taxAreas</span></span>|<span data-ttu-id="aff29-114">创建税务区域对象。</span><span class="sxs-lookup"><span data-stu-id="aff29-114">Creates a tax area object.</span></span>|
|[<span data-ttu-id="aff29-115">修补程序 taxAreas</span><span class="sxs-lookup"><span data-stu-id="aff29-115">Patch taxAreas</span></span>](../api/dynamics-taxarea-update.md)|<span data-ttu-id="aff29-116">taxAreas</span><span class="sxs-lookup"><span data-stu-id="aff29-116">taxAreas</span></span>|<span data-ttu-id="aff29-117">更新税务区域对象。</span><span class="sxs-lookup"><span data-stu-id="aff29-117">Updates a tax area object.</span></span>|
|[<span data-ttu-id="aff29-118">删除 taxAreas</span><span class="sxs-lookup"><span data-stu-id="aff29-118">Delete taxAreas</span></span>](../api/dynamics-taxarea-delete.md)|<span data-ttu-id="aff29-119">无</span><span class="sxs-lookup"><span data-stu-id="aff29-119">none</span></span>|<span data-ttu-id="aff29-120">删除税务区域对象。</span><span class="sxs-lookup"><span data-stu-id="aff29-120">Deletes a tax area object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aff29-121">属性</span><span class="sxs-lookup"><span data-stu-id="aff29-121">Properties</span></span>
| <span data-ttu-id="aff29-122">属性</span><span class="sxs-lookup"><span data-stu-id="aff29-122">Property</span></span>     | <span data-ttu-id="aff29-123">类型</span><span class="sxs-lookup"><span data-stu-id="aff29-123">Type</span></span>   |<span data-ttu-id="aff29-124">说明</span><span class="sxs-lookup"><span data-stu-id="aff29-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aff29-125">id</span><span class="sxs-lookup"><span data-stu-id="aff29-125">id</span></span>|<span data-ttu-id="aff29-126">GUID</span><span class="sxs-lookup"><span data-stu-id="aff29-126">GUID</span></span>|<span data-ttu-id="aff29-127">税务区域的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="aff29-127">The unique ID of the tax area.</span></span> <span data-ttu-id="aff29-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="aff29-128">Non-editable.</span></span>|
|<span data-ttu-id="aff29-129">code</span><span class="sxs-lookup"><span data-stu-id="aff29-129">code</span></span>|<span data-ttu-id="aff29-130">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="aff29-130">string, maximum size 20</span></span>| <span data-ttu-id="aff29-131">税务区域的代码。</span><span class="sxs-lookup"><span data-stu-id="aff29-131">The code of the tax area.</span></span>|
|<span data-ttu-id="aff29-132">displayName</span><span class="sxs-lookup"><span data-stu-id="aff29-132">displayName</span></span>|<span data-ttu-id="aff29-133">字符串, 最大大小为50</span><span class="sxs-lookup"><span data-stu-id="aff29-133">string, maximum size 50</span></span>| <span data-ttu-id="aff29-134">税务区域的显示名称。</span><span class="sxs-lookup"><span data-stu-id="aff29-134">The display name of the tax area.</span></span>|
|<span data-ttu-id="aff29-135">taxType</span><span class="sxs-lookup"><span data-stu-id="aff29-135">taxType</span></span>|<span data-ttu-id="aff29-136">string</span><span class="sxs-lookup"><span data-stu-id="aff29-136">string</span></span>|<span data-ttu-id="aff29-137">税务区域的税金类型。</span><span class="sxs-lookup"><span data-stu-id="aff29-137">The tax type of the tax area.</span></span>|
|<span data-ttu-id="aff29-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aff29-138">lastModifiedDateTime</span></span>|<span data-ttu-id="aff29-139">datetime</span><span class="sxs-lookup"><span data-stu-id="aff29-139">datetime</span></span>|<span data-ttu-id="aff29-140">税区域的最后修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="aff29-140">The last datetime the tax area was modified.</span></span> <span data-ttu-id="aff29-141">只读。</span><span class="sxs-lookup"><span data-stu-id="aff29-141">Read-Only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aff29-142">关系</span><span class="sxs-lookup"><span data-stu-id="aff29-142">Relationships</span></span>

## <a name="json-representation"></a><span data-ttu-id="aff29-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aff29-143">JSON representation</span></span>

<span data-ttu-id="aff29-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aff29-144">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "datetime"
}
```


