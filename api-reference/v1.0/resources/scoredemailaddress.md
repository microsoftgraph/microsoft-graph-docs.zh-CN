---
title: scoredEmailAddress 资源类型
description: 表示经过评分的电子邮件地址。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c16d9b2b6d88f651fa65375f0b8ea9418432cc73
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533807"
---
# <a name="scoredemailaddress-resource-type"></a><span data-ttu-id="bcfd8-103">scoredEmailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="bcfd8-103">scoredEmailAddress resource type</span></span>

<span data-ttu-id="bcfd8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcfd8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bcfd8-105">表示经过评分的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="bcfd8-105">Represents a scored email address.</span></span>


## <a name="properties"></a><span data-ttu-id="bcfd8-106">属性</span><span class="sxs-lookup"><span data-stu-id="bcfd8-106">Properties</span></span>
| <span data-ttu-id="bcfd8-107">属性</span><span class="sxs-lookup"><span data-stu-id="bcfd8-107">Property</span></span>     | <span data-ttu-id="bcfd8-108">类型</span><span class="sxs-lookup"><span data-stu-id="bcfd8-108">Type</span></span>   |<span data-ttu-id="bcfd8-109">说明</span><span class="sxs-lookup"><span data-stu-id="bcfd8-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bcfd8-110">address</span><span class="sxs-lookup"><span data-stu-id="bcfd8-110">address</span></span>|<span data-ttu-id="bcfd8-111">string</span><span class="sxs-lookup"><span data-stu-id="bcfd8-111">string</span></span>|<span data-ttu-id="bcfd8-112">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="bcfd8-112">The email address.</span></span>|
|<span data-ttu-id="bcfd8-113">relevanceScore</span><span class="sxs-lookup"><span data-stu-id="bcfd8-113">relevanceScore</span></span>|<span data-ttu-id="bcfd8-114">double</span><span class="sxs-lookup"><span data-stu-id="bcfd8-114">double</span></span>|<span data-ttu-id="bcfd8-p101">电子邮件地址的相关性评分。相关性评分用作排序关键字，与其他返回的结果相关。相关性评分值越高，对应结果的相关性越高。相关性由用户的通信和协作模式及业务关系决定。</span><span class="sxs-lookup"><span data-stu-id="bcfd8-p101">The relevance score of the email address. A relevance score is used as a sort key, in relation to the other returned results. A higher relevance score value corresponds to a more relevant result. Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bcfd8-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bcfd8-119">JSON representation</span></span>

<span data-ttu-id="bcfd8-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bcfd8-120">Here is a JSON representation of the resource.</span></span>

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
