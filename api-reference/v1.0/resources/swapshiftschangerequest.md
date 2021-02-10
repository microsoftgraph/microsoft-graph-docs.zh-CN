---
title: swapShiftsChangeRequest 资源类型
description: 表示要与团队中的其他用户交换班次的班次请求类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5f5d1bb7a520d5d7f64640725a846ef5bc76a0b2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154731"
---
# <a name="swapshiftschangerequest-resource-type"></a><span data-ttu-id="f7024-103">swapShiftsChangeRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7024-103">swapShiftsChangeRequest resource type</span></span>

<span data-ttu-id="f7024-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7024-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f7024-105">表示要与团队中的 [其他用户交换班次](../resources/shift.md) 的班次 [请求类型](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="f7024-105">Represents a type of shift request to swap a [shift](../resources/shift.md) with another user in the [team](../resources/team.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f7024-106">方法</span><span class="sxs-lookup"><span data-stu-id="f7024-106">Methods</span></span>

| <span data-ttu-id="f7024-107">方法</span><span class="sxs-lookup"><span data-stu-id="f7024-107">Method</span></span>       | <span data-ttu-id="f7024-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f7024-108">Return Type</span></span> | <span data-ttu-id="f7024-109">Description</span><span class="sxs-lookup"><span data-stu-id="f7024-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f7024-110">List</span><span class="sxs-lookup"><span data-stu-id="f7024-110">List</span></span>](../api/swapshiftschangerequest-list.md) | <span data-ttu-id="f7024-111">[swapShiftsChangeRequest 集合](swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="f7024-111">Collection of [swapShiftsChangeRequest](swapshiftschangerequest.md)</span></span> | <span data-ttu-id="f7024-112">列出团队 **中 swapShiftsChangeRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f7024-112">List the properties and relationships of **swapShiftsChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="f7024-113">创建</span><span class="sxs-lookup"><span data-stu-id="f7024-113">Create</span></span>](../api/swapshiftschangerequest-post.md) | [<span data-ttu-id="f7024-114">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="f7024-114">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="f7024-115">创建 **swapShiftsChangeRequest 对象** 的实例。</span><span class="sxs-lookup"><span data-stu-id="f7024-115">Create an instance of a **swapShiftsChangeRequest** object.</span></span> |
| [<span data-ttu-id="f7024-116">Get</span><span class="sxs-lookup"><span data-stu-id="f7024-116">Get</span></span>](../api/swapshiftschangerequest-get.md) | [<span data-ttu-id="f7024-117">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="f7024-117">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="f7024-118">读取 **swapShiftsChangeRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f7024-118">Read the properties and relationships of a **swapShiftsChangeRequest** object.</span></span> |
|[<span data-ttu-id="f7024-119">批准</span><span class="sxs-lookup"><span data-stu-id="f7024-119">Approve</span></span>](../api/swapshiftschangerequest-approve.md)|<span data-ttu-id="f7024-120">无</span><span class="sxs-lookup"><span data-stu-id="f7024-120">None</span></span>|<span data-ttu-id="f7024-121">批准 **swapShiftsChangeRequest**。</span><span class="sxs-lookup"><span data-stu-id="f7024-121">Approve a **swapShiftsChangeRequest**.</span></span> |
|[<span data-ttu-id="f7024-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="f7024-122">Decline</span></span>](../api/swapshiftschangerequest-decline.md)|<span data-ttu-id="f7024-123">无</span><span class="sxs-lookup"><span data-stu-id="f7024-123">None</span></span>|<span data-ttu-id="f7024-124">拒绝 **swapShiftsChangeRequest**。</span><span class="sxs-lookup"><span data-stu-id="f7024-124">Decline a **swapShiftsChangeRequest**.</span></span>|

## <a name="properties"></a><span data-ttu-id="f7024-125">属性</span><span class="sxs-lookup"><span data-stu-id="f7024-125">Properties</span></span>

| <span data-ttu-id="f7024-126">属性</span><span class="sxs-lookup"><span data-stu-id="f7024-126">Property</span></span>     | <span data-ttu-id="f7024-127">类型</span><span class="sxs-lookup"><span data-stu-id="f7024-127">Type</span></span>        | <span data-ttu-id="f7024-128">说明</span><span class="sxs-lookup"><span data-stu-id="f7024-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f7024-129">recipientShiftId</span><span class="sxs-lookup"><span data-stu-id="f7024-129">recipientShiftId</span></span>|<span data-ttu-id="f7024-130">String</span><span class="sxs-lookup"><span data-stu-id="f7024-130">String</span></span>|<span data-ttu-id="f7024-131">要与之交换请求的收件人用户的 ShiftId。</span><span class="sxs-lookup"><span data-stu-id="f7024-131">ShiftId for the recipient user with whom the request is to swap.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7024-132">关系</span><span class="sxs-lookup"><span data-stu-id="f7024-132">Relationships</span></span>

<span data-ttu-id="f7024-133">无。</span><span class="sxs-lookup"><span data-stu-id="f7024-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7024-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7024-134">JSON representation</span></span>

<span data-ttu-id="f7024-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7024-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
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

