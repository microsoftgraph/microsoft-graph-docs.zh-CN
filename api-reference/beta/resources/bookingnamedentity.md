---
title: bookingNamedEntity 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 3302f364b3f16dc6327b9a1e9ab74161e122ebfb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071778"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="3926f-104">bookingNamedEntity 资源类型</span><span class="sxs-lookup"><span data-stu-id="3926f-104">bookingNamedEntity resource type</span></span>

<span data-ttu-id="3926f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3926f-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="3926f-106">这是 Microsoft 预订实体的基本类型，可提供显示名称，例如， [bookingBusiness](bookingbusiness.md)、 [bookingPerson](bookingperson.md)、 [bookingService](bookingservice.md)。</span><span class="sxs-lookup"><span data-stu-id="3926f-106">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3926f-107">属性</span><span class="sxs-lookup"><span data-stu-id="3926f-107">Properties</span></span>
| <span data-ttu-id="3926f-108">属性</span><span class="sxs-lookup"><span data-stu-id="3926f-108">Property</span></span>     | <span data-ttu-id="3926f-109">类型</span><span class="sxs-lookup"><span data-stu-id="3926f-109">Type</span></span>   |<span data-ttu-id="3926f-110">说明</span><span class="sxs-lookup"><span data-stu-id="3926f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3926f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="3926f-111">displayName</span></span>|<span data-ttu-id="3926f-112">String</span><span class="sxs-lookup"><span data-stu-id="3926f-112">String</span></span>|<span data-ttu-id="3926f-113">派生实体的名称，与客户进行交互。</span><span class="sxs-lookup"><span data-stu-id="3926f-113">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="3926f-114">id</span><span class="sxs-lookup"><span data-stu-id="3926f-114">id</span></span>|<span data-ttu-id="3926f-115">String</span><span class="sxs-lookup"><span data-stu-id="3926f-115">String</span></span>| <span data-ttu-id="3926f-116">派生实体的 ID。</span><span class="sxs-lookup"><span data-stu-id="3926f-116">The ID for the derived entity.</span></span> <span data-ttu-id="3926f-117">只读。</span><span class="sxs-lookup"><span data-stu-id="3926f-117">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3926f-118">关系</span><span class="sxs-lookup"><span data-stu-id="3926f-118">Relationships</span></span>
<span data-ttu-id="3926f-119">无</span><span class="sxs-lookup"><span data-stu-id="3926f-119">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3926f-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3926f-120">JSON representation</span></span>

<span data-ttu-id="3926f-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3926f-121">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingNamedEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


