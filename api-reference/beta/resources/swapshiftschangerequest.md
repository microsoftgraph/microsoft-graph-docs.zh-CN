---
title: swapShiftsChangeRequest 资源类型
description: 表示向团队中的其他用户交换班次的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 96589309cbeb2880e533b5607dc05beec78894ed
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520266"
---
# <a name="swapshiftschangerequest-resource-type"></a><span data-ttu-id="9638b-103">swapShiftsChangeRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="9638b-103">swapShiftsChangeRequest resource type</span></span>

<span data-ttu-id="9638b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9638b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9638b-105">表示将[班次](../resources/shift.md)与[团队](../resources/team.md)中的其他用户交换的班次请求类型。</span><span class="sxs-lookup"><span data-stu-id="9638b-105">Represents a type of shift request to swap a [shift](../resources/shift.md) with another user in the [team](../resources/team.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9638b-106">方法</span><span class="sxs-lookup"><span data-stu-id="9638b-106">Methods</span></span>

| <span data-ttu-id="9638b-107">方法</span><span class="sxs-lookup"><span data-stu-id="9638b-107">Method</span></span>       | <span data-ttu-id="9638b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9638b-108">Return Type</span></span> | <span data-ttu-id="9638b-109">说明</span><span class="sxs-lookup"><span data-stu-id="9638b-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9638b-110">List</span><span class="sxs-lookup"><span data-stu-id="9638b-110">List</span></span>](../api/swapshiftschangerequest-list.md) | <span data-ttu-id="9638b-111">[SwapShiftsChangeRequest](swapshiftschangerequest.md)的集合</span><span class="sxs-lookup"><span data-stu-id="9638b-111">Collection of [swapShiftsChangeRequest](swapshiftschangerequest.md)</span></span> | <span data-ttu-id="9638b-112">列出团队中的**swapShiftsChangeRequest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9638b-112">List the properties and relationships of **swapShiftsChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="9638b-113">创建</span><span class="sxs-lookup"><span data-stu-id="9638b-113">Create</span></span>](../api/swapshiftschangerequest-post.md) | [<span data-ttu-id="9638b-114">swapshiftschangerequest</span><span class="sxs-lookup"><span data-stu-id="9638b-114">swapshiftschangerequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="9638b-115">创建 swapshiftschangerequest 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="9638b-115">Create an instance of an swapshiftschangerequest object.</span></span> |
| [<span data-ttu-id="9638b-116">获取</span><span class="sxs-lookup"><span data-stu-id="9638b-116">Get</span></span>](../api/swapshiftschangerequest-get.md) | [<span data-ttu-id="9638b-117">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="9638b-117">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="9638b-118">读取**swapShiftsChangeRequest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9638b-118">Read the properties and relationships of a **swapShiftsChangeRequest** object.</span></span> |
|[<span data-ttu-id="9638b-119">批准</span><span class="sxs-lookup"><span data-stu-id="9638b-119">Approve</span></span>](../api/swapshiftschangerequest-approve.md)|<span data-ttu-id="9638b-120">无</span><span class="sxs-lookup"><span data-stu-id="9638b-120">None</span></span>|<span data-ttu-id="9638b-121">批准**swapShiftsChangeRequest**。</span><span class="sxs-lookup"><span data-stu-id="9638b-121">Approve a **swapShiftsChangeRequest**.</span></span> |
|[<span data-ttu-id="9638b-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="9638b-122">Decline</span></span>](../api/swapshiftschangerequest-decline.md)|<span data-ttu-id="9638b-123">无</span><span class="sxs-lookup"><span data-stu-id="9638b-123">None</span></span>|<span data-ttu-id="9638b-124">拒绝**swapShiftsChangeRequest**。</span><span class="sxs-lookup"><span data-stu-id="9638b-124">Decline a **swapShiftsChangeRequest**.</span></span>|

## <a name="properties"></a><span data-ttu-id="9638b-125">属性</span><span class="sxs-lookup"><span data-stu-id="9638b-125">Properties</span></span>

| <span data-ttu-id="9638b-126">属性</span><span class="sxs-lookup"><span data-stu-id="9638b-126">Property</span></span>     | <span data-ttu-id="9638b-127">类型</span><span class="sxs-lookup"><span data-stu-id="9638b-127">Type</span></span>        | <span data-ttu-id="9638b-128">说明</span><span class="sxs-lookup"><span data-stu-id="9638b-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9638b-129">recipientShiftId</span><span class="sxs-lookup"><span data-stu-id="9638b-129">recipientShiftId</span></span>|<span data-ttu-id="9638b-130">String</span><span class="sxs-lookup"><span data-stu-id="9638b-130">String</span></span>|<span data-ttu-id="9638b-131">交换请求的收件人的 ID。</span><span class="sxs-lookup"><span data-stu-id="9638b-131">ID of the recipient of the swap request.</span></span> <span data-ttu-id="9638b-132">这是请求要交换的用户。</span><span class="sxs-lookup"><span data-stu-id="9638b-132">This is the user with whom the request is to swap.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9638b-133">关系</span><span class="sxs-lookup"><span data-stu-id="9638b-133">Relationships</span></span>

<span data-ttu-id="9638b-134">无。</span><span class="sxs-lookup"><span data-stu-id="9638b-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9638b-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9638b-135">JSON representation</span></span>

<span data-ttu-id="9638b-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9638b-136">The following is a JSON representation of the resource.</span></span>

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
