---
title: swapShiftsChangeRequest 资源类型
description: 表示向团队中的其他用户交换班次的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a172737f40572b29358ecdc6fba804db2a8b80e5
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951956"
---
# <a name="swapshiftschangerequest-resource-type"></a><span data-ttu-id="169c8-103">swapShiftsChangeRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="169c8-103">swapShiftsChangeRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="169c8-104">表示将[班次](../resources/shift.md)与[团队](../resources/team.md)中的其他用户交换的班次请求类型。</span><span class="sxs-lookup"><span data-stu-id="169c8-104">Represents a type of shift request to swap a [shift](../resources/shift.md) with another user in the [team](../resources/team.md).</span></span>

## <a name="methods"></a><span data-ttu-id="169c8-105">Methods</span><span class="sxs-lookup"><span data-stu-id="169c8-105">Methods</span></span>

| <span data-ttu-id="169c8-106">方法</span><span class="sxs-lookup"><span data-stu-id="169c8-106">Method</span></span>       | <span data-ttu-id="169c8-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="169c8-107">Return Type</span></span> | <span data-ttu-id="169c8-108">说明</span><span class="sxs-lookup"><span data-stu-id="169c8-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="169c8-109">List</span><span class="sxs-lookup"><span data-stu-id="169c8-109">List</span></span>](../api/swapshiftschangerequest-list.md) | <span data-ttu-id="169c8-110">[SwapShiftsChangeRequest](swapshiftschangerequest.md)的集合</span><span class="sxs-lookup"><span data-stu-id="169c8-110">Collection of [swapShiftsChangeRequest](swapshiftschangerequest.md)</span></span> | <span data-ttu-id="169c8-111">列出团队中的**swapShiftsChangeRequest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="169c8-111">List the properties and relationships of **swapShiftsChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="169c8-112">创建</span><span class="sxs-lookup"><span data-stu-id="169c8-112">Create</span></span>](../api/swapshiftschangerequest-post.md) | [<span data-ttu-id="169c8-113">swapshiftschangerequest</span><span class="sxs-lookup"><span data-stu-id="169c8-113">swapshiftschangerequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="169c8-114">创建 swapshiftschangerequest 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="169c8-114">Create an instance of an swapshiftschangerequest object.</span></span> |
| [<span data-ttu-id="169c8-115">Get</span><span class="sxs-lookup"><span data-stu-id="169c8-115">Get</span></span>](../api/swapshiftschangerequest-get.md) | [<span data-ttu-id="169c8-116">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="169c8-116">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="169c8-117">读取**swapShiftsChangeRequest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="169c8-117">Read the properties and relationships of a **swapShiftsChangeRequest** object.</span></span> |
|[<span data-ttu-id="169c8-118">批准</span><span class="sxs-lookup"><span data-stu-id="169c8-118">Approve</span></span>](../api/swapshiftschangerequest-approve.md)|<span data-ttu-id="169c8-119">无</span><span class="sxs-lookup"><span data-stu-id="169c8-119">None</span></span>|<span data-ttu-id="169c8-120">批准 swapshiftschangerequest。</span><span class="sxs-lookup"><span data-stu-id="169c8-120">Approve an swapshiftschangerequest.</span></span> |

## <a name="properties"></a><span data-ttu-id="169c8-121">属性</span><span class="sxs-lookup"><span data-stu-id="169c8-121">Properties</span></span>

| <span data-ttu-id="169c8-122">属性</span><span class="sxs-lookup"><span data-stu-id="169c8-122">Property</span></span>     | <span data-ttu-id="169c8-123">类型</span><span class="sxs-lookup"><span data-stu-id="169c8-123">Type</span></span>        | <span data-ttu-id="169c8-124">Description</span><span class="sxs-lookup"><span data-stu-id="169c8-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="169c8-125">recipientShiftId</span><span class="sxs-lookup"><span data-stu-id="169c8-125">recipientShiftId</span></span>|<span data-ttu-id="169c8-126">String</span><span class="sxs-lookup"><span data-stu-id="169c8-126">String</span></span>|<span data-ttu-id="169c8-127">交换请求的收件人的 ID。</span><span class="sxs-lookup"><span data-stu-id="169c8-127">ID of the recipient of the swap request.</span></span> <span data-ttu-id="169c8-128">这是请求要交换的用户。</span><span class="sxs-lookup"><span data-stu-id="169c8-128">This is the user with whom the request is to swap.</span></span>|

## <a name="relationships"></a><span data-ttu-id="169c8-129">关系</span><span class="sxs-lookup"><span data-stu-id="169c8-129">Relationships</span></span>

<span data-ttu-id="169c8-130">无。</span><span class="sxs-lookup"><span data-stu-id="169c8-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="169c8-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="169c8-131">JSON representation</span></span>

<span data-ttu-id="169c8-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="169c8-132">The following is a JSON representation of the resource.</span></span>

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
