---
title: userFeedback 资源类型
description: UserFeedback 类型。
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 661d1f114bc004d5c4fbaafac2ee7e9c1ea3fa5e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046872"
---
# <a name="userfeedback-resource-type"></a><span data-ttu-id="7ad04-103">userFeedback 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ad04-103">userFeedback resource type</span></span>

<span data-ttu-id="7ad04-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="7ad04-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ad04-105">代表用户提供的有关会话质量的终结点的反馈。</span><span class="sxs-lookup"><span data-stu-id="7ad04-105">Represents the feedback provided by the user an endpoint about the quality of the session.</span></span>

## <a name="properties"></a><span data-ttu-id="7ad04-106">属性</span><span class="sxs-lookup"><span data-stu-id="7ad04-106">Properties</span></span>

| <span data-ttu-id="7ad04-107">属性</span><span class="sxs-lookup"><span data-stu-id="7ad04-107">Property</span></span>     | <span data-ttu-id="7ad04-108">类型</span><span class="sxs-lookup"><span data-stu-id="7ad04-108">Type</span></span>        | <span data-ttu-id="7ad04-109">说明</span><span class="sxs-lookup"><span data-stu-id="7ad04-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7ad04-110">评估</span><span class="sxs-lookup"><span data-stu-id="7ad04-110">rating</span></span>|<span data-ttu-id="7ad04-111">callRecords。 userFeedbackRating</span><span class="sxs-lookup"><span data-stu-id="7ad04-111">microsoft.graph.callRecords.userFeedbackRating</span></span>|<span data-ttu-id="7ad04-112">此终结点的用户提供的有关此会话的质量的分级。</span><span class="sxs-lookup"><span data-stu-id="7ad04-112">The rating provided by the user of this endpoint about the quality of this Session.</span></span> <span data-ttu-id="7ad04-113">可取值为：`notRated`、`bad`、`poor`、`fair`、`good`、`excellent` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="7ad04-113">Possible values are: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7ad04-114">text</span><span class="sxs-lookup"><span data-stu-id="7ad04-114">text</span></span>|<span data-ttu-id="7ad04-115">String</span><span class="sxs-lookup"><span data-stu-id="7ad04-115">String</span></span>|<span data-ttu-id="7ad04-116">此终结点的用户提供的反馈文本，用于会话。</span><span class="sxs-lookup"><span data-stu-id="7ad04-116">The feedback text provided by the user of this endpoint for the session.</span></span>|
|<span data-ttu-id="7ad04-117">等级</span><span class="sxs-lookup"><span data-stu-id="7ad04-117">tokens</span></span>|[<span data-ttu-id="7ad04-118">callRecords。 feedbackTokenSet</span><span class="sxs-lookup"><span data-stu-id="7ad04-118">microsoft.graph.callRecords.feedbackTokenSet</span></span>](callrecords-feedbacktokenset.md)|<span data-ttu-id="7ad04-119">此终结点的用户为会话提供的一组反馈令牌。</span><span class="sxs-lookup"><span data-stu-id="7ad04-119">The set of feedback tokens provided by the user of this endpoint for the session.</span></span> <span data-ttu-id="7ad04-120">这是一组布尔属性。</span><span class="sxs-lookup"><span data-stu-id="7ad04-120">This is a set of Boolean properties.</span></span> <span data-ttu-id="7ad04-121">属性名称不应依赖，因为它们可能会根据向用户提供的令牌而发生变化。</span><span class="sxs-lookup"><span data-stu-id="7ad04-121">The property names should not be relied upon since they may change depending on what tokens are offered to the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ad04-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ad04-122">JSON representation</span></span>

<span data-ttu-id="7ad04-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ad04-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.userFeedback",
  "baseType": null
}-->

```json
{
  "rating": "String",
  "text": "String",
  "tokens": {"@odata.type": "microsoft.graph.callRecords.feedbackTokenSet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

