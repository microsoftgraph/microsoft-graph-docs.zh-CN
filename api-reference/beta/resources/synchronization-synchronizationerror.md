---
title: synchronizationError 资源类型
description: 表示同步过程中发生的错误。
localization_priority: Normal
ms.openlocfilehash: f37dca5b65a67eb36b2b6a130eee8feb692cd271
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525976"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="28154-103">synchronizationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="28154-103">synchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28154-104">表示同步过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="28154-104">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="28154-105">属性</span><span class="sxs-lookup"><span data-stu-id="28154-105">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="28154-106">属性</span><span class="sxs-lookup"><span data-stu-id="28154-106">Property</span></span>     | <span data-ttu-id="28154-107">类型</span><span class="sxs-lookup"><span data-stu-id="28154-107">Type</span></span>   |<span data-ttu-id="28154-108">说明</span><span class="sxs-lookup"><span data-stu-id="28154-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28154-109">code</span><span class="sxs-lookup"><span data-stu-id="28154-109">code</span></span>|<span data-ttu-id="28154-110">String</span><span class="sxs-lookup"><span data-stu-id="28154-110">String</span></span>||
|<span data-ttu-id="28154-111">message</span><span class="sxs-lookup"><span data-stu-id="28154-111">message</span></span>|<span data-ttu-id="28154-112">String</span><span class="sxs-lookup"><span data-stu-id="28154-112">String</span></span>||
|<span data-ttu-id="28154-113">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="28154-113">tenantActionable</span></span>|<span data-ttu-id="28154-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="28154-114">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="28154-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28154-115">JSON representation</span></span>

<span data-ttu-id="28154-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28154-116">The following is a JSON representation of the resource.</span></span>

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
