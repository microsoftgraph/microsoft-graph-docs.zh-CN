---
title: bookingCustomer 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 864635014b3e215dabd11896922ca9e73a5e8cb9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974167"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="05d82-104">bookingCustomer 资源类型</span><span class="sxs-lookup"><span data-stu-id="05d82-104">bookingCustomer resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="05d82-105">表示[bookingBusiness](bookingbusiness.md)的客户。</span><span class="sxs-lookup"><span data-stu-id="05d82-105">Represents a customer of a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="05d82-106">方法</span><span class="sxs-lookup"><span data-stu-id="05d82-106">Methods</span></span>

| <span data-ttu-id="05d82-107">方法</span><span class="sxs-lookup"><span data-stu-id="05d82-107">Method</span></span>           | <span data-ttu-id="05d82-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="05d82-108">Return Type</span></span>    |<span data-ttu-id="05d82-109">说明</span><span class="sxs-lookup"><span data-stu-id="05d82-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="05d82-110">列出客户</span><span class="sxs-lookup"><span data-stu-id="05d82-110">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="05d82-111">[bookingCustomer](bookingcustomer.md)集合</span><span class="sxs-lookup"><span data-stu-id="05d82-111">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="05d82-112">获取**bookingCustomer**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="05d82-112">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="05d82-113">创建 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="05d82-113">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="05d82-114">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="05d82-114">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="05d82-115">创建新的**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="05d82-115">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="05d82-116">获取 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="05d82-116">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="05d82-117">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="05d82-117">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="05d82-118">读取**bookingCustomer**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="05d82-118">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="05d82-119">更新</span><span class="sxs-lookup"><span data-stu-id="05d82-119">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="05d82-120">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="05d82-120">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="05d82-121">更新**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="05d82-121">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="05d82-122">删除</span><span class="sxs-lookup"><span data-stu-id="05d82-122">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="05d82-123">无</span><span class="sxs-lookup"><span data-stu-id="05d82-123">None</span></span> |<span data-ttu-id="05d82-124">删除**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="05d82-124">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="05d82-125">属性</span><span class="sxs-lookup"><span data-stu-id="05d82-125">Properties</span></span>
| <span data-ttu-id="05d82-126">属性</span><span class="sxs-lookup"><span data-stu-id="05d82-126">Property</span></span>     | <span data-ttu-id="05d82-127">类型</span><span class="sxs-lookup"><span data-stu-id="05d82-127">Type</span></span>   |<span data-ttu-id="05d82-128">说明</span><span class="sxs-lookup"><span data-stu-id="05d82-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05d82-129">displayName</span><span class="sxs-lookup"><span data-stu-id="05d82-129">displayName</span></span>|<span data-ttu-id="05d82-130">字符串</span><span class="sxs-lookup"><span data-stu-id="05d82-130">String</span></span>|<span data-ttu-id="05d82-131">客户的名称。</span><span class="sxs-lookup"><span data-stu-id="05d82-131">The name of the customer.</span></span>|
|<span data-ttu-id="05d82-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="05d82-132">emailAddress</span></span>|<span data-ttu-id="05d82-133">String</span><span class="sxs-lookup"><span data-stu-id="05d82-133">String</span></span>|<span data-ttu-id="05d82-134">客户的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="05d82-134">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="05d82-135">id</span><span class="sxs-lookup"><span data-stu-id="05d82-135">id</span></span>|<span data-ttu-id="05d82-136">String</span><span class="sxs-lookup"><span data-stu-id="05d82-136">String</span></span>| <span data-ttu-id="05d82-137">客户的 ID。</span><span class="sxs-lookup"><span data-stu-id="05d82-137">The ID of the customer.</span></span> <span data-ttu-id="05d82-138">只读。</span><span class="sxs-lookup"><span data-stu-id="05d82-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05d82-139">关系</span><span class="sxs-lookup"><span data-stu-id="05d82-139">Relationships</span></span>
<span data-ttu-id="05d82-140">无</span><span class="sxs-lookup"><span data-stu-id="05d82-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="05d82-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05d82-141">JSON representation</span></span>

<span data-ttu-id="05d82-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05d82-142">The following is a JSON representation of the resource.</span></span>

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
