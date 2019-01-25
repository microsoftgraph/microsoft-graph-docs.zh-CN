---
title: rankedEmailAddress 资源类型
description: 代表一个排名的电子邮件地址。
localization_priority: Normal
ms.openlocfilehash: 938afc0de208fd3cdbd0cfec299d01ada9d4f592
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510006"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="a5b5c-103">rankedEmailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5b5c-103">rankedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5b5c-104">代表一个排名的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a5b5c-104">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="a5b5c-105">属性</span><span class="sxs-lookup"><span data-stu-id="a5b5c-105">Properties</span></span>
| <span data-ttu-id="a5b5c-106">属性</span><span class="sxs-lookup"><span data-stu-id="a5b5c-106">Property</span></span>     | <span data-ttu-id="a5b5c-107">类型</span><span class="sxs-lookup"><span data-stu-id="a5b5c-107">Type</span></span>   |<span data-ttu-id="a5b5c-108">说明</span><span class="sxs-lookup"><span data-stu-id="a5b5c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5b5c-109">address</span><span class="sxs-lookup"><span data-stu-id="a5b5c-109">address</span></span>|<span data-ttu-id="a5b5c-110">string</span><span class="sxs-lookup"><span data-stu-id="a5b5c-110">string</span></span>|<span data-ttu-id="a5b5c-111">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a5b5c-111">The email address.</span></span>|
|<span data-ttu-id="a5b5c-112">排名</span><span class="sxs-lookup"><span data-stu-id="a5b5c-112">rank</span></span>|<span data-ttu-id="a5b5c-113">double</span><span class="sxs-lookup"><span data-stu-id="a5b5c-113">double</span></span>|<span data-ttu-id="a5b5c-114">电子邮件地址的排名。</span><span class="sxs-lookup"><span data-stu-id="a5b5c-114">The rank of the email address.</span></span> <span data-ttu-id="a5b5c-115">排名用作排序关键字，相对于其他返回的结果。</span><span class="sxs-lookup"><span data-stu-id="a5b5c-115">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="a5b5c-116">较高的排名值对应于更相关的结果。</span><span class="sxs-lookup"><span data-stu-id="a5b5c-116">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="a5b5c-117">相关性取决于沟通、协作和业务关系信号。</span><span class="sxs-lookup"><span data-stu-id="a5b5c-117">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5b5c-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5b5c-118">JSON representation</span></span>

<span data-ttu-id="a5b5c-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5b5c-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rankedEmailAddress"
}-->

```json
{
  "address": "string",
  "rank": 1024
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rankedemailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
