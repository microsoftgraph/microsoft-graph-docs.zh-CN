---
title: threatAssessmentResult 资源类型
description: 表示威胁评估结果项。
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 307b3bbebd9059ffee057781b5f647e407657684
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950261"
---
# <a name="threatassessmentresult-resource-type"></a><span data-ttu-id="64dfc-103">threatAssessmentResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="64dfc-103">threatAssessmentResult resource type</span></span>

<span data-ttu-id="64dfc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64dfc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64dfc-105">表示威胁评估结果项。</span><span class="sxs-lookup"><span data-stu-id="64dfc-105">Represents a threat assessment result item.</span></span>

## <a name="properties"></a><span data-ttu-id="64dfc-106">属性</span><span class="sxs-lookup"><span data-stu-id="64dfc-106">Properties</span></span>

| <span data-ttu-id="64dfc-107">属性</span><span class="sxs-lookup"><span data-stu-id="64dfc-107">Property</span></span>     | <span data-ttu-id="64dfc-108">类型</span><span class="sxs-lookup"><span data-stu-id="64dfc-108">Type</span></span>        | <span data-ttu-id="64dfc-109">说明</span><span class="sxs-lookup"><span data-stu-id="64dfc-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="64dfc-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64dfc-110">createdDateTime</span></span>|<span data-ttu-id="64dfc-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64dfc-111">DateTimeOffset</span></span>|<span data-ttu-id="64dfc-112">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="64dfc-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="64dfc-113">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="64dfc-113">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="64dfc-114">id</span><span class="sxs-lookup"><span data-stu-id="64dfc-114">id</span></span>|<span data-ttu-id="64dfc-115">String</span><span class="sxs-lookup"><span data-stu-id="64dfc-115">String</span></span>|<span data-ttu-id="64dfc-116">威胁评估结果 ID 是 GUID (全局唯一) 。</span><span class="sxs-lookup"><span data-stu-id="64dfc-116">The threat assessment result ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="64dfc-117">message</span><span class="sxs-lookup"><span data-stu-id="64dfc-117">message</span></span>|<span data-ttu-id="64dfc-118">String</span><span class="sxs-lookup"><span data-stu-id="64dfc-118">String</span></span>|<span data-ttu-id="64dfc-119">每个威胁评估的结果消息。</span><span class="sxs-lookup"><span data-stu-id="64dfc-119">The result message for each threat assessment.</span></span>|
|<span data-ttu-id="64dfc-120">resultType</span><span class="sxs-lookup"><span data-stu-id="64dfc-120">resultType</span></span>|<span data-ttu-id="64dfc-121">threatAssessmentResultType</span><span class="sxs-lookup"><span data-stu-id="64dfc-121">threatAssessmentResultType</span></span>|<span data-ttu-id="64dfc-122">威胁评估结果类型。</span><span class="sxs-lookup"><span data-stu-id="64dfc-122">The threat assessment result type.</span></span> <span data-ttu-id="64dfc-123">可能的值是 `checkPolicy` ： (邮件评估) ， `rescan` 。</span><span class="sxs-lookup"><span data-stu-id="64dfc-123">Possible values are: `checkPolicy` (only for mail assessment), `rescan`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64dfc-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64dfc-124">JSON representation</span></span>

<span data-ttu-id="64dfc-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64dfc-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.threatAssessmentResult",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "message": "String",
  "resultType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "threatAssessmentResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


