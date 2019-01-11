---
title: bookingCustomer 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 02439b16235b3ff1560b5a74b15cd6ce2cb3075b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888975"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="aec12-104">bookingCustomer 资源类型</span><span class="sxs-lookup"><span data-stu-id="aec12-104">bookingCustomer resource type</span></span>

 > <span data-ttu-id="aec12-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aec12-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aec12-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aec12-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="aec12-107">代表[bookingBsiness](bookingbusiness.md)客户。</span><span class="sxs-lookup"><span data-stu-id="aec12-107">Represents a customer of a [bookingBsiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="aec12-108">方法</span><span class="sxs-lookup"><span data-stu-id="aec12-108">Methods</span></span>

| <span data-ttu-id="aec12-109">方法</span><span class="sxs-lookup"><span data-stu-id="aec12-109">Method</span></span>           | <span data-ttu-id="aec12-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="aec12-110">Return Type</span></span>    |<span data-ttu-id="aec12-111">说明</span><span class="sxs-lookup"><span data-stu-id="aec12-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aec12-112">列出的客户</span><span class="sxs-lookup"><span data-stu-id="aec12-112">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="aec12-113">[bookingCustomer](bookingcustomer.md)集合</span><span class="sxs-lookup"><span data-stu-id="aec12-113">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="aec12-114">获取**bookingCustomer**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="aec12-114">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="aec12-115">创建 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="aec12-115">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="aec12-116">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="aec12-116">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="aec12-117">创建新的**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="aec12-117">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="aec12-118">获取 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="aec12-118">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="aec12-119">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="aec12-119">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="aec12-120">读取的属性和**bookingCustomer**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="aec12-120">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="aec12-121">Update</span><span class="sxs-lookup"><span data-stu-id="aec12-121">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="aec12-122">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="aec12-122">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="aec12-123">更新**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="aec12-123">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="aec12-124">删除</span><span class="sxs-lookup"><span data-stu-id="aec12-124">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="aec12-125">无</span><span class="sxs-lookup"><span data-stu-id="aec12-125">None</span></span> |<span data-ttu-id="aec12-126">删除**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="aec12-126">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="aec12-127">属性</span><span class="sxs-lookup"><span data-stu-id="aec12-127">Properties</span></span>
| <span data-ttu-id="aec12-128">属性</span><span class="sxs-lookup"><span data-stu-id="aec12-128">Property</span></span>     | <span data-ttu-id="aec12-129">类型</span><span class="sxs-lookup"><span data-stu-id="aec12-129">Type</span></span>   |<span data-ttu-id="aec12-130">说明</span><span class="sxs-lookup"><span data-stu-id="aec12-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aec12-131">displayName</span><span class="sxs-lookup"><span data-stu-id="aec12-131">displayName</span></span>|<span data-ttu-id="aec12-132">字符串</span><span class="sxs-lookup"><span data-stu-id="aec12-132">String</span></span>|<span data-ttu-id="aec12-133">客户的名称。</span><span class="sxs-lookup"><span data-stu-id="aec12-133">The name of the customer.</span></span>|
|<span data-ttu-id="aec12-134">emailAddress</span><span class="sxs-lookup"><span data-stu-id="aec12-134">emailAddress</span></span>|<span data-ttu-id="aec12-135">String</span><span class="sxs-lookup"><span data-stu-id="aec12-135">String</span></span>|<span data-ttu-id="aec12-136">客户的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="aec12-136">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="aec12-137">id</span><span class="sxs-lookup"><span data-stu-id="aec12-137">id</span></span>|<span data-ttu-id="aec12-138">字符串</span><span class="sxs-lookup"><span data-stu-id="aec12-138">String</span></span>| <span data-ttu-id="aec12-139">客户的 ID。</span><span class="sxs-lookup"><span data-stu-id="aec12-139">The ID of the customer.</span></span> <span data-ttu-id="aec12-140">只读。</span><span class="sxs-lookup"><span data-stu-id="aec12-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aec12-141">Relationships</span><span class="sxs-lookup"><span data-stu-id="aec12-141">Relationships</span></span>
<span data-ttu-id="aec12-142">无</span><span class="sxs-lookup"><span data-stu-id="aec12-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="aec12-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aec12-143">JSON representation</span></span>

<span data-ttu-id="aec12-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aec12-144">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingCustomer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
