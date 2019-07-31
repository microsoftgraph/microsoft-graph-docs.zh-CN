---
title: 日记资源类型
description: Dynamics 365 Business Central 中的日记。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 7cfc723a4370c2b30440dcd4e33b50ed066ac89b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006590"
---
# <a name="journal-resource-type"></a><span data-ttu-id="80773-103">日记资源类型</span><span class="sxs-lookup"><span data-stu-id="80773-103">journal resource type</span></span>
<span data-ttu-id="80773-104">代表 Dynamics 365 Business Central 中的日记。</span><span class="sxs-lookup"><span data-stu-id="80773-104">Represents a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="80773-105">方法</span><span class="sxs-lookup"><span data-stu-id="80773-105">Methods</span></span>

| <span data-ttu-id="80773-106">方法</span><span class="sxs-lookup"><span data-stu-id="80773-106">Method</span></span>                                            |<span data-ttu-id="80773-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="80773-107">Return Type</span></span>|<span data-ttu-id="80773-108">说明</span><span class="sxs-lookup"><span data-stu-id="80773-108">Description</span></span>    |
|:--------------------------------------------------|:----------|:--------------|
|[<span data-ttu-id="80773-109">获取分类账</span><span class="sxs-lookup"><span data-stu-id="80773-109">Get journal</span></span>](../api/dynamics-journal-get.md)      |<span data-ttu-id="80773-110">日志</span><span class="sxs-lookup"><span data-stu-id="80773-110">journal</span></span>    |<span data-ttu-id="80773-111">获取日记。</span><span class="sxs-lookup"><span data-stu-id="80773-111">Gets a journal.</span></span>   |
|[<span data-ttu-id="80773-112">过帐日记</span><span class="sxs-lookup"><span data-stu-id="80773-112">Post journal</span></span>](../api/dynamics-create-journal.md)  |<span data-ttu-id="80773-113">日志</span><span class="sxs-lookup"><span data-stu-id="80773-113">journal</span></span>    |<span data-ttu-id="80773-114">创建日记。</span><span class="sxs-lookup"><span data-stu-id="80773-114">Creates a journal.</span></span>|
|[<span data-ttu-id="80773-115">修补程序日记</span><span class="sxs-lookup"><span data-stu-id="80773-115">Patch journal</span></span>](../api/dynamics-journal-update.md) |<span data-ttu-id="80773-116">日志</span><span class="sxs-lookup"><span data-stu-id="80773-116">journal</span></span>    |<span data-ttu-id="80773-117">更新日记。</span><span class="sxs-lookup"><span data-stu-id="80773-117">Updates a journal.</span></span>|
|[<span data-ttu-id="80773-118">删除分类账</span><span class="sxs-lookup"><span data-stu-id="80773-118">Delete journal</span></span>](../api/dynamics-journal-delete.md)|<span data-ttu-id="80773-119">无</span><span class="sxs-lookup"><span data-stu-id="80773-119">none</span></span>       |<span data-ttu-id="80773-120">删除日记。</span><span class="sxs-lookup"><span data-stu-id="80773-120">Deletes a journal.</span></span>|

## <a name="properties"></a><span data-ttu-id="80773-121">属性</span><span class="sxs-lookup"><span data-stu-id="80773-121">Properties</span></span>
| <span data-ttu-id="80773-122">属性</span><span class="sxs-lookup"><span data-stu-id="80773-122">Property</span></span>           | <span data-ttu-id="80773-123">类型</span><span class="sxs-lookup"><span data-stu-id="80773-123">Type</span></span>                  |<span data-ttu-id="80773-124">说明</span><span class="sxs-lookup"><span data-stu-id="80773-124">Description</span></span>                                           |
|:-------------------|:----------------------|:-----------------------------------------------------|
|<span data-ttu-id="80773-125">id</span><span class="sxs-lookup"><span data-stu-id="80773-125">id</span></span>                  |<span data-ttu-id="80773-126">GUID</span><span class="sxs-lookup"><span data-stu-id="80773-126">GUID</span></span>                   |<span data-ttu-id="80773-127">日记的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="80773-127">The unique ID of the journal.</span></span> <span data-ttu-id="80773-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="80773-128">Non-editable.</span></span>           |
|<span data-ttu-id="80773-129">code</span><span class="sxs-lookup"><span data-stu-id="80773-129">code</span></span>                |<span data-ttu-id="80773-130">字符串, 最大值为10</span><span class="sxs-lookup"><span data-stu-id="80773-130">string, maximum size 10</span></span>| <span data-ttu-id="80773-131">日记的代码。</span><span class="sxs-lookup"><span data-stu-id="80773-131">The code of the journal.</span></span>                             |
|<span data-ttu-id="80773-132">displayName</span><span class="sxs-lookup"><span data-stu-id="80773-132">displayName</span></span>         |<span data-ttu-id="80773-133">字符串, 最大大小为50</span><span class="sxs-lookup"><span data-stu-id="80773-133">string, maximum size 50</span></span>| <span data-ttu-id="80773-134">日记的显示名称。</span><span class="sxs-lookup"><span data-stu-id="80773-134">The display name of the journal.</span></span>                     |
|<span data-ttu-id="80773-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80773-135">lastModifiedDateTime</span></span>|<span data-ttu-id="80773-136">datetime</span><span class="sxs-lookup"><span data-stu-id="80773-136">datetime</span></span>               |<span data-ttu-id="80773-137">日记已修改的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="80773-137">The last datetime the journal was modified.</span></span> <span data-ttu-id="80773-138">只读。</span><span class="sxs-lookup"><span data-stu-id="80773-138">Read-Only.</span></span>|

## <a name="bound-actions"></a><span data-ttu-id="80773-139">绑定操作</span><span class="sxs-lookup"><span data-stu-id="80773-139">Bound actions</span></span>
<span data-ttu-id="80773-140">日记资源类型提供一个调用`post`的绑定操作, 该操作将发布相应的常规日记批处理。</span><span class="sxs-lookup"><span data-stu-id="80773-140">The journal resource type offers a bound action called `post` which posts the corresponding general journal batch.</span></span>

<span data-ttu-id="80773-141">下面的示例演示了如何过帐常规日记批处理:</span><span class="sxs-lookup"><span data-stu-id="80773-141">Posting the general journal batch is illustrated in the following example:</span></span>  
<span data-ttu-id="80773-142">`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.</span><span class="sxs-lookup"><span data-stu-id="80773-142"></span></span>

<span data-ttu-id="80773-143">响应没有内容;响应代码为204。</span><span class="sxs-lookup"><span data-stu-id="80773-143">The response has no content; the response code is 204.</span></span>

## <a name="json-representation"></a><span data-ttu-id="80773-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80773-144">JSON representation</span></span>

<span data-ttu-id="80773-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80773-145">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

