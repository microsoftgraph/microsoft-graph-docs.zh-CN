---
title: threatAssessmentResult 资源类型
description: 表示威胁评估结果项。
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cde4965d1b535b9ca147fda175556b8d3637e308
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075537"
---
# <a name="threatassessmentresult-resource-type"></a><span data-ttu-id="66ad9-103">threatAssessmentResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="66ad9-103">threatAssessmentResult resource type</span></span>

<span data-ttu-id="66ad9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66ad9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66ad9-105">表示威胁评估结果项。</span><span class="sxs-lookup"><span data-stu-id="66ad9-105">Represents a threat assessment result item.</span></span>

## <a name="properties"></a><span data-ttu-id="66ad9-106">属性</span><span class="sxs-lookup"><span data-stu-id="66ad9-106">Properties</span></span>

| <span data-ttu-id="66ad9-107">属性</span><span class="sxs-lookup"><span data-stu-id="66ad9-107">Property</span></span>     | <span data-ttu-id="66ad9-108">类型</span><span class="sxs-lookup"><span data-stu-id="66ad9-108">Type</span></span>        | <span data-ttu-id="66ad9-109">说明</span><span class="sxs-lookup"><span data-stu-id="66ad9-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="66ad9-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66ad9-110">createdDateTime</span></span>|<span data-ttu-id="66ad9-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66ad9-111">DateTimeOffset</span></span>|<span data-ttu-id="66ad9-112">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="66ad9-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="66ad9-113">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="66ad9-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="66ad9-114">id</span><span class="sxs-lookup"><span data-stu-id="66ad9-114">id</span></span>|<span data-ttu-id="66ad9-115">String</span><span class="sxs-lookup"><span data-stu-id="66ad9-115">String</span></span>|<span data-ttu-id="66ad9-116">威胁评估结果 ID 是 GUID)  (全局唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="66ad9-116">The threat assessment result ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="66ad9-117">message</span><span class="sxs-lookup"><span data-stu-id="66ad9-117">message</span></span>|<span data-ttu-id="66ad9-118">String</span><span class="sxs-lookup"><span data-stu-id="66ad9-118">String</span></span>|<span data-ttu-id="66ad9-119">每个威胁评估的结果消息。</span><span class="sxs-lookup"><span data-stu-id="66ad9-119">The result message for each threat assessment.</span></span>|
|<span data-ttu-id="66ad9-120">resultType</span><span class="sxs-lookup"><span data-stu-id="66ad9-120">resultType</span></span>|[<span data-ttu-id="66ad9-121">threatAssessmentResultType</span><span class="sxs-lookup"><span data-stu-id="66ad9-121">threatAssessmentResultType</span></span>](enums.md#threatassessmentresulttype-values)|<span data-ttu-id="66ad9-122">威胁评估结果类型。</span><span class="sxs-lookup"><span data-stu-id="66ad9-122">The threat assessment result type.</span></span> <span data-ttu-id="66ad9-123">可取值为：`checkPolicy`、`rescan`。</span><span class="sxs-lookup"><span data-stu-id="66ad9-123">Possible values are: `checkPolicy`, `rescan`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66ad9-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66ad9-124">JSON representation</span></span>

<span data-ttu-id="66ad9-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66ad9-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.threatAssessmentResult",
  "baseType": "",
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


