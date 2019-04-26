---
title: rankedEmailAddress 资源类型
description: 表示排名排名的电子邮件地址。
localization_priority: Normal
ms.openlocfilehash: 938afc0de208fd3cdbd0cfec299d01ada9d4f592
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563249"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="dcbc2-103">rankedEmailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="dcbc2-103">rankedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcbc2-104">表示排名排名的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="dcbc2-104">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="dcbc2-105">属性</span><span class="sxs-lookup"><span data-stu-id="dcbc2-105">Properties</span></span>
| <span data-ttu-id="dcbc2-106">属性</span><span class="sxs-lookup"><span data-stu-id="dcbc2-106">Property</span></span>     | <span data-ttu-id="dcbc2-107">类型</span><span class="sxs-lookup"><span data-stu-id="dcbc2-107">Type</span></span>   |<span data-ttu-id="dcbc2-108">说明</span><span class="sxs-lookup"><span data-stu-id="dcbc2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dcbc2-109">address</span><span class="sxs-lookup"><span data-stu-id="dcbc2-109">address</span></span>|<span data-ttu-id="dcbc2-110">string</span><span class="sxs-lookup"><span data-stu-id="dcbc2-110">string</span></span>|<span data-ttu-id="dcbc2-111">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="dcbc2-111">The email address.</span></span>|
|<span data-ttu-id="dcbc2-112">排名</span><span class="sxs-lookup"><span data-stu-id="dcbc2-112">rank</span></span>|<span data-ttu-id="dcbc2-113">double</span><span class="sxs-lookup"><span data-stu-id="dcbc2-113">double</span></span>|<span data-ttu-id="dcbc2-114">电子邮件地址的排名。</span><span class="sxs-lookup"><span data-stu-id="dcbc2-114">The rank of the email address.</span></span> <span data-ttu-id="dcbc2-115">rank 用作排序关键字, 相对于其他返回的结果。</span><span class="sxs-lookup"><span data-stu-id="dcbc2-115">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="dcbc2-116">较高的排名值对应于更相关的结果。</span><span class="sxs-lookup"><span data-stu-id="dcbc2-116">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="dcbc2-117">相关性取决于沟通、协作和业务关系信号。</span><span class="sxs-lookup"><span data-stu-id="dcbc2-117">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dcbc2-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dcbc2-118">JSON representation</span></span>

<span data-ttu-id="dcbc2-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dcbc2-119">Here is a JSON representation of the resource.</span></span>

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
