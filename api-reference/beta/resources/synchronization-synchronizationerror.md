---
title: synchronizationError 资源类型
description: 代表同步过程中发生的错误。
localization_priority: Normal
ms.openlocfilehash: f37dca5b65a67eb36b2b6a130eee8feb692cd271
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513170"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="61f8b-103">synchronizationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="61f8b-103">synchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61f8b-104">代表同步过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="61f8b-104">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="61f8b-105">属性</span><span class="sxs-lookup"><span data-stu-id="61f8b-105">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="61f8b-106">属性</span><span class="sxs-lookup"><span data-stu-id="61f8b-106">Property</span></span>     | <span data-ttu-id="61f8b-107">类型</span><span class="sxs-lookup"><span data-stu-id="61f8b-107">Type</span></span>   |<span data-ttu-id="61f8b-108">说明</span><span class="sxs-lookup"><span data-stu-id="61f8b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61f8b-109">code</span><span class="sxs-lookup"><span data-stu-id="61f8b-109">code</span></span>|<span data-ttu-id="61f8b-110">String</span><span class="sxs-lookup"><span data-stu-id="61f8b-110">String</span></span>||
|<span data-ttu-id="61f8b-111">message</span><span class="sxs-lookup"><span data-stu-id="61f8b-111">message</span></span>|<span data-ttu-id="61f8b-112">String</span><span class="sxs-lookup"><span data-stu-id="61f8b-112">String</span></span>||
|<span data-ttu-id="61f8b-113">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="61f8b-113">tenantActionable</span></span>|<span data-ttu-id="61f8b-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="61f8b-114">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="61f8b-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61f8b-115">JSON representation</span></span>

<span data-ttu-id="61f8b-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61f8b-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
