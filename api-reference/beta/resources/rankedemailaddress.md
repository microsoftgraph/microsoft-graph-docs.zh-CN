---
title: rankedEmailAddress 资源类型
description: 代表一个排名的电子邮件地址。
localization_priority: Normal
ms.openlocfilehash: bb3b906929bddcb52a57a478647000e7e16fa0be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818513"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="08300-103">rankedEmailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="08300-103">rankedEmailAddress resource type</span></span>

> <span data-ttu-id="08300-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="08300-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08300-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="08300-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08300-106">代表一个排名的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="08300-106">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="08300-107">属性</span><span class="sxs-lookup"><span data-stu-id="08300-107">Properties</span></span>
| <span data-ttu-id="08300-108">属性</span><span class="sxs-lookup"><span data-stu-id="08300-108">Property</span></span>     | <span data-ttu-id="08300-109">类型</span><span class="sxs-lookup"><span data-stu-id="08300-109">Type</span></span>   |<span data-ttu-id="08300-110">说明</span><span class="sxs-lookup"><span data-stu-id="08300-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08300-111">address</span><span class="sxs-lookup"><span data-stu-id="08300-111">address</span></span>|<span data-ttu-id="08300-112">string</span><span class="sxs-lookup"><span data-stu-id="08300-112">string</span></span>|<span data-ttu-id="08300-113">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="08300-113">The email address.</span></span>|
|<span data-ttu-id="08300-114">排名</span><span class="sxs-lookup"><span data-stu-id="08300-114">rank</span></span>|<span data-ttu-id="08300-115">double</span><span class="sxs-lookup"><span data-stu-id="08300-115">double</span></span>|<span data-ttu-id="08300-116">电子邮件地址的排名。</span><span class="sxs-lookup"><span data-stu-id="08300-116">The rank of the email address.</span></span> <span data-ttu-id="08300-117">排名用作排序关键字，相对于其他返回的结果。</span><span class="sxs-lookup"><span data-stu-id="08300-117">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="08300-118">较高的排名值对应于更相关的结果。</span><span class="sxs-lookup"><span data-stu-id="08300-118">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="08300-119">相关性取决于沟通、协作和业务关系信号。</span><span class="sxs-lookup"><span data-stu-id="08300-119">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08300-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="08300-120">JSON representation</span></span>

<span data-ttu-id="08300-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08300-121">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
