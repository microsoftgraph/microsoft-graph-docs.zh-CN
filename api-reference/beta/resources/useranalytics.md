---
title: userAnalytics 资源类型
description: 用户的设置和活动统计信息。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ac4024fff534bd89e369f1f8048ca274ccfd157a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057898"
---
# <a name="useranalytics-resource-type"></a><span data-ttu-id="e2d4a-103">userAnalytics 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2d4a-103">userAnalytics resource type</span></span>

<span data-ttu-id="e2d4a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2d4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2d4a-105">用户的设置和活动统计信息。</span><span class="sxs-lookup"><span data-stu-id="e2d4a-105">The user's settings and activity statistics.</span></span>

## <a name="methods"></a><span data-ttu-id="e2d4a-106">方法</span><span class="sxs-lookup"><span data-stu-id="e2d4a-106">Methods</span></span>

| <span data-ttu-id="e2d4a-107">方法</span><span class="sxs-lookup"><span data-stu-id="e2d4a-107">Method</span></span>       | <span data-ttu-id="e2d4a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e2d4a-108">Return Type</span></span> | <span data-ttu-id="e2d4a-109">说明</span><span class="sxs-lookup"><span data-stu-id="e2d4a-109">Description</span></span> |
|:-------------|:------------|:------------|
[<span data-ttu-id="e2d4a-110">获取设置</span><span class="sxs-lookup"><span data-stu-id="e2d4a-110">Get settings</span></span>](../api/useranalytics-get-settings.md) | [<span data-ttu-id="e2d4a-111">设置</span><span class="sxs-lookup"><span data-stu-id="e2d4a-111">settings</span></span>](settings.md) | <span data-ttu-id="e2d4a-112">获取用户使用分析 API 的设置。</span><span class="sxs-lookup"><span data-stu-id="e2d4a-112">Get the user's settings for using the analytics API.</span></span>|

## <a name="properties"></a><span data-ttu-id="e2d4a-113">属性</span><span class="sxs-lookup"><span data-stu-id="e2d4a-113">Properties</span></span>

| <span data-ttu-id="e2d4a-114">属性</span><span class="sxs-lookup"><span data-stu-id="e2d4a-114">Property</span></span>     | <span data-ttu-id="e2d4a-115">类型</span><span class="sxs-lookup"><span data-stu-id="e2d4a-115">Type</span></span>        | <span data-ttu-id="e2d4a-116">说明</span><span class="sxs-lookup"><span data-stu-id="e2d4a-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e2d4a-117">设置</span><span class="sxs-lookup"><span data-stu-id="e2d4a-117">settings</span></span>|[<span data-ttu-id="e2d4a-118">设置</span><span class="sxs-lookup"><span data-stu-id="e2d4a-118">settings</span></span>](settings.md)|<span data-ttu-id="e2d4a-119">用户使用分析 API 的当前设置。</span><span class="sxs-lookup"><span data-stu-id="e2d4a-119">The current settings for a user to use the analytics API.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2d4a-120">关系</span><span class="sxs-lookup"><span data-stu-id="e2d4a-120">Relationships</span></span>

| <span data-ttu-id="e2d4a-121">关系</span><span class="sxs-lookup"><span data-stu-id="e2d4a-121">Relationship</span></span> | <span data-ttu-id="e2d4a-122">类型</span><span class="sxs-lookup"><span data-stu-id="e2d4a-122">Type</span></span>        | <span data-ttu-id="e2d4a-123">说明</span><span class="sxs-lookup"><span data-stu-id="e2d4a-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e2d4a-124">activityStatistics</span><span class="sxs-lookup"><span data-stu-id="e2d4a-124">activityStatistics</span></span>|<span data-ttu-id="e2d4a-125">[activityStatistics](activitystatistics.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e2d4a-125">[activityStatistics](activitystatistics.md) collection</span></span>| <span data-ttu-id="e2d4a-126">用户在工作时间和工作时间之外花费时间的工作活动的集合。</span><span class="sxs-lookup"><span data-stu-id="e2d4a-126">The collection of work activities that a user spent time on during and outside of working hours.</span></span> <span data-ttu-id="e2d4a-127">只读。</span><span class="sxs-lookup"><span data-stu-id="e2d4a-127">Read-only.</span></span> <span data-ttu-id="e2d4a-128">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e2d4a-128">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2d4a-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2d4a-129">JSON representation</span></span>

<span data-ttu-id="e2d4a-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2d4a-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [
    "activityStatistics"
  ],
  "@odata.type": "microsoft.graph.userAnalytics"
}-->

```json
{
  "id": "string",
  "settings": {"@odata.type": "microsoft.graph.settings"},
  "activityStatistics": [{"@odata.type": "microsoft.graph.activityStatistics"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAnalytics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


