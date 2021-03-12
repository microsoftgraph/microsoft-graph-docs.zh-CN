---
title: threatAssessmentResult 资源类型
description: 表示威胁评估结果项。
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0657cef555cd982c6649f6a8a4f40b7e5e15eaab
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722099"
---
# <a name="threatassessmentresult-resource-type"></a><span data-ttu-id="8872f-103">threatAssessmentResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="8872f-103">threatAssessmentResult resource type</span></span>

<span data-ttu-id="8872f-104">表示威胁评估结果项。</span><span class="sxs-lookup"><span data-stu-id="8872f-104">Represents a threat assessment result item.</span></span>

## <a name="properties"></a><span data-ttu-id="8872f-105">属性</span><span class="sxs-lookup"><span data-stu-id="8872f-105">Properties</span></span>

| <span data-ttu-id="8872f-106">属性</span><span class="sxs-lookup"><span data-stu-id="8872f-106">Property</span></span>     | <span data-ttu-id="8872f-107">类型</span><span class="sxs-lookup"><span data-stu-id="8872f-107">Type</span></span>        | <span data-ttu-id="8872f-108">说明</span><span class="sxs-lookup"><span data-stu-id="8872f-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8872f-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8872f-109">createdDateTime</span></span>|<span data-ttu-id="8872f-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8872f-110">DateTimeOffset</span></span>|<span data-ttu-id="8872f-111">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="8872f-111">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8872f-112">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="8872f-112">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="8872f-113">id</span><span class="sxs-lookup"><span data-stu-id="8872f-113">id</span></span>|<span data-ttu-id="8872f-114">字符串</span><span class="sxs-lookup"><span data-stu-id="8872f-114">String</span></span>|<span data-ttu-id="8872f-115">威胁评估结果 ID 是 GUID (全局唯一) 。</span><span class="sxs-lookup"><span data-stu-id="8872f-115">The threat assessment result ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="8872f-116">message</span><span class="sxs-lookup"><span data-stu-id="8872f-116">message</span></span>|<span data-ttu-id="8872f-117">String</span><span class="sxs-lookup"><span data-stu-id="8872f-117">String</span></span>|<span data-ttu-id="8872f-118">每个威胁评估的结果消息。</span><span class="sxs-lookup"><span data-stu-id="8872f-118">The result message for each threat assessment.</span></span>|
|<span data-ttu-id="8872f-119">resultType</span><span class="sxs-lookup"><span data-stu-id="8872f-119">resultType</span></span>|[<span data-ttu-id="8872f-120">threatAssessmentResultType</span><span class="sxs-lookup"><span data-stu-id="8872f-120">threatAssessmentResultType</span></span>](enums.md#threatassessmentresulttype-values)|<span data-ttu-id="8872f-121">威胁评估结果类型。</span><span class="sxs-lookup"><span data-stu-id="8872f-121">The threat assessment result type.</span></span> <span data-ttu-id="8872f-122">可取值为：`checkPolicy`、`rescan`。</span><span class="sxs-lookup"><span data-stu-id="8872f-122">Possible values are: `checkPolicy`, `rescan`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8872f-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8872f-123">JSON representation</span></span>

<span data-ttu-id="8872f-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8872f-124">The following is a JSON representation of the resource.</span></span>

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

