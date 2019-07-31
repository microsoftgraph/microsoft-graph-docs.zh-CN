---
title: bookingNamedEntity 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 7eba40effa1ef5107a97e2acd075dad0c5e350f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013099"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="ae7bf-104">bookingNamedEntity 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae7bf-104">bookingNamedEntity resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="ae7bf-105">这是 Microsoft 预订实体的基本类型, 可提供显示名称, 例如, [bookingBusiness](bookingbusiness.md)、 [bookingPerson](bookingperson.md)、 [bookingService](bookingservice.md)。</span><span class="sxs-lookup"><span data-stu-id="ae7bf-105">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ae7bf-106">属性</span><span class="sxs-lookup"><span data-stu-id="ae7bf-106">Properties</span></span>
| <span data-ttu-id="ae7bf-107">属性</span><span class="sxs-lookup"><span data-stu-id="ae7bf-107">Property</span></span>     | <span data-ttu-id="ae7bf-108">类型</span><span class="sxs-lookup"><span data-stu-id="ae7bf-108">Type</span></span>   |<span data-ttu-id="ae7bf-109">说明</span><span class="sxs-lookup"><span data-stu-id="ae7bf-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae7bf-110">displayName</span><span class="sxs-lookup"><span data-stu-id="ae7bf-110">displayName</span></span>|<span data-ttu-id="ae7bf-111">String</span><span class="sxs-lookup"><span data-stu-id="ae7bf-111">String</span></span>|<span data-ttu-id="ae7bf-112">派生实体的名称, 与客户进行交互。</span><span class="sxs-lookup"><span data-stu-id="ae7bf-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="ae7bf-113">id</span><span class="sxs-lookup"><span data-stu-id="ae7bf-113">id</span></span>|<span data-ttu-id="ae7bf-114">String</span><span class="sxs-lookup"><span data-stu-id="ae7bf-114">String</span></span>| <span data-ttu-id="ae7bf-115">派生实体的 ID。</span><span class="sxs-lookup"><span data-stu-id="ae7bf-115">The ID for the derived entity.</span></span> <span data-ttu-id="ae7bf-116">只读。</span><span class="sxs-lookup"><span data-stu-id="ae7bf-116">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae7bf-117">关系</span><span class="sxs-lookup"><span data-stu-id="ae7bf-117">Relationships</span></span>
<span data-ttu-id="ae7bf-118">无</span><span class="sxs-lookup"><span data-stu-id="ae7bf-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ae7bf-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae7bf-119">JSON representation</span></span>

<span data-ttu-id="ae7bf-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae7bf-120">The following is a JSON representation of the resource.</span></span>

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
