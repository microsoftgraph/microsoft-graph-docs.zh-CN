---
title: oneNoteIdentity 资源类型
description: '**即将提供的支持**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: f1b03ad907a0b8f6f3cf2674d74f1ee8722357ea
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642133"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="c9e2b-103">oneNoteIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9e2b-103">oneNoteIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9e2b-104">**即将提供的支持**</span><span class="sxs-lookup"><span data-stu-id="c9e2b-104">**Support coming soon**</span></span>

<span data-ttu-id="c9e2b-105">OneNoteIdentity 类型表示_用户_的标识。</span><span class="sxs-lookup"><span data-stu-id="c9e2b-105">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="c9e2b-106">将在将来，与[标识](identity.md)合并此类型</span><span class="sxs-lookup"><span data-stu-id="c9e2b-106">In future, this type will be merged with [Identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="c9e2b-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9e2b-107">JSON representation</span></span>

<span data-ttu-id="c9e2b-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9e2b-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a><span data-ttu-id="c9e2b-109">属性</span><span class="sxs-lookup"><span data-stu-id="c9e2b-109">Properties</span></span>
| <span data-ttu-id="c9e2b-110">属性</span><span class="sxs-lookup"><span data-stu-id="c9e2b-110">Property</span></span>     | <span data-ttu-id="c9e2b-111">类型</span><span class="sxs-lookup"><span data-stu-id="c9e2b-111">Type</span></span>   |<span data-ttu-id="c9e2b-112">说明</span><span class="sxs-lookup"><span data-stu-id="c9e2b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9e2b-113">displayName</span><span class="sxs-lookup"><span data-stu-id="c9e2b-113">displayName</span></span>|<span data-ttu-id="c9e2b-114">string</span><span class="sxs-lookup"><span data-stu-id="c9e2b-114">string</span></span>|<span data-ttu-id="c9e2b-115">标识的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c9e2b-115">The identity's display name.</span></span>|
|<span data-ttu-id="c9e2b-116">id</span><span class="sxs-lookup"><span data-stu-id="c9e2b-116">id</span></span>|<span data-ttu-id="c9e2b-117">string</span><span class="sxs-lookup"><span data-stu-id="c9e2b-117">string</span></span>|<span data-ttu-id="c9e2b-118">身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c9e2b-118">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteidentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
