---
title: bookingPerson 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: e39fbbf12909e7a4d29c95e22896df081522a7d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990108"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="de4e3-104">bookingPerson 资源类型</span><span class="sxs-lookup"><span data-stu-id="de4e3-104">bookingPerson resource type</span></span>

 > <span data-ttu-id="de4e3-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="de4e3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de4e3-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="de4e3-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="de4e3-107">这是 Microsoft 预订业务，可以是[bookingCustomer](bookingcustomer.md)或[bookingStaffMember](bookingstaffmember.md)中的人员的基类型。</span><span class="sxs-lookup"><span data-stu-id="de4e3-107">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="de4e3-108">属性</span><span class="sxs-lookup"><span data-stu-id="de4e3-108">Properties</span></span>
| <span data-ttu-id="de4e3-109">属性</span><span class="sxs-lookup"><span data-stu-id="de4e3-109">Property</span></span>     | <span data-ttu-id="de4e3-110">类型</span><span class="sxs-lookup"><span data-stu-id="de4e3-110">Type</span></span>   |<span data-ttu-id="de4e3-111">说明</span><span class="sxs-lookup"><span data-stu-id="de4e3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de4e3-112">displayName</span><span class="sxs-lookup"><span data-stu-id="de4e3-112">displayName</span></span>|<span data-ttu-id="de4e3-113">字符串</span><span class="sxs-lookup"><span data-stu-id="de4e3-113">String</span></span>|<span data-ttu-id="de4e3-114">派生实体，哪些接口与客户的名称。</span><span class="sxs-lookup"><span data-stu-id="de4e3-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="de4e3-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="de4e3-115">emailAddress</span></span>|<span data-ttu-id="de4e3-116">String</span><span class="sxs-lookup"><span data-stu-id="de4e3-116">String</span></span>|<span data-ttu-id="de4e3-117">人员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="de4e3-117">The email address of the person.</span></span>|
|<span data-ttu-id="de4e3-118">id</span><span class="sxs-lookup"><span data-stu-id="de4e3-118">id</span></span>|<span data-ttu-id="de4e3-119">字符串</span><span class="sxs-lookup"><span data-stu-id="de4e3-119">String</span></span>| <span data-ttu-id="de4e3-120">派生实体的 ID。</span><span class="sxs-lookup"><span data-stu-id="de4e3-120">The ID for the derived entity.</span></span> <span data-ttu-id="de4e3-121">只读。</span><span class="sxs-lookup"><span data-stu-id="de4e3-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de4e3-122">Relationships</span><span class="sxs-lookup"><span data-stu-id="de4e3-122">Relationships</span></span>
<span data-ttu-id="de4e3-123">无</span><span class="sxs-lookup"><span data-stu-id="de4e3-123">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="de4e3-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de4e3-124">JSON representation</span></span>

<span data-ttu-id="de4e3-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de4e3-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingPerson"
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
  "description": "bookingPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
