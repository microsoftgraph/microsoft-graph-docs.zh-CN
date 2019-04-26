---
title: bookingNamedEntity 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c9dc533360d28fc470a3a00528a20cea1b7ea551
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328190"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="01027-104">bookingNamedEntity 资源类型</span><span class="sxs-lookup"><span data-stu-id="01027-104">bookingNamedEntity resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="01027-105">这是 Microsoft 预订实体的基本类型, 可提供显示名称, 例如, [bookingBusiness](bookingbusiness.md)、 [bookingPerson](bookingperson.md)、 [bookingService](bookingservice.md)。</span><span class="sxs-lookup"><span data-stu-id="01027-105">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="01027-106">属性</span><span class="sxs-lookup"><span data-stu-id="01027-106">Properties</span></span>
| <span data-ttu-id="01027-107">属性</span><span class="sxs-lookup"><span data-stu-id="01027-107">Property</span></span>     | <span data-ttu-id="01027-108">类型</span><span class="sxs-lookup"><span data-stu-id="01027-108">Type</span></span>   |<span data-ttu-id="01027-109">说明</span><span class="sxs-lookup"><span data-stu-id="01027-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01027-110">displayName</span><span class="sxs-lookup"><span data-stu-id="01027-110">displayName</span></span>|<span data-ttu-id="01027-111">String</span><span class="sxs-lookup"><span data-stu-id="01027-111">String</span></span>|<span data-ttu-id="01027-112">派生实体的名称, 与客户进行交互。</span><span class="sxs-lookup"><span data-stu-id="01027-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="01027-113">id</span><span class="sxs-lookup"><span data-stu-id="01027-113">id</span></span>|<span data-ttu-id="01027-114">String</span><span class="sxs-lookup"><span data-stu-id="01027-114">String</span></span>| <span data-ttu-id="01027-115">派生实体的 ID。</span><span class="sxs-lookup"><span data-stu-id="01027-115">The ID for the derived entity.</span></span> <span data-ttu-id="01027-116">只读。</span><span class="sxs-lookup"><span data-stu-id="01027-116">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01027-117">关系</span><span class="sxs-lookup"><span data-stu-id="01027-117">Relationships</span></span>
<span data-ttu-id="01027-118">无</span><span class="sxs-lookup"><span data-stu-id="01027-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="01027-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01027-119">JSON representation</span></span>

<span data-ttu-id="01027-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01027-120">The following is a JSON representation of the resource.</span></span>

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
