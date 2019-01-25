---
title: bookingCustomer 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cd4991b28f1dee0ba647a7f95b70817beffbef95
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522215"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="4011b-104">bookingCustomer 资源类型</span><span class="sxs-lookup"><span data-stu-id="4011b-104">bookingCustomer resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="4011b-105">代表[bookingBsiness](bookingbusiness.md)客户。</span><span class="sxs-lookup"><span data-stu-id="4011b-105">Represents a customer of a [bookingBsiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="4011b-106">方法</span><span class="sxs-lookup"><span data-stu-id="4011b-106">Methods</span></span>

| <span data-ttu-id="4011b-107">方法</span><span class="sxs-lookup"><span data-stu-id="4011b-107">Method</span></span>           | <span data-ttu-id="4011b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4011b-108">Return Type</span></span>    |<span data-ttu-id="4011b-109">说明</span><span class="sxs-lookup"><span data-stu-id="4011b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4011b-110">列出的客户</span><span class="sxs-lookup"><span data-stu-id="4011b-110">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="4011b-111">[bookingCustomer](bookingcustomer.md)集合</span><span class="sxs-lookup"><span data-stu-id="4011b-111">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="4011b-112">获取**bookingCustomer**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="4011b-112">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="4011b-113">创建 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="4011b-113">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="4011b-114">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="4011b-114">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="4011b-115">创建新的**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="4011b-115">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="4011b-116">获取 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="4011b-116">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="4011b-117">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="4011b-117">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="4011b-118">读取的属性和**bookingCustomer**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="4011b-118">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="4011b-119">Update</span><span class="sxs-lookup"><span data-stu-id="4011b-119">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="4011b-120">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="4011b-120">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="4011b-121">更新**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="4011b-121">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="4011b-122">删除</span><span class="sxs-lookup"><span data-stu-id="4011b-122">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="4011b-123">无</span><span class="sxs-lookup"><span data-stu-id="4011b-123">None</span></span> |<span data-ttu-id="4011b-124">删除**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="4011b-124">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4011b-125">属性</span><span class="sxs-lookup"><span data-stu-id="4011b-125">Properties</span></span>
| <span data-ttu-id="4011b-126">属性</span><span class="sxs-lookup"><span data-stu-id="4011b-126">Property</span></span>     | <span data-ttu-id="4011b-127">类型</span><span class="sxs-lookup"><span data-stu-id="4011b-127">Type</span></span>   |<span data-ttu-id="4011b-128">说明</span><span class="sxs-lookup"><span data-stu-id="4011b-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4011b-129">displayName</span><span class="sxs-lookup"><span data-stu-id="4011b-129">displayName</span></span>|<span data-ttu-id="4011b-130">String</span><span class="sxs-lookup"><span data-stu-id="4011b-130">String</span></span>|<span data-ttu-id="4011b-131">客户的名称。</span><span class="sxs-lookup"><span data-stu-id="4011b-131">The name of the customer.</span></span>|
|<span data-ttu-id="4011b-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4011b-132">emailAddress</span></span>|<span data-ttu-id="4011b-133">String</span><span class="sxs-lookup"><span data-stu-id="4011b-133">String</span></span>|<span data-ttu-id="4011b-134">客户的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="4011b-134">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="4011b-135">id</span><span class="sxs-lookup"><span data-stu-id="4011b-135">id</span></span>|<span data-ttu-id="4011b-136">字符串</span><span class="sxs-lookup"><span data-stu-id="4011b-136">String</span></span>| <span data-ttu-id="4011b-137">客户的 ID。</span><span class="sxs-lookup"><span data-stu-id="4011b-137">The ID of the customer.</span></span> <span data-ttu-id="4011b-138">只读。</span><span class="sxs-lookup"><span data-stu-id="4011b-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4011b-139">关系</span><span class="sxs-lookup"><span data-stu-id="4011b-139">Relationships</span></span>
<span data-ttu-id="4011b-140">无</span><span class="sxs-lookup"><span data-stu-id="4011b-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4011b-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4011b-141">JSON representation</span></span>

<span data-ttu-id="4011b-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4011b-142">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingcustomer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
