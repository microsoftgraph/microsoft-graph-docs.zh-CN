---
title: 网站资源类型
description: 代表网站。
localization_priority: Normal
ms.openlocfilehash: 3f8aadaf0a6b6beb2394664f04195267062dc9ae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454042"
---
# <a name="website-resource-type"></a><span data-ttu-id="2d30f-103">网站资源类型</span><span class="sxs-lookup"><span data-stu-id="2d30f-103">website resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d30f-104">代表网站。</span><span class="sxs-lookup"><span data-stu-id="2d30f-104">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="2d30f-105">属性</span><span class="sxs-lookup"><span data-stu-id="2d30f-105">Properties</span></span>
| <span data-ttu-id="2d30f-106">属性</span><span class="sxs-lookup"><span data-stu-id="2d30f-106">Property</span></span>     | <span data-ttu-id="2d30f-107">类型</span><span class="sxs-lookup"><span data-stu-id="2d30f-107">Type</span></span>   |<span data-ttu-id="2d30f-108">描述</span><span class="sxs-lookup"><span data-stu-id="2d30f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d30f-109">类型</span><span class="sxs-lookup"><span data-stu-id="2d30f-109">type</span></span>|<span data-ttu-id="2d30f-110">字符串</span><span class="sxs-lookup"><span data-stu-id="2d30f-110">String</span></span>| <span data-ttu-id="2d30f-111">可取值为：`other`、`home`、`work`、`blog` 或 `profile`。</span><span class="sxs-lookup"><span data-stu-id="2d30f-111">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="2d30f-112">address</span><span class="sxs-lookup"><span data-stu-id="2d30f-112">address</span></span>|<span data-ttu-id="2d30f-113">string</span><span class="sxs-lookup"><span data-stu-id="2d30f-113">string</span></span>|<span data-ttu-id="2d30f-114">网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="2d30f-114">The URL of the website.</span></span>|
|<span data-ttu-id="2d30f-115">displayName</span><span class="sxs-lookup"><span data-stu-id="2d30f-115">displayName</span></span>|<span data-ttu-id="2d30f-116">string</span><span class="sxs-lookup"><span data-stu-id="2d30f-116">string</span></span>|<span data-ttu-id="2d30f-117">网站的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2d30f-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d30f-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d30f-118">JSON representation</span></span>

<span data-ttu-id="2d30f-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d30f-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/website.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
