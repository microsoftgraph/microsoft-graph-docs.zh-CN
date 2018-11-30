---
title: bookingNamedEntity 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: 1d82fcf6fcf7ffad6e60baea3f3e1118ec60345d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041942"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="34ef7-104">bookingNamedEntity 资源类型</span><span class="sxs-lookup"><span data-stu-id="34ef7-104">bookingNamedEntity resource type</span></span>

 > <span data-ttu-id="34ef7-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="34ef7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34ef7-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="34ef7-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="34ef7-107">这是提供显示名称，例如 Microsoft 预订实体[bookingBusiness](bookingbusiness.md)、 [bookingPerson](bookingperson.md)、 [bookingService](bookingservice.md)的基类型。</span><span class="sxs-lookup"><span data-stu-id="34ef7-107">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="34ef7-108">属性</span><span class="sxs-lookup"><span data-stu-id="34ef7-108">Properties</span></span>
| <span data-ttu-id="34ef7-109">属性</span><span class="sxs-lookup"><span data-stu-id="34ef7-109">Property</span></span>     | <span data-ttu-id="34ef7-110">类型</span><span class="sxs-lookup"><span data-stu-id="34ef7-110">Type</span></span>   |<span data-ttu-id="34ef7-111">说明</span><span class="sxs-lookup"><span data-stu-id="34ef7-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34ef7-112">displayName</span><span class="sxs-lookup"><span data-stu-id="34ef7-112">displayName</span></span>|<span data-ttu-id="34ef7-113">字符串</span><span class="sxs-lookup"><span data-stu-id="34ef7-113">String</span></span>|<span data-ttu-id="34ef7-114">派生实体，哪些接口与客户的名称。</span><span class="sxs-lookup"><span data-stu-id="34ef7-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="34ef7-115">id</span><span class="sxs-lookup"><span data-stu-id="34ef7-115">id</span></span>|<span data-ttu-id="34ef7-116">字符串</span><span class="sxs-lookup"><span data-stu-id="34ef7-116">String</span></span>| <span data-ttu-id="34ef7-117">派生实体的 ID。</span><span class="sxs-lookup"><span data-stu-id="34ef7-117">The ID for the derived entity.</span></span> <span data-ttu-id="34ef7-118">只读。</span><span class="sxs-lookup"><span data-stu-id="34ef7-118">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34ef7-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="34ef7-119">Relationships</span></span>
<span data-ttu-id="34ef7-120">无</span><span class="sxs-lookup"><span data-stu-id="34ef7-120">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="34ef7-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34ef7-121">JSON representation</span></span>

<span data-ttu-id="34ef7-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34ef7-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingNamedEntity"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingNamedEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->