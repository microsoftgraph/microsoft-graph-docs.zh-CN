---
title: bookingNamedEntity 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 1cee769181fdf8dce694050cdbc2658fdf29ece4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515319"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="1aca2-104">bookingNamedEntity 资源类型</span><span class="sxs-lookup"><span data-stu-id="1aca2-104">bookingNamedEntity resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="1aca2-105">这是提供显示名称，例如 Microsoft 预订实体[bookingBusiness](bookingbusiness.md)、 [bookingPerson](bookingperson.md)、 [bookingService](bookingservice.md)的基类型。</span><span class="sxs-lookup"><span data-stu-id="1aca2-105">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1aca2-106">属性</span><span class="sxs-lookup"><span data-stu-id="1aca2-106">Properties</span></span>
| <span data-ttu-id="1aca2-107">属性</span><span class="sxs-lookup"><span data-stu-id="1aca2-107">Property</span></span>     | <span data-ttu-id="1aca2-108">类型</span><span class="sxs-lookup"><span data-stu-id="1aca2-108">Type</span></span>   |<span data-ttu-id="1aca2-109">说明</span><span class="sxs-lookup"><span data-stu-id="1aca2-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1aca2-110">displayName</span><span class="sxs-lookup"><span data-stu-id="1aca2-110">displayName</span></span>|<span data-ttu-id="1aca2-111">String</span><span class="sxs-lookup"><span data-stu-id="1aca2-111">String</span></span>|<span data-ttu-id="1aca2-112">派生实体，哪些接口与客户的名称。</span><span class="sxs-lookup"><span data-stu-id="1aca2-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="1aca2-113">id</span><span class="sxs-lookup"><span data-stu-id="1aca2-113">id</span></span>|<span data-ttu-id="1aca2-114">String</span><span class="sxs-lookup"><span data-stu-id="1aca2-114">String</span></span>| <span data-ttu-id="1aca2-115">派生实体的 ID。</span><span class="sxs-lookup"><span data-stu-id="1aca2-115">The ID for the derived entity.</span></span> <span data-ttu-id="1aca2-116">只读。</span><span class="sxs-lookup"><span data-stu-id="1aca2-116">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1aca2-117">关系</span><span class="sxs-lookup"><span data-stu-id="1aca2-117">Relationships</span></span>
<span data-ttu-id="1aca2-118">无</span><span class="sxs-lookup"><span data-stu-id="1aca2-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1aca2-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1aca2-119">JSON representation</span></span>

<span data-ttu-id="1aca2-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1aca2-120">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingnamedentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
