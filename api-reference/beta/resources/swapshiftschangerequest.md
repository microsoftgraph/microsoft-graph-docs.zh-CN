---
title: swapShiftsChangeRequest 资源类型
description: 表示向团队中的其他用户交换班次的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d274c73cfcfb71bb86349dbe4cbbc7661e9e7a16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078148"
---
# <a name="swapshiftschangerequest-resource-type"></a><span data-ttu-id="f03e3-103">swapShiftsChangeRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="f03e3-103">swapShiftsChangeRequest resource type</span></span>

<span data-ttu-id="f03e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f03e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f03e3-105">表示将 [班次](../resources/shift.md) 与 [团队](../resources/team.md)中的其他用户交换的班次请求类型。</span><span class="sxs-lookup"><span data-stu-id="f03e3-105">Represents a type of shift request to swap a [shift](../resources/shift.md) with another user in the [team](../resources/team.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f03e3-106">方法</span><span class="sxs-lookup"><span data-stu-id="f03e3-106">Methods</span></span>

| <span data-ttu-id="f03e3-107">方法</span><span class="sxs-lookup"><span data-stu-id="f03e3-107">Method</span></span>       | <span data-ttu-id="f03e3-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f03e3-108">Return Type</span></span> | <span data-ttu-id="f03e3-109">Description</span><span class="sxs-lookup"><span data-stu-id="f03e3-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f03e3-110">List</span><span class="sxs-lookup"><span data-stu-id="f03e3-110">List</span></span>](../api/swapshiftschangerequest-list.md) | <span data-ttu-id="f03e3-111">[SwapShiftsChangeRequest](swapshiftschangerequest.md)的集合</span><span class="sxs-lookup"><span data-stu-id="f03e3-111">Collection of [swapShiftsChangeRequest](swapshiftschangerequest.md)</span></span> | <span data-ttu-id="f03e3-112">列出团队中的 **swapShiftsChangeRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f03e3-112">List the properties and relationships of **swapShiftsChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="f03e3-113">Create</span><span class="sxs-lookup"><span data-stu-id="f03e3-113">Create</span></span>](../api/swapshiftschangerequest-post.md) | [<span data-ttu-id="f03e3-114">swapshiftschangerequest</span><span class="sxs-lookup"><span data-stu-id="f03e3-114">swapshiftschangerequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="f03e3-115">创建 swapshiftschangerequest 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="f03e3-115">Create an instance of an swapshiftschangerequest object.</span></span> |
| [<span data-ttu-id="f03e3-116">Get</span><span class="sxs-lookup"><span data-stu-id="f03e3-116">Get</span></span>](../api/swapshiftschangerequest-get.md) | [<span data-ttu-id="f03e3-117">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="f03e3-117">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="f03e3-118">读取 **swapShiftsChangeRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f03e3-118">Read the properties and relationships of a **swapShiftsChangeRequest** object.</span></span> |
|[<span data-ttu-id="f03e3-119">批准</span><span class="sxs-lookup"><span data-stu-id="f03e3-119">Approve</span></span>](../api/swapshiftschangerequest-approve.md)|<span data-ttu-id="f03e3-120">无</span><span class="sxs-lookup"><span data-stu-id="f03e3-120">None</span></span>|<span data-ttu-id="f03e3-121">批准 **swapShiftsChangeRequest**。</span><span class="sxs-lookup"><span data-stu-id="f03e3-121">Approve a **swapShiftsChangeRequest**.</span></span> |
|[<span data-ttu-id="f03e3-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="f03e3-122">Decline</span></span>](../api/swapshiftschangerequest-decline.md)|<span data-ttu-id="f03e3-123">无</span><span class="sxs-lookup"><span data-stu-id="f03e3-123">None</span></span>|<span data-ttu-id="f03e3-124">拒绝 **swapShiftsChangeRequest**。</span><span class="sxs-lookup"><span data-stu-id="f03e3-124">Decline a **swapShiftsChangeRequest**.</span></span>|

## <a name="properties"></a><span data-ttu-id="f03e3-125">属性</span><span class="sxs-lookup"><span data-stu-id="f03e3-125">Properties</span></span>

| <span data-ttu-id="f03e3-126">属性</span><span class="sxs-lookup"><span data-stu-id="f03e3-126">Property</span></span>     | <span data-ttu-id="f03e3-127">类型</span><span class="sxs-lookup"><span data-stu-id="f03e3-127">Type</span></span>        | <span data-ttu-id="f03e3-128">说明</span><span class="sxs-lookup"><span data-stu-id="f03e3-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f03e3-129">recipientShiftId</span><span class="sxs-lookup"><span data-stu-id="f03e3-129">recipientShiftId</span></span>|<span data-ttu-id="f03e3-130">String</span><span class="sxs-lookup"><span data-stu-id="f03e3-130">String</span></span>|<span data-ttu-id="f03e3-131">请求要交换的收件人用户的 Shift ID。</span><span class="sxs-lookup"><span data-stu-id="f03e3-131">Shift ID for the recipient user with whom the request is to swap.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f03e3-132">关系</span><span class="sxs-lookup"><span data-stu-id="f03e3-132">Relationships</span></span>

<span data-ttu-id="f03e3-133">无。</span><span class="sxs-lookup"><span data-stu-id="f03e3-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f03e3-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f03e3-134">JSON representation</span></span>

<span data-ttu-id="f03e3-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f03e3-135">The following is a JSON representation of the resource.</span></span>

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


