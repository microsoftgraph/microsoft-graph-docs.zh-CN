---
title: scoredEmailAddress 资源类型
description: 表示经过评分的电子邮件地址。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b8cdcd7a0192bdd97bc096ce06514e75a7184f63
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034592"
---
# <a name="scoredemailaddress-resource-type"></a><span data-ttu-id="3b3d1-103">scoredEmailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b3d1-103">scoredEmailAddress resource type</span></span>

<span data-ttu-id="3b3d1-104">表示经过评分的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="3b3d1-104">Represents a scored email address.</span></span>


## <a name="properties"></a><span data-ttu-id="3b3d1-105">属性</span><span class="sxs-lookup"><span data-stu-id="3b3d1-105">Properties</span></span>
| <span data-ttu-id="3b3d1-106">属性</span><span class="sxs-lookup"><span data-stu-id="3b3d1-106">Property</span></span>     | <span data-ttu-id="3b3d1-107">类型</span><span class="sxs-lookup"><span data-stu-id="3b3d1-107">Type</span></span>   |<span data-ttu-id="3b3d1-108">说明</span><span class="sxs-lookup"><span data-stu-id="3b3d1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b3d1-109">address</span><span class="sxs-lookup"><span data-stu-id="3b3d1-109">address</span></span>|<span data-ttu-id="3b3d1-110">string</span><span class="sxs-lookup"><span data-stu-id="3b3d1-110">string</span></span>|<span data-ttu-id="3b3d1-111">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="3b3d1-111">The email address.</span></span>|
|<span data-ttu-id="3b3d1-112">relevanceScore</span><span class="sxs-lookup"><span data-stu-id="3b3d1-112">relevanceScore</span></span>|<span data-ttu-id="3b3d1-113">double</span><span class="sxs-lookup"><span data-stu-id="3b3d1-113">double</span></span>|<span data-ttu-id="3b3d1-p101">电子邮件地址的相关性评分。相关性评分用作排序关键字，与其他返回的结果相关。相关性评分值越高，对应结果的相关性越高。相关性由用户的通信和协作模式及业务关系决定。</span><span class="sxs-lookup"><span data-stu-id="3b3d1-p101">The relevance score of the email address. A relevance score is used as a sort key, in relation to the other returned results. A higher relevance score value corresponds to a more relevant result. Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3b3d1-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b3d1-118">JSON representation</span></span>

<span data-ttu-id="3b3d1-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b3d1-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scoredEmailAddress"
}-->

```json
{
  "address": "string",
  "relevanceScore": 1024.0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scoredEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
