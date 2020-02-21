---
title: swapShiftsChangeRequest 资源类型
description: 表示向团队中的其他用户交换班次的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b0fbc0f392a6efa1b0a0ba5f1568451a6fe7d1cf
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219753"
---
# <a name="swapshiftschangerequest-resource-type"></a><span data-ttu-id="a73de-103">swapShiftsChangeRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="a73de-103">swapShiftsChangeRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a73de-104">表示将[班次](../resources/shift.md)与[团队](../resources/team.md)中的其他用户交换的班次请求类型。</span><span class="sxs-lookup"><span data-stu-id="a73de-104">Represents a type of shift request to swap a [shift](../resources/shift.md) with another user in the [team](../resources/team.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a73de-105">Methods</span><span class="sxs-lookup"><span data-stu-id="a73de-105">Methods</span></span>

| <span data-ttu-id="a73de-106">方法</span><span class="sxs-lookup"><span data-stu-id="a73de-106">Method</span></span>       | <span data-ttu-id="a73de-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="a73de-107">Return Type</span></span> | <span data-ttu-id="a73de-108">说明</span><span class="sxs-lookup"><span data-stu-id="a73de-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a73de-109">List</span><span class="sxs-lookup"><span data-stu-id="a73de-109">List</span></span>](../api/swapshiftschangerequest-list.md) | <span data-ttu-id="a73de-110">[SwapShiftsChangeRequest](swapshiftschangerequest.md)的集合</span><span class="sxs-lookup"><span data-stu-id="a73de-110">Collection of [swapShiftsChangeRequest](swapshiftschangerequest.md)</span></span> | <span data-ttu-id="a73de-111">列出团队中的**swapShiftsChangeRequest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a73de-111">List the properties and relationships of **swapShiftsChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="a73de-112">创建</span><span class="sxs-lookup"><span data-stu-id="a73de-112">Create</span></span>](../api/swapshiftschangerequest-post.md) | [<span data-ttu-id="a73de-113">swapshiftschangerequest</span><span class="sxs-lookup"><span data-stu-id="a73de-113">swapshiftschangerequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="a73de-114">创建 swapshiftschangerequest 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="a73de-114">Create an instance of an swapshiftschangerequest object.</span></span> |
| [<span data-ttu-id="a73de-115">获取</span><span class="sxs-lookup"><span data-stu-id="a73de-115">Get</span></span>](../api/swapshiftschangerequest-get.md) | [<span data-ttu-id="a73de-116">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="a73de-116">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="a73de-117">读取**swapShiftsChangeRequest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a73de-117">Read the properties and relationships of a **swapShiftsChangeRequest** object.</span></span> |
|[<span data-ttu-id="a73de-118">批准</span><span class="sxs-lookup"><span data-stu-id="a73de-118">Approve</span></span>](../api/swapshiftschangerequest-approve.md)|<span data-ttu-id="a73de-119">无</span><span class="sxs-lookup"><span data-stu-id="a73de-119">None</span></span>|<span data-ttu-id="a73de-120">批准**swapShiftsChangeRequest**。</span><span class="sxs-lookup"><span data-stu-id="a73de-120">Approve a **swapShiftsChangeRequest**.</span></span> |
|[<span data-ttu-id="a73de-121">拒绝</span><span class="sxs-lookup"><span data-stu-id="a73de-121">Decline</span></span>](../api/swapshiftschangerequest-decline.md)|<span data-ttu-id="a73de-122">无</span><span class="sxs-lookup"><span data-stu-id="a73de-122">None</span></span>|<span data-ttu-id="a73de-123">拒绝**swapShiftsChangeRequest**。</span><span class="sxs-lookup"><span data-stu-id="a73de-123">Decline a **swapShiftsChangeRequest**.</span></span>|

## <a name="properties"></a><span data-ttu-id="a73de-124">属性</span><span class="sxs-lookup"><span data-stu-id="a73de-124">Properties</span></span>

| <span data-ttu-id="a73de-125">属性</span><span class="sxs-lookup"><span data-stu-id="a73de-125">Property</span></span>     | <span data-ttu-id="a73de-126">类型</span><span class="sxs-lookup"><span data-stu-id="a73de-126">Type</span></span>        | <span data-ttu-id="a73de-127">说明</span><span class="sxs-lookup"><span data-stu-id="a73de-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a73de-128">recipientShiftId</span><span class="sxs-lookup"><span data-stu-id="a73de-128">recipientShiftId</span></span>|<span data-ttu-id="a73de-129">String</span><span class="sxs-lookup"><span data-stu-id="a73de-129">String</span></span>|<span data-ttu-id="a73de-130">交换请求的收件人的 ID。</span><span class="sxs-lookup"><span data-stu-id="a73de-130">ID of the recipient of the swap request.</span></span> <span data-ttu-id="a73de-131">这是请求要交换的用户。</span><span class="sxs-lookup"><span data-stu-id="a73de-131">This is the user with whom the request is to swap.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a73de-132">关系</span><span class="sxs-lookup"><span data-stu-id="a73de-132">Relationships</span></span>

<span data-ttu-id="a73de-133">无。</span><span class="sxs-lookup"><span data-stu-id="a73de-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a73de-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a73de-134">JSON representation</span></span>

<span data-ttu-id="a73de-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a73de-135">The following is a JSON representation of the resource.</span></span>

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
