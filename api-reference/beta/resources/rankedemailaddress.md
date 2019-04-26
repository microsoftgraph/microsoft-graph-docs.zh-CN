---
title: rankedEmailAddress 资源类型
description: 表示排名排名的电子邮件地址。
localization_priority: Normal
ms.openlocfilehash: 0c92f46c587b4f615b640e47b8d82a33aefc5e50
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344097"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="6bfdd-103">rankedEmailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="6bfdd-103">rankedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bfdd-104">表示排名排名的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="6bfdd-104">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="6bfdd-105">属性</span><span class="sxs-lookup"><span data-stu-id="6bfdd-105">Properties</span></span>
| <span data-ttu-id="6bfdd-106">属性</span><span class="sxs-lookup"><span data-stu-id="6bfdd-106">Property</span></span>     | <span data-ttu-id="6bfdd-107">类型</span><span class="sxs-lookup"><span data-stu-id="6bfdd-107">Type</span></span>   |<span data-ttu-id="6bfdd-108">说明</span><span class="sxs-lookup"><span data-stu-id="6bfdd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6bfdd-109">address</span><span class="sxs-lookup"><span data-stu-id="6bfdd-109">address</span></span>|<span data-ttu-id="6bfdd-110">string</span><span class="sxs-lookup"><span data-stu-id="6bfdd-110">string</span></span>|<span data-ttu-id="6bfdd-111">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="6bfdd-111">The email address.</span></span>|
|<span data-ttu-id="6bfdd-112">排名</span><span class="sxs-lookup"><span data-stu-id="6bfdd-112">rank</span></span>|<span data-ttu-id="6bfdd-113">double</span><span class="sxs-lookup"><span data-stu-id="6bfdd-113">double</span></span>|<span data-ttu-id="6bfdd-114">电子邮件地址的排名。</span><span class="sxs-lookup"><span data-stu-id="6bfdd-114">The rank of the email address.</span></span> <span data-ttu-id="6bfdd-115">rank 用作排序关键字, 相对于其他返回的结果。</span><span class="sxs-lookup"><span data-stu-id="6bfdd-115">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="6bfdd-116">较高的排名值对应于更相关的结果。</span><span class="sxs-lookup"><span data-stu-id="6bfdd-116">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="6bfdd-117">相关性取决于沟通、协作和业务关系信号。</span><span class="sxs-lookup"><span data-stu-id="6bfdd-117">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6bfdd-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6bfdd-118">JSON representation</span></span>

<span data-ttu-id="6bfdd-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6bfdd-119">Here is a JSON representation of the resource.</span></span>

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
