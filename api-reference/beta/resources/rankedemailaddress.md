---
title: rankedEmailAddress 资源类型
description: 表示排名排名的电子邮件地址。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bdba5af83357737c77e3b5c441703e404f971587
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521276"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="92698-103">rankedEmailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="92698-103">rankedEmailAddress resource type</span></span>

<span data-ttu-id="92698-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="92698-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92698-105">表示排名排名的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="92698-105">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="92698-106">属性</span><span class="sxs-lookup"><span data-stu-id="92698-106">Properties</span></span>
| <span data-ttu-id="92698-107">属性</span><span class="sxs-lookup"><span data-stu-id="92698-107">Property</span></span>     | <span data-ttu-id="92698-108">类型</span><span class="sxs-lookup"><span data-stu-id="92698-108">Type</span></span>   |<span data-ttu-id="92698-109">说明</span><span class="sxs-lookup"><span data-stu-id="92698-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92698-110">address</span><span class="sxs-lookup"><span data-stu-id="92698-110">address</span></span>|<span data-ttu-id="92698-111">string</span><span class="sxs-lookup"><span data-stu-id="92698-111">string</span></span>|<span data-ttu-id="92698-112">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="92698-112">The email address.</span></span>|
|<span data-ttu-id="92698-113">排名</span><span class="sxs-lookup"><span data-stu-id="92698-113">rank</span></span>|<span data-ttu-id="92698-114">double</span><span class="sxs-lookup"><span data-stu-id="92698-114">double</span></span>|<span data-ttu-id="92698-115">电子邮件地址的排名。</span><span class="sxs-lookup"><span data-stu-id="92698-115">The rank of the email address.</span></span> <span data-ttu-id="92698-116">Rank 用作排序关键字，相对于其他返回的结果。</span><span class="sxs-lookup"><span data-stu-id="92698-116">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="92698-117">较高的排名值对应于更相关的结果。</span><span class="sxs-lookup"><span data-stu-id="92698-117">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="92698-118">相关性取决于沟通、协作和业务关系信号。</span><span class="sxs-lookup"><span data-stu-id="92698-118">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92698-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92698-119">JSON representation</span></span>

<span data-ttu-id="92698-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92698-120">Here is a JSON representation of the resource.</span></span>

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
