---
title: taxAreas 资源类型
description: 税务区域。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: aeda0ca136c178355a8a8f9589eb7410399ef62a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507229"
---
# <a name="taxareas-resource-type"></a><span data-ttu-id="ddf11-103">taxAreas 资源类型</span><span class="sxs-lookup"><span data-stu-id="ddf11-103">taxAreas resource type</span></span>
<span data-ttu-id="ddf11-104">表示 Dynamics 365 Business Central 中的税务区域资源类型。</span><span class="sxs-lookup"><span data-stu-id="ddf11-104">Represents a tax area resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="ddf11-105">方法</span><span class="sxs-lookup"><span data-stu-id="ddf11-105">Methods</span></span>
| <span data-ttu-id="ddf11-106">方法</span><span class="sxs-lookup"><span data-stu-id="ddf11-106">Method</span></span>       | <span data-ttu-id="ddf11-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="ddf11-107">Return Type</span></span>  |<span data-ttu-id="ddf11-108">说明</span><span class="sxs-lookup"><span data-stu-id="ddf11-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ddf11-109">获取 taxAreas</span><span class="sxs-lookup"><span data-stu-id="ddf11-109">Get taxAreas</span></span>](../api/dynamics-taxarea-get.md)|<span data-ttu-id="ddf11-110">taxAreas</span><span class="sxs-lookup"><span data-stu-id="ddf11-110">taxAreas</span></span>|<span data-ttu-id="ddf11-111">获取税务区域对象。</span><span class="sxs-lookup"><span data-stu-id="ddf11-111">Gets a tax area object.</span></span>|
|[<span data-ttu-id="ddf11-112">Post taxAreas</span><span class="sxs-lookup"><span data-stu-id="ddf11-112">Post taxAreas</span></span>](../api/dynamics-create-taxarea.md)|<span data-ttu-id="ddf11-113">taxAreas</span><span class="sxs-lookup"><span data-stu-id="ddf11-113">taxAreas</span></span>|<span data-ttu-id="ddf11-114">创建税务区域对象。</span><span class="sxs-lookup"><span data-stu-id="ddf11-114">Creates a tax area object.</span></span>|
|[<span data-ttu-id="ddf11-115">修补程序 taxAreas</span><span class="sxs-lookup"><span data-stu-id="ddf11-115">Patch taxAreas</span></span>](../api/dynamics-taxarea-update.md)|<span data-ttu-id="ddf11-116">taxAreas</span><span class="sxs-lookup"><span data-stu-id="ddf11-116">taxAreas</span></span>|<span data-ttu-id="ddf11-117">更新税务区域对象。</span><span class="sxs-lookup"><span data-stu-id="ddf11-117">Updates a tax area object.</span></span>|
|[<span data-ttu-id="ddf11-118">删除 taxAreas</span><span class="sxs-lookup"><span data-stu-id="ddf11-118">Delete taxAreas</span></span>](../api/dynamics-taxarea-delete.md)|<span data-ttu-id="ddf11-119">无</span><span class="sxs-lookup"><span data-stu-id="ddf11-119">none</span></span>|<span data-ttu-id="ddf11-120">删除税务区域对象。</span><span class="sxs-lookup"><span data-stu-id="ddf11-120">Deletes a tax area object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ddf11-121">属性</span><span class="sxs-lookup"><span data-stu-id="ddf11-121">Properties</span></span>
| <span data-ttu-id="ddf11-122">属性</span><span class="sxs-lookup"><span data-stu-id="ddf11-122">Property</span></span>     | <span data-ttu-id="ddf11-123">类型</span><span class="sxs-lookup"><span data-stu-id="ddf11-123">Type</span></span>   |<span data-ttu-id="ddf11-124">说明</span><span class="sxs-lookup"><span data-stu-id="ddf11-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ddf11-125">id</span><span class="sxs-lookup"><span data-stu-id="ddf11-125">id</span></span>|<span data-ttu-id="ddf11-126">GUID</span><span class="sxs-lookup"><span data-stu-id="ddf11-126">GUID</span></span>|<span data-ttu-id="ddf11-127">税务区域的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="ddf11-127">The unique ID of the tax area.</span></span> <span data-ttu-id="ddf11-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="ddf11-128">Non-editable.</span></span>|
|<span data-ttu-id="ddf11-129">code</span><span class="sxs-lookup"><span data-stu-id="ddf11-129">code</span></span>|<span data-ttu-id="ddf11-130">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="ddf11-130">string, maximum size 20</span></span>| <span data-ttu-id="ddf11-131">税务区域的代码。</span><span class="sxs-lookup"><span data-stu-id="ddf11-131">The code of the tax area.</span></span>|
|<span data-ttu-id="ddf11-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ddf11-132">displayName</span></span>|<span data-ttu-id="ddf11-133">字符串, 最大大小为50</span><span class="sxs-lookup"><span data-stu-id="ddf11-133">string, maximum size 50</span></span>| <span data-ttu-id="ddf11-134">税务区域的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ddf11-134">The display name of the tax area.</span></span>|
|<span data-ttu-id="ddf11-135">taxType</span><span class="sxs-lookup"><span data-stu-id="ddf11-135">taxType</span></span>|<span data-ttu-id="ddf11-136">字符串</span><span class="sxs-lookup"><span data-stu-id="ddf11-136">string</span></span>|<span data-ttu-id="ddf11-137">税务区域的税金类型。</span><span class="sxs-lookup"><span data-stu-id="ddf11-137">The tax type of the tax area.</span></span>|
|<span data-ttu-id="ddf11-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddf11-138">lastModifiedDateTime</span></span>|<span data-ttu-id="ddf11-139">datetime</span><span class="sxs-lookup"><span data-stu-id="ddf11-139">datetime</span></span>|<span data-ttu-id="ddf11-140">税区域的最后修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="ddf11-140">The last datetime the tax area was modified.</span></span> <span data-ttu-id="ddf11-141">只读。</span><span class="sxs-lookup"><span data-stu-id="ddf11-141">Read-Only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddf11-142">关系</span><span class="sxs-lookup"><span data-stu-id="ddf11-142">Relationships</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddf11-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ddf11-143">JSON representation</span></span>

<span data-ttu-id="ddf11-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ddf11-144">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "datetime"
}
```


