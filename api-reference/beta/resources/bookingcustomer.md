---
title: bookingCustomer 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: d996c5e06c5c12e3a5115253bb73ed4a7a450258
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645212"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="44a32-104">bookingCustomer 资源类型</span><span class="sxs-lookup"><span data-stu-id="44a32-104">bookingCustomer resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="44a32-105">表示[bookingBusiness](bookingbusiness.md)的客户。</span><span class="sxs-lookup"><span data-stu-id="44a32-105">Represents a customer of a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="44a32-106">方法</span><span class="sxs-lookup"><span data-stu-id="44a32-106">Methods</span></span>

| <span data-ttu-id="44a32-107">方法</span><span class="sxs-lookup"><span data-stu-id="44a32-107">Method</span></span>           | <span data-ttu-id="44a32-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="44a32-108">Return Type</span></span>    |<span data-ttu-id="44a32-109">说明</span><span class="sxs-lookup"><span data-stu-id="44a32-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="44a32-110">列出客户</span><span class="sxs-lookup"><span data-stu-id="44a32-110">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="44a32-111">[bookingCustomer](bookingcustomer.md)集合</span><span class="sxs-lookup"><span data-stu-id="44a32-111">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="44a32-112">获取**bookingCustomer**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="44a32-112">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="44a32-113">创建 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="44a32-113">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="44a32-114">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="44a32-114">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="44a32-115">创建新的**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="44a32-115">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="44a32-116">获取 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="44a32-116">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="44a32-117">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="44a32-117">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="44a32-118">读取**bookingCustomer**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="44a32-118">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="44a32-119">更新</span><span class="sxs-lookup"><span data-stu-id="44a32-119">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="44a32-120">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="44a32-120">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="44a32-121">更新**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="44a32-121">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="44a32-122">删除</span><span class="sxs-lookup"><span data-stu-id="44a32-122">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="44a32-123">无</span><span class="sxs-lookup"><span data-stu-id="44a32-123">None</span></span> |<span data-ttu-id="44a32-124">删除**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="44a32-124">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="44a32-125">属性</span><span class="sxs-lookup"><span data-stu-id="44a32-125">Properties</span></span>
| <span data-ttu-id="44a32-126">属性</span><span class="sxs-lookup"><span data-stu-id="44a32-126">Property</span></span>     | <span data-ttu-id="44a32-127">类型</span><span class="sxs-lookup"><span data-stu-id="44a32-127">Type</span></span>   |<span data-ttu-id="44a32-128">说明</span><span class="sxs-lookup"><span data-stu-id="44a32-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44a32-129">displayName</span><span class="sxs-lookup"><span data-stu-id="44a32-129">displayName</span></span>|<span data-ttu-id="44a32-130">字符串</span><span class="sxs-lookup"><span data-stu-id="44a32-130">String</span></span>|<span data-ttu-id="44a32-131">客户的名称。</span><span class="sxs-lookup"><span data-stu-id="44a32-131">The name of the customer.</span></span>|
|<span data-ttu-id="44a32-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="44a32-132">emailAddress</span></span>|<span data-ttu-id="44a32-133">String</span><span class="sxs-lookup"><span data-stu-id="44a32-133">String</span></span>|<span data-ttu-id="44a32-134">客户的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="44a32-134">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="44a32-135">id</span><span class="sxs-lookup"><span data-stu-id="44a32-135">id</span></span>|<span data-ttu-id="44a32-136">String</span><span class="sxs-lookup"><span data-stu-id="44a32-136">String</span></span>| <span data-ttu-id="44a32-137">客户的 ID。</span><span class="sxs-lookup"><span data-stu-id="44a32-137">The ID of the customer.</span></span> <span data-ttu-id="44a32-138">只读。</span><span class="sxs-lookup"><span data-stu-id="44a32-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44a32-139">关系</span><span class="sxs-lookup"><span data-stu-id="44a32-139">Relationships</span></span>
<span data-ttu-id="44a32-140">无</span><span class="sxs-lookup"><span data-stu-id="44a32-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="44a32-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44a32-141">JSON representation</span></span>

<span data-ttu-id="44a32-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44a32-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCustomer"
}-->

```json
{
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingCustomer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
