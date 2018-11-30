---
title: bookingPerson 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: d20f6ee9e14723a80f012cfffb1e4b8214f89739
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046434"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="1aa65-104">bookingPerson 资源类型</span><span class="sxs-lookup"><span data-stu-id="1aa65-104">bookingPerson resource type</span></span>

 > <span data-ttu-id="1aa65-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1aa65-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1aa65-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1aa65-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="1aa65-107">这是 Microsoft 预订业务，可以是[bookingCustomer](bookingcustomer.md)或[bookingStaffMember](bookingstaffmember.md)中的人员的基类型。</span><span class="sxs-lookup"><span data-stu-id="1aa65-107">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1aa65-108">属性</span><span class="sxs-lookup"><span data-stu-id="1aa65-108">Properties</span></span>
| <span data-ttu-id="1aa65-109">属性</span><span class="sxs-lookup"><span data-stu-id="1aa65-109">Property</span></span>     | <span data-ttu-id="1aa65-110">类型</span><span class="sxs-lookup"><span data-stu-id="1aa65-110">Type</span></span>   |<span data-ttu-id="1aa65-111">说明</span><span class="sxs-lookup"><span data-stu-id="1aa65-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1aa65-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1aa65-112">displayName</span></span>|<span data-ttu-id="1aa65-113">字符串</span><span class="sxs-lookup"><span data-stu-id="1aa65-113">String</span></span>|<span data-ttu-id="1aa65-114">派生实体，哪些接口与客户的名称。</span><span class="sxs-lookup"><span data-stu-id="1aa65-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="1aa65-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1aa65-115">emailAddress</span></span>|<span data-ttu-id="1aa65-116">String</span><span class="sxs-lookup"><span data-stu-id="1aa65-116">String</span></span>|<span data-ttu-id="1aa65-117">人员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="1aa65-117">The email address of the person.</span></span>|
|<span data-ttu-id="1aa65-118">id</span><span class="sxs-lookup"><span data-stu-id="1aa65-118">id</span></span>|<span data-ttu-id="1aa65-119">字符串</span><span class="sxs-lookup"><span data-stu-id="1aa65-119">String</span></span>| <span data-ttu-id="1aa65-120">派生实体的 ID。</span><span class="sxs-lookup"><span data-stu-id="1aa65-120">The ID for the derived entity.</span></span> <span data-ttu-id="1aa65-121">只读。</span><span class="sxs-lookup"><span data-stu-id="1aa65-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1aa65-122">Relationships</span><span class="sxs-lookup"><span data-stu-id="1aa65-122">Relationships</span></span>
<span data-ttu-id="1aa65-123">无</span><span class="sxs-lookup"><span data-stu-id="1aa65-123">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1aa65-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1aa65-124">JSON representation</span></span>

<span data-ttu-id="1aa65-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1aa65-125">The following is a JSON representation of the resource.</span></span>

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