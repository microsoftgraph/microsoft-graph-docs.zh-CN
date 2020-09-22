---
title: 日记资源类型
description: Dynamics 365 Business Central 中的日记。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ecbeba91828ba06b9927af08ac8d75a177e27cea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013830"
---
# <a name="journal-resource-type"></a><span data-ttu-id="663e3-103">日记资源类型</span><span class="sxs-lookup"><span data-stu-id="663e3-103">journal resource type</span></span>

<span data-ttu-id="663e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="663e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="663e3-105">代表 Dynamics 365 Business Central 中的日记。</span><span class="sxs-lookup"><span data-stu-id="663e3-105">Represents a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="663e3-106">方法</span><span class="sxs-lookup"><span data-stu-id="663e3-106">Methods</span></span>

| <span data-ttu-id="663e3-107">方法</span><span class="sxs-lookup"><span data-stu-id="663e3-107">Method</span></span>                                            |<span data-ttu-id="663e3-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="663e3-108">Return Type</span></span>|<span data-ttu-id="663e3-109">说明</span><span class="sxs-lookup"><span data-stu-id="663e3-109">Description</span></span>    |
|:--------------------------------------------------|:----------|:--------------|
|[<span data-ttu-id="663e3-110">获取分类账</span><span class="sxs-lookup"><span data-stu-id="663e3-110">Get journal</span></span>](../api/dynamics-journal-get.md)      |<span data-ttu-id="663e3-111">日志</span><span class="sxs-lookup"><span data-stu-id="663e3-111">journal</span></span>    |<span data-ttu-id="663e3-112">获取日记。</span><span class="sxs-lookup"><span data-stu-id="663e3-112">Gets a journal.</span></span>   |
|[<span data-ttu-id="663e3-113">过帐日记</span><span class="sxs-lookup"><span data-stu-id="663e3-113">Post journal</span></span>](../api/dynamics-create-journal.md)  |<span data-ttu-id="663e3-114">日志</span><span class="sxs-lookup"><span data-stu-id="663e3-114">journal</span></span>    |<span data-ttu-id="663e3-115">创建日记。</span><span class="sxs-lookup"><span data-stu-id="663e3-115">Creates a journal.</span></span>|
|[<span data-ttu-id="663e3-116">修补程序日记</span><span class="sxs-lookup"><span data-stu-id="663e3-116">Patch journal</span></span>](../api/dynamics-journal-update.md) |<span data-ttu-id="663e3-117">日志</span><span class="sxs-lookup"><span data-stu-id="663e3-117">journal</span></span>    |<span data-ttu-id="663e3-118">更新日记。</span><span class="sxs-lookup"><span data-stu-id="663e3-118">Updates a journal.</span></span>|
|[<span data-ttu-id="663e3-119">删除分类账</span><span class="sxs-lookup"><span data-stu-id="663e3-119">Delete journal</span></span>](../api/dynamics-journal-delete.md)|<span data-ttu-id="663e3-120">无</span><span class="sxs-lookup"><span data-stu-id="663e3-120">none</span></span>       |<span data-ttu-id="663e3-121">删除日记。</span><span class="sxs-lookup"><span data-stu-id="663e3-121">Deletes a journal.</span></span>|

## <a name="properties"></a><span data-ttu-id="663e3-122">属性</span><span class="sxs-lookup"><span data-stu-id="663e3-122">Properties</span></span>
| <span data-ttu-id="663e3-123">属性</span><span class="sxs-lookup"><span data-stu-id="663e3-123">Property</span></span>           | <span data-ttu-id="663e3-124">类型</span><span class="sxs-lookup"><span data-stu-id="663e3-124">Type</span></span>                  |<span data-ttu-id="663e3-125">说明</span><span class="sxs-lookup"><span data-stu-id="663e3-125">Description</span></span>                                           |
|:-------------------|:----------------------|:-----------------------------------------------------|
|<span data-ttu-id="663e3-126">id</span><span class="sxs-lookup"><span data-stu-id="663e3-126">id</span></span>                  |<span data-ttu-id="663e3-127">GUID</span><span class="sxs-lookup"><span data-stu-id="663e3-127">GUID</span></span>                   |<span data-ttu-id="663e3-128">日记的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="663e3-128">The unique ID of the journal.</span></span> <span data-ttu-id="663e3-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="663e3-129">Non-editable.</span></span>           |
|<span data-ttu-id="663e3-130">code</span><span class="sxs-lookup"><span data-stu-id="663e3-130">code</span></span>                |<span data-ttu-id="663e3-131">字符串，最大值为10</span><span class="sxs-lookup"><span data-stu-id="663e3-131">string, maximum size 10</span></span>| <span data-ttu-id="663e3-132">日记的代码。</span><span class="sxs-lookup"><span data-stu-id="663e3-132">The code of the journal.</span></span>                             |
|<span data-ttu-id="663e3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="663e3-133">displayName</span></span>         |<span data-ttu-id="663e3-134">字符串，最大大小为50</span><span class="sxs-lookup"><span data-stu-id="663e3-134">string, maximum size 50</span></span>| <span data-ttu-id="663e3-135">日记的显示名称。</span><span class="sxs-lookup"><span data-stu-id="663e3-135">The display name of the journal.</span></span>                     |
|<span data-ttu-id="663e3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="663e3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="663e3-137">datetime</span><span class="sxs-lookup"><span data-stu-id="663e3-137">datetime</span></span>               |<span data-ttu-id="663e3-138">日记已修改的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="663e3-138">The last datetime the journal was modified.</span></span> <span data-ttu-id="663e3-139">只读。</span><span class="sxs-lookup"><span data-stu-id="663e3-139">Read-Only.</span></span>|

## <a name="bound-actions"></a><span data-ttu-id="663e3-140">绑定操作</span><span class="sxs-lookup"><span data-stu-id="663e3-140">Bound actions</span></span>
<span data-ttu-id="663e3-141">日记资源类型提供一个调用的绑定操作 `post` ，该操作将发布相应的常规日记批处理。</span><span class="sxs-lookup"><span data-stu-id="663e3-141">The journal resource type offers a bound action called `post` which posts the corresponding general journal batch.</span></span>

<span data-ttu-id="663e3-142">下面的示例演示了如何过帐常规日记批处理：</span><span class="sxs-lookup"><span data-stu-id="663e3-142">Posting the general journal batch is illustrated in the following example:</span></span>  
<span data-ttu-id="663e3-143">`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.</span><span class="sxs-lookup"><span data-stu-id="663e3-143">`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.</span></span>

<span data-ttu-id="663e3-144">响应没有内容;响应代码为204。</span><span class="sxs-lookup"><span data-stu-id="663e3-144">The response has no content; the response code is 204.</span></span>

## <a name="json-representation"></a><span data-ttu-id="663e3-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="663e3-145">JSON representation</span></span>

<span data-ttu-id="663e3-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="663e3-146">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```



