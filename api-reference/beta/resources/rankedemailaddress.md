---
title: rankedEmailAddress 资源类型
description: 表示排名排名的电子邮件地址。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: AAmatino
ms.openlocfilehash: f0311b379d2768a2dc704730b7547334e5a64c97
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811418"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="02836-103">rankedEmailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="02836-103">rankedEmailAddress resource type</span></span>

<span data-ttu-id="02836-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02836-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02836-105">表示排名排名的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="02836-105">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="02836-106">属性</span><span class="sxs-lookup"><span data-stu-id="02836-106">Properties</span></span>
| <span data-ttu-id="02836-107">属性</span><span class="sxs-lookup"><span data-stu-id="02836-107">Property</span></span>     | <span data-ttu-id="02836-108">类型</span><span class="sxs-lookup"><span data-stu-id="02836-108">Type</span></span>   |<span data-ttu-id="02836-109">说明</span><span class="sxs-lookup"><span data-stu-id="02836-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02836-110">address</span><span class="sxs-lookup"><span data-stu-id="02836-110">address</span></span>|<span data-ttu-id="02836-111">string</span><span class="sxs-lookup"><span data-stu-id="02836-111">string</span></span>|<span data-ttu-id="02836-112">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="02836-112">The email address.</span></span>|
|<span data-ttu-id="02836-113">排名</span><span class="sxs-lookup"><span data-stu-id="02836-113">rank</span></span>|<span data-ttu-id="02836-114">double</span><span class="sxs-lookup"><span data-stu-id="02836-114">double</span></span>|<span data-ttu-id="02836-115">电子邮件地址的排名。</span><span class="sxs-lookup"><span data-stu-id="02836-115">The rank of the email address.</span></span> <span data-ttu-id="02836-116">Rank 用作排序关键字，相对于其他返回的结果。</span><span class="sxs-lookup"><span data-stu-id="02836-116">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="02836-117">较高的排名值对应于更相关的结果。</span><span class="sxs-lookup"><span data-stu-id="02836-117">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="02836-118">相关性取决于沟通、协作和业务关系信号。</span><span class="sxs-lookup"><span data-stu-id="02836-118">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02836-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02836-119">JSON representation</span></span>

<span data-ttu-id="02836-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02836-120">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
