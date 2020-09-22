---
title: swapShiftsChangeRequest 资源类型
description: 表示向团队中的其他用户交换班次的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3a18b3627aec777bf95ece65cd26a170d6f98ad7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056441"
---
# <a name="swapshiftschangerequest-resource-type"></a><span data-ttu-id="984d1-103">swapShiftsChangeRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="984d1-103">swapShiftsChangeRequest resource type</span></span>

<span data-ttu-id="984d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="984d1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="984d1-105">表示将 [班次](../resources/shift.md) 与 [团队](../resources/team.md)中的其他用户交换的班次请求类型。</span><span class="sxs-lookup"><span data-stu-id="984d1-105">Represents a type of shift request to swap a [shift](../resources/shift.md) with another user in the [team](../resources/team.md).</span></span>

## <a name="methods"></a><span data-ttu-id="984d1-106">方法</span><span class="sxs-lookup"><span data-stu-id="984d1-106">Methods</span></span>

| <span data-ttu-id="984d1-107">方法</span><span class="sxs-lookup"><span data-stu-id="984d1-107">Method</span></span>       | <span data-ttu-id="984d1-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="984d1-108">Return Type</span></span> | <span data-ttu-id="984d1-109">Description</span><span class="sxs-lookup"><span data-stu-id="984d1-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="984d1-110">List</span><span class="sxs-lookup"><span data-stu-id="984d1-110">List</span></span>](../api/swapshiftschangerequest-list.md) | <span data-ttu-id="984d1-111">[SwapShiftsChangeRequest](swapshiftschangerequest.md)的集合</span><span class="sxs-lookup"><span data-stu-id="984d1-111">Collection of [swapShiftsChangeRequest](swapshiftschangerequest.md)</span></span> | <span data-ttu-id="984d1-112">列出团队中的 **swapShiftsChangeRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="984d1-112">List the properties and relationships of **swapShiftsChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="984d1-113">创建</span><span class="sxs-lookup"><span data-stu-id="984d1-113">Create</span></span>](../api/swapshiftschangerequest-post.md) | [<span data-ttu-id="984d1-114">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="984d1-114">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="984d1-115">创建 **swapShiftsChangeRequest** 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="984d1-115">Create an instance of a **swapShiftsChangeRequest** object.</span></span> |
| [<span data-ttu-id="984d1-116">获取</span><span class="sxs-lookup"><span data-stu-id="984d1-116">Get</span></span>](../api/swapshiftschangerequest-get.md) | [<span data-ttu-id="984d1-117">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="984d1-117">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="984d1-118">读取 **swapShiftsChangeRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="984d1-118">Read the properties and relationships of a **swapShiftsChangeRequest** object.</span></span> |
|[<span data-ttu-id="984d1-119">批准</span><span class="sxs-lookup"><span data-stu-id="984d1-119">Approve</span></span>](../api/swapshiftschangerequest-approve.md)|<span data-ttu-id="984d1-120">无</span><span class="sxs-lookup"><span data-stu-id="984d1-120">None</span></span>|<span data-ttu-id="984d1-121">批准 **swapShiftsChangeRequest**。</span><span class="sxs-lookup"><span data-stu-id="984d1-121">Approve a **swapShiftsChangeRequest**.</span></span> |
|[<span data-ttu-id="984d1-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="984d1-122">Decline</span></span>](../api/swapshiftschangerequest-decline.md)|<span data-ttu-id="984d1-123">无</span><span class="sxs-lookup"><span data-stu-id="984d1-123">None</span></span>|<span data-ttu-id="984d1-124">拒绝 **swapShiftsChangeRequest**。</span><span class="sxs-lookup"><span data-stu-id="984d1-124">Decline a **swapShiftsChangeRequest**.</span></span>|

## <a name="properties"></a><span data-ttu-id="984d1-125">属性</span><span class="sxs-lookup"><span data-stu-id="984d1-125">Properties</span></span>

| <span data-ttu-id="984d1-126">属性</span><span class="sxs-lookup"><span data-stu-id="984d1-126">Property</span></span>     | <span data-ttu-id="984d1-127">类型</span><span class="sxs-lookup"><span data-stu-id="984d1-127">Type</span></span>        | <span data-ttu-id="984d1-128">说明</span><span class="sxs-lookup"><span data-stu-id="984d1-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="984d1-129">recipientShiftId</span><span class="sxs-lookup"><span data-stu-id="984d1-129">recipientShiftId</span></span>|<span data-ttu-id="984d1-130">String</span><span class="sxs-lookup"><span data-stu-id="984d1-130">String</span></span>|<span data-ttu-id="984d1-131">ShiftId 要与之交换请求的收件人用户。</span><span class="sxs-lookup"><span data-stu-id="984d1-131">ShiftId for the recipient user with whom the request is to swap.</span></span>|

## <a name="relationships"></a><span data-ttu-id="984d1-132">关系</span><span class="sxs-lookup"><span data-stu-id="984d1-132">Relationships</span></span>

<span data-ttu-id="984d1-133">无。</span><span class="sxs-lookup"><span data-stu-id="984d1-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="984d1-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="984d1-134">JSON representation</span></span>

<span data-ttu-id="984d1-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="984d1-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest",
  "baseType": ""
}-->

```json
{
  "recipientShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "swapShiftsChangeRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

