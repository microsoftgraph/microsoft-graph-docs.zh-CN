---
title: bookingCustomer 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 5b527902c5d6e39bb752e07838c6a5e1c3022bb0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071785"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="9592b-104">bookingCustomer 资源类型</span><span class="sxs-lookup"><span data-stu-id="9592b-104">bookingCustomer resource type</span></span>

<span data-ttu-id="9592b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9592b-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="9592b-106">表示 [bookingBusiness](bookingbusiness.md)的客户。</span><span class="sxs-lookup"><span data-stu-id="9592b-106">Represents a customer of a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="9592b-107">方法</span><span class="sxs-lookup"><span data-stu-id="9592b-107">Methods</span></span>

| <span data-ttu-id="9592b-108">方法</span><span class="sxs-lookup"><span data-stu-id="9592b-108">Method</span></span>           | <span data-ttu-id="9592b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9592b-109">Return Type</span></span>    |<span data-ttu-id="9592b-110">说明</span><span class="sxs-lookup"><span data-stu-id="9592b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9592b-111">列出客户</span><span class="sxs-lookup"><span data-stu-id="9592b-111">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="9592b-112">[bookingCustomer](bookingcustomer.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9592b-112">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="9592b-113">获取 **bookingCustomer** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="9592b-113">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="9592b-114">创建 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="9592b-114">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="9592b-115">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="9592b-115">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="9592b-116">创建新的 **bookingCustomer** 对象。</span><span class="sxs-lookup"><span data-stu-id="9592b-116">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="9592b-117">获取 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="9592b-117">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="9592b-118">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="9592b-118">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="9592b-119">读取 **bookingCustomer** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9592b-119">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="9592b-120">更新</span><span class="sxs-lookup"><span data-stu-id="9592b-120">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="9592b-121">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="9592b-121">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="9592b-122">更新 **bookingCustomer** 对象。</span><span class="sxs-lookup"><span data-stu-id="9592b-122">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="9592b-123">删除</span><span class="sxs-lookup"><span data-stu-id="9592b-123">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="9592b-124">无</span><span class="sxs-lookup"><span data-stu-id="9592b-124">None</span></span> |<span data-ttu-id="9592b-125">删除 **bookingCustomer** 对象。</span><span class="sxs-lookup"><span data-stu-id="9592b-125">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9592b-126">属性</span><span class="sxs-lookup"><span data-stu-id="9592b-126">Properties</span></span>
| <span data-ttu-id="9592b-127">属性</span><span class="sxs-lookup"><span data-stu-id="9592b-127">Property</span></span>     | <span data-ttu-id="9592b-128">类型</span><span class="sxs-lookup"><span data-stu-id="9592b-128">Type</span></span>   |<span data-ttu-id="9592b-129">说明</span><span class="sxs-lookup"><span data-stu-id="9592b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9592b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="9592b-130">displayName</span></span>|<span data-ttu-id="9592b-131">String</span><span class="sxs-lookup"><span data-stu-id="9592b-131">String</span></span>|<span data-ttu-id="9592b-132">客户的名称。</span><span class="sxs-lookup"><span data-stu-id="9592b-132">The name of the customer.</span></span>|
|<span data-ttu-id="9592b-133">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9592b-133">emailAddress</span></span>|<span data-ttu-id="9592b-134">String</span><span class="sxs-lookup"><span data-stu-id="9592b-134">String</span></span>|<span data-ttu-id="9592b-135">客户的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="9592b-135">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="9592b-136">id</span><span class="sxs-lookup"><span data-stu-id="9592b-136">id</span></span>|<span data-ttu-id="9592b-137">String</span><span class="sxs-lookup"><span data-stu-id="9592b-137">String</span></span>| <span data-ttu-id="9592b-138">客户的 ID。</span><span class="sxs-lookup"><span data-stu-id="9592b-138">The ID of the customer.</span></span> <span data-ttu-id="9592b-139">只读。</span><span class="sxs-lookup"><span data-stu-id="9592b-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9592b-140">关系</span><span class="sxs-lookup"><span data-stu-id="9592b-140">Relationships</span></span>
<span data-ttu-id="9592b-141">无</span><span class="sxs-lookup"><span data-stu-id="9592b-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9592b-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9592b-142">JSON representation</span></span>

<span data-ttu-id="9592b-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9592b-143">The following is a JSON representation of the resource.</span></span>

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


