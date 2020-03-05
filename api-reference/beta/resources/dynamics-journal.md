---
title: 日记资源类型
description: Dynamics 365 Business Central 中的日记。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 041de72a3372fd80063b96ba73d10272247c4fdb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503745"
---
# <a name="journal-resource-type"></a><span data-ttu-id="b32e5-103">日记资源类型</span><span class="sxs-lookup"><span data-stu-id="b32e5-103">journal resource type</span></span>

<span data-ttu-id="b32e5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b32e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b32e5-105">代表 Dynamics 365 Business Central 中的日记。</span><span class="sxs-lookup"><span data-stu-id="b32e5-105">Represents a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="b32e5-106">方法</span><span class="sxs-lookup"><span data-stu-id="b32e5-106">Methods</span></span>

| <span data-ttu-id="b32e5-107">方法</span><span class="sxs-lookup"><span data-stu-id="b32e5-107">Method</span></span>                                            |<span data-ttu-id="b32e5-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b32e5-108">Return Type</span></span>|<span data-ttu-id="b32e5-109">说明</span><span class="sxs-lookup"><span data-stu-id="b32e5-109">Description</span></span>    |
|:--------------------------------------------------|:----------|:--------------|
|[<span data-ttu-id="b32e5-110">获取分类账</span><span class="sxs-lookup"><span data-stu-id="b32e5-110">Get journal</span></span>](../api/dynamics-journal-get.md)      |<span data-ttu-id="b32e5-111">日志</span><span class="sxs-lookup"><span data-stu-id="b32e5-111">journal</span></span>    |<span data-ttu-id="b32e5-112">获取日记。</span><span class="sxs-lookup"><span data-stu-id="b32e5-112">Gets a journal.</span></span>   |
|[<span data-ttu-id="b32e5-113">过帐日记</span><span class="sxs-lookup"><span data-stu-id="b32e5-113">Post journal</span></span>](../api/dynamics-create-journal.md)  |<span data-ttu-id="b32e5-114">日志</span><span class="sxs-lookup"><span data-stu-id="b32e5-114">journal</span></span>    |<span data-ttu-id="b32e5-115">创建日记。</span><span class="sxs-lookup"><span data-stu-id="b32e5-115">Creates a journal.</span></span>|
|[<span data-ttu-id="b32e5-116">修补程序日记</span><span class="sxs-lookup"><span data-stu-id="b32e5-116">Patch journal</span></span>](../api/dynamics-journal-update.md) |<span data-ttu-id="b32e5-117">日志</span><span class="sxs-lookup"><span data-stu-id="b32e5-117">journal</span></span>    |<span data-ttu-id="b32e5-118">更新日记。</span><span class="sxs-lookup"><span data-stu-id="b32e5-118">Updates a journal.</span></span>|
|[<span data-ttu-id="b32e5-119">删除分类账</span><span class="sxs-lookup"><span data-stu-id="b32e5-119">Delete journal</span></span>](../api/dynamics-journal-delete.md)|<span data-ttu-id="b32e5-120">无</span><span class="sxs-lookup"><span data-stu-id="b32e5-120">none</span></span>       |<span data-ttu-id="b32e5-121">删除日记。</span><span class="sxs-lookup"><span data-stu-id="b32e5-121">Deletes a journal.</span></span>|

## <a name="properties"></a><span data-ttu-id="b32e5-122">属性</span><span class="sxs-lookup"><span data-stu-id="b32e5-122">Properties</span></span>
| <span data-ttu-id="b32e5-123">属性</span><span class="sxs-lookup"><span data-stu-id="b32e5-123">Property</span></span>           | <span data-ttu-id="b32e5-124">类型</span><span class="sxs-lookup"><span data-stu-id="b32e5-124">Type</span></span>                  |<span data-ttu-id="b32e5-125">说明</span><span class="sxs-lookup"><span data-stu-id="b32e5-125">Description</span></span>                                           |
|:-------------------|:----------------------|:-----------------------------------------------------|
|<span data-ttu-id="b32e5-126">id</span><span class="sxs-lookup"><span data-stu-id="b32e5-126">id</span></span>                  |<span data-ttu-id="b32e5-127">GUID</span><span class="sxs-lookup"><span data-stu-id="b32e5-127">GUID</span></span>                   |<span data-ttu-id="b32e5-128">日记的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="b32e5-128">The unique ID of the journal.</span></span> <span data-ttu-id="b32e5-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="b32e5-129">Non-editable.</span></span>           |
|<span data-ttu-id="b32e5-130">code</span><span class="sxs-lookup"><span data-stu-id="b32e5-130">code</span></span>                |<span data-ttu-id="b32e5-131">字符串，最大值为10</span><span class="sxs-lookup"><span data-stu-id="b32e5-131">string, maximum size 10</span></span>| <span data-ttu-id="b32e5-132">日记的代码。</span><span class="sxs-lookup"><span data-stu-id="b32e5-132">The code of the journal.</span></span>                             |
|<span data-ttu-id="b32e5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b32e5-133">displayName</span></span>         |<span data-ttu-id="b32e5-134">字符串，最大大小为50</span><span class="sxs-lookup"><span data-stu-id="b32e5-134">string, maximum size 50</span></span>| <span data-ttu-id="b32e5-135">日记的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b32e5-135">The display name of the journal.</span></span>                     |
|<span data-ttu-id="b32e5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b32e5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b32e5-137">datetime</span><span class="sxs-lookup"><span data-stu-id="b32e5-137">datetime</span></span>               |<span data-ttu-id="b32e5-138">日记已修改的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b32e5-138">The last datetime the journal was modified.</span></span> <span data-ttu-id="b32e5-139">只读。</span><span class="sxs-lookup"><span data-stu-id="b32e5-139">Read-Only.</span></span>|

## <a name="bound-actions"></a><span data-ttu-id="b32e5-140">绑定操作</span><span class="sxs-lookup"><span data-stu-id="b32e5-140">Bound actions</span></span>
<span data-ttu-id="b32e5-141">日记资源类型提供一个调用`post`的绑定操作，该操作将发布相应的常规日记批处理。</span><span class="sxs-lookup"><span data-stu-id="b32e5-141">The journal resource type offers a bound action called `post` which posts the corresponding general journal batch.</span></span>

<span data-ttu-id="b32e5-142">下面的示例演示了如何过帐常规日记批处理：</span><span class="sxs-lookup"><span data-stu-id="b32e5-142">Posting the general journal batch is illustrated in the following example:</span></span>  
<span data-ttu-id="b32e5-143">`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.</span><span class="sxs-lookup"><span data-stu-id="b32e5-143">`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.</span></span>

<span data-ttu-id="b32e5-144">响应没有内容;响应代码为204。</span><span class="sxs-lookup"><span data-stu-id="b32e5-144">The response has no content; the response code is 204.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b32e5-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b32e5-145">JSON representation</span></span>

<span data-ttu-id="b32e5-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b32e5-146">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

