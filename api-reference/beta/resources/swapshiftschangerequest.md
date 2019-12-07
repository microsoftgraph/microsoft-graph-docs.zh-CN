---
title: swapShiftsChangeRequest 资源类型
description: 表示向团队中的其他用户交换班次的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 80149a37dfb4d8d900066d11c315d125ff7fd670
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895621"
---
# <a name="swapshiftschangerequest-resource-type"></a><span data-ttu-id="3e856-103">swapShiftsChangeRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e856-103">swapShiftsChangeRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e856-104">表示将[班次](../resources/shift.md)与[团队](../resources/team.md)中的其他用户交换的班次请求类型。</span><span class="sxs-lookup"><span data-stu-id="3e856-104">Represents a type of shift request to swap a [shift](../resources/shift.md) with another user in the [team](../resources/team.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3e856-105">方法</span><span class="sxs-lookup"><span data-stu-id="3e856-105">Methods</span></span>

| <span data-ttu-id="3e856-106">方法</span><span class="sxs-lookup"><span data-stu-id="3e856-106">Method</span></span>       | <span data-ttu-id="3e856-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="3e856-107">Return Type</span></span> | <span data-ttu-id="3e856-108">说明</span><span class="sxs-lookup"><span data-stu-id="3e856-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3e856-109">获取</span><span class="sxs-lookup"><span data-stu-id="3e856-109">Get</span></span>](../api/swapshiftschangerequest-get.md) | [<span data-ttu-id="3e856-110">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="3e856-110">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="3e856-111">读取**swapShiftsChangeRequest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3e856-111">Read the properties and relationships of a **swapShiftsChangeRequest** object.</span></span> |
| [<span data-ttu-id="3e856-112">更新</span><span class="sxs-lookup"><span data-stu-id="3e856-112">Update</span></span>](../api/swapshiftschangerequest-update.md) | [<span data-ttu-id="3e856-113">swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="3e856-113">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="3e856-114">更新**swapShiftsChangeRequest**对象。</span><span class="sxs-lookup"><span data-stu-id="3e856-114">Update a **swapShiftsChangeRequest** object.</span></span> |
| [<span data-ttu-id="3e856-115">删除</span><span class="sxs-lookup"><span data-stu-id="3e856-115">Delete</span></span>](../api/swapshiftschangerequest-delete.md) | <span data-ttu-id="3e856-116">None</span><span class="sxs-lookup"><span data-stu-id="3e856-116">None</span></span> | <span data-ttu-id="3e856-117">删除**swapShiftsChangeRequest**对象。</span><span class="sxs-lookup"><span data-stu-id="3e856-117">Delete a **swapShiftsChangeRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3e856-118">属性</span><span class="sxs-lookup"><span data-stu-id="3e856-118">Properties</span></span>

| <span data-ttu-id="3e856-119">属性</span><span class="sxs-lookup"><span data-stu-id="3e856-119">Property</span></span>     | <span data-ttu-id="3e856-120">类型</span><span class="sxs-lookup"><span data-stu-id="3e856-120">Type</span></span>        | <span data-ttu-id="3e856-121">说明</span><span class="sxs-lookup"><span data-stu-id="3e856-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3e856-122">recipientShiftId</span><span class="sxs-lookup"><span data-stu-id="3e856-122">recipientShiftId</span></span>|<span data-ttu-id="3e856-123">字符串</span><span class="sxs-lookup"><span data-stu-id="3e856-123">String</span></span>|<span data-ttu-id="3e856-124">交换请求的收件人的 ID。</span><span class="sxs-lookup"><span data-stu-id="3e856-124">ID of the recipient of the swap request.</span></span> <span data-ttu-id="3e856-125">这是请求要交换的用户。</span><span class="sxs-lookup"><span data-stu-id="3e856-125">This is the user with whom the request is to swap.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e856-126">关系</span><span class="sxs-lookup"><span data-stu-id="3e856-126">Relationships</span></span>

<span data-ttu-id="3e856-127">无。</span><span class="sxs-lookup"><span data-stu-id="3e856-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e856-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e856-128">JSON representation</span></span>

<span data-ttu-id="3e856-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e856-129">The following is a JSON representation of the resource.</span></span>

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
