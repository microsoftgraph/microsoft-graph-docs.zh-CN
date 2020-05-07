---
title: swapShiftsChangeRequest 资源类型
description: 表示向团队中的其他用户交换班次的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9bd867642da41b2aa0644744655c94b1d842d977
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154267"
---
# <a name="swapshiftschangerequest-resource-type"></a><span data-ttu-id="df165-103">swapShiftsChangeRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="df165-103">swapShiftsChangeRequest resource type</span></span>

<span data-ttu-id="df165-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df165-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df165-105">表示将[班次](../resources/shift.md)与[团队](../resources/team.md)中的其他用户交换的班次请求类型。</span><span class="sxs-lookup"><span data-stu-id="df165-105">Represents a type of shift request to swap a [shift](../resources/shift.md) with another user in the [team](../resources/team.md).</span></span>

## <a name="methods"></a><span data-ttu-id="df165-106">方法</span><span class="sxs-lookup"><span data-stu-id="df165-106">Methods</span></span>

| <span data-ttu-id="df165-107">方法</span><span class="sxs-lookup"><span data-stu-id="df165-107">Method</span></span>       | <span data-ttu-id="df165-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="df165-108">Return Type</span></span> | <span data-ttu-id="df165-109">说明</span><span class="sxs-lookup"><span data-stu-id="df165-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="df165-110">List</span><span class="sxs-lookup"><span data-stu-id="df165-110">List</span></span>](../api/swapshiftschangerequest-list.md) | <span data-ttu-id="df165-111">[SwapShiftsChangeRequest](swapshiftschangerequest.md)的集合</span><span class="sxs-lookup"><span data-stu-id="df165-111">Collection of [swapShiftsChangeRequest](swapshiftschangerequest.md)</span></span> | <span data-ttu-id="df165-112">列出团队中的**swapShiftsChangeRequest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="df165-112">List the properties and relationships of **swapShiftsChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="df165-113">创建</span><span class="sxs-lookup"><span data-stu-id="df165-113">Create</span></span>](../api/swapshiftschangerequest-post.md) | [<span data-ttu-id="df165-114">swapshiftschangerequest</span><span class="sxs-lookup"><span data-stu-id="df165-114">swapshiftschangerequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="df165-115">创建 swapshiftschangerequest 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="df165-115">Create an instance of an swapshiftschangerequest object.</span></span> |
| [<span data-ttu-id="df165-116">获取</span><span class="sxs-lookup"><span data-stu-id="df165-116">Get</span></span>](../api/swapshiftschangerequest-get.md) | [<span data-ttu-id="df165-117">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="df165-117">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="df165-118">读取**swapShiftsChangeRequest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="df165-118">Read the properties and relationships of a **swapShiftsChangeRequest** object.</span></span> |
|[<span data-ttu-id="df165-119">批准</span><span class="sxs-lookup"><span data-stu-id="df165-119">Approve</span></span>](../api/swapshiftschangerequest-approve.md)|<span data-ttu-id="df165-120">None</span><span class="sxs-lookup"><span data-stu-id="df165-120">None</span></span>|<span data-ttu-id="df165-121">批准**swapShiftsChangeRequest**。</span><span class="sxs-lookup"><span data-stu-id="df165-121">Approve a **swapShiftsChangeRequest**.</span></span> |
|[<span data-ttu-id="df165-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="df165-122">Decline</span></span>](../api/swapshiftschangerequest-decline.md)|<span data-ttu-id="df165-123">None</span><span class="sxs-lookup"><span data-stu-id="df165-123">None</span></span>|<span data-ttu-id="df165-124">拒绝**swapShiftsChangeRequest**。</span><span class="sxs-lookup"><span data-stu-id="df165-124">Decline a **swapShiftsChangeRequest**.</span></span>|

## <a name="properties"></a><span data-ttu-id="df165-125">属性</span><span class="sxs-lookup"><span data-stu-id="df165-125">Properties</span></span>

| <span data-ttu-id="df165-126">属性</span><span class="sxs-lookup"><span data-stu-id="df165-126">Property</span></span>     | <span data-ttu-id="df165-127">类型</span><span class="sxs-lookup"><span data-stu-id="df165-127">Type</span></span>        | <span data-ttu-id="df165-128">Description</span><span class="sxs-lookup"><span data-stu-id="df165-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df165-129">recipientShiftId</span><span class="sxs-lookup"><span data-stu-id="df165-129">recipientShiftId</span></span>|<span data-ttu-id="df165-130">字符串</span><span class="sxs-lookup"><span data-stu-id="df165-130">String</span></span>|<span data-ttu-id="df165-131">请求要交换的收件人用户的 Shift ID。</span><span class="sxs-lookup"><span data-stu-id="df165-131">Shift ID for the recipient user with whom the request is to swap.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df165-132">关系</span><span class="sxs-lookup"><span data-stu-id="df165-132">Relationships</span></span>

<span data-ttu-id="df165-133">无。</span><span class="sxs-lookup"><span data-stu-id="df165-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="df165-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df165-134">JSON representation</span></span>

<span data-ttu-id="df165-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df165-135">The following is a JSON representation of the resource.</span></span>

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
