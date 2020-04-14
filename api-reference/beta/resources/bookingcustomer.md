---
title: bookingCustomer 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 42ad0826cdabbba2c3b26101d93160f71344fc6c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453653"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="b0368-104">bookingCustomer 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0368-104">bookingCustomer resource type</span></span>

<span data-ttu-id="b0368-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0368-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="b0368-106">表示[bookingBusiness](bookingbusiness.md)的客户。</span><span class="sxs-lookup"><span data-stu-id="b0368-106">Represents a customer of a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="b0368-107">方法</span><span class="sxs-lookup"><span data-stu-id="b0368-107">Methods</span></span>

| <span data-ttu-id="b0368-108">方法</span><span class="sxs-lookup"><span data-stu-id="b0368-108">Method</span></span>           | <span data-ttu-id="b0368-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b0368-109">Return Type</span></span>    |<span data-ttu-id="b0368-110">说明</span><span class="sxs-lookup"><span data-stu-id="b0368-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0368-111">列出客户</span><span class="sxs-lookup"><span data-stu-id="b0368-111">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="b0368-112">[bookingCustomer](bookingcustomer.md)集合</span><span class="sxs-lookup"><span data-stu-id="b0368-112">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="b0368-113">获取**bookingCustomer**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="b0368-113">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="b0368-114">创建 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="b0368-114">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="b0368-115">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="b0368-115">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="b0368-116">创建新的**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="b0368-116">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="b0368-117">获取 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="b0368-117">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="b0368-118">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="b0368-118">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="b0368-119">读取**bookingCustomer**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b0368-119">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="b0368-120">更新</span><span class="sxs-lookup"><span data-stu-id="b0368-120">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="b0368-121">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="b0368-121">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="b0368-122">更新**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="b0368-122">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="b0368-123">删除</span><span class="sxs-lookup"><span data-stu-id="b0368-123">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="b0368-124">无</span><span class="sxs-lookup"><span data-stu-id="b0368-124">None</span></span> |<span data-ttu-id="b0368-125">删除**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="b0368-125">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b0368-126">属性</span><span class="sxs-lookup"><span data-stu-id="b0368-126">Properties</span></span>
| <span data-ttu-id="b0368-127">属性</span><span class="sxs-lookup"><span data-stu-id="b0368-127">Property</span></span>     | <span data-ttu-id="b0368-128">类型</span><span class="sxs-lookup"><span data-stu-id="b0368-128">Type</span></span>   |<span data-ttu-id="b0368-129">说明</span><span class="sxs-lookup"><span data-stu-id="b0368-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0368-130">displayName</span><span class="sxs-lookup"><span data-stu-id="b0368-130">displayName</span></span>|<span data-ttu-id="b0368-131">字符串</span><span class="sxs-lookup"><span data-stu-id="b0368-131">String</span></span>|<span data-ttu-id="b0368-132">客户的名称。</span><span class="sxs-lookup"><span data-stu-id="b0368-132">The name of the customer.</span></span>|
|<span data-ttu-id="b0368-133">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b0368-133">emailAddress</span></span>|<span data-ttu-id="b0368-134">String</span><span class="sxs-lookup"><span data-stu-id="b0368-134">String</span></span>|<span data-ttu-id="b0368-135">客户的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="b0368-135">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="b0368-136">id</span><span class="sxs-lookup"><span data-stu-id="b0368-136">id</span></span>|<span data-ttu-id="b0368-137">String</span><span class="sxs-lookup"><span data-stu-id="b0368-137">String</span></span>| <span data-ttu-id="b0368-138">客户的 ID。</span><span class="sxs-lookup"><span data-stu-id="b0368-138">The ID of the customer.</span></span> <span data-ttu-id="b0368-139">只读。</span><span class="sxs-lookup"><span data-stu-id="b0368-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0368-140">关系</span><span class="sxs-lookup"><span data-stu-id="b0368-140">Relationships</span></span>
<span data-ttu-id="b0368-141">无</span><span class="sxs-lookup"><span data-stu-id="b0368-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b0368-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0368-142">JSON representation</span></span>

<span data-ttu-id="b0368-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0368-143">The following is a JSON representation of the resource.</span></span>

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
