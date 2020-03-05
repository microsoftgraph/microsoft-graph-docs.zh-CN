---
title: userAnalytics 资源类型
description: 用户的设置和活动统计信息。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ffe6830088bd60c4de9cea8def8e8202d1b33f13
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519538"
---
# <a name="useranalytics-resource-type"></a><span data-ttu-id="07bed-103">userAnalytics 资源类型</span><span class="sxs-lookup"><span data-stu-id="07bed-103">userAnalytics resource type</span></span>

<span data-ttu-id="07bed-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="07bed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07bed-105">用户的设置和活动统计信息。</span><span class="sxs-lookup"><span data-stu-id="07bed-105">The user's settings and activity statistics.</span></span>

## <a name="methods"></a><span data-ttu-id="07bed-106">方法</span><span class="sxs-lookup"><span data-stu-id="07bed-106">Methods</span></span>

| <span data-ttu-id="07bed-107">方法</span><span class="sxs-lookup"><span data-stu-id="07bed-107">Method</span></span>       | <span data-ttu-id="07bed-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="07bed-108">Return Type</span></span> | <span data-ttu-id="07bed-109">说明</span><span class="sxs-lookup"><span data-stu-id="07bed-109">Description</span></span> |
|:-------------|:------------|:------------|
[<span data-ttu-id="07bed-110">获取设置</span><span class="sxs-lookup"><span data-stu-id="07bed-110">Get settings</span></span>](../api/useranalytics-get-settings.md) | [<span data-ttu-id="07bed-111">设置</span><span class="sxs-lookup"><span data-stu-id="07bed-111">settings</span></span>](settings.md) | <span data-ttu-id="07bed-112">获取用户使用分析 API 的设置。</span><span class="sxs-lookup"><span data-stu-id="07bed-112">Get the user's settings for using the analytics API.</span></span>|

## <a name="properties"></a><span data-ttu-id="07bed-113">属性</span><span class="sxs-lookup"><span data-stu-id="07bed-113">Properties</span></span>

| <span data-ttu-id="07bed-114">属性</span><span class="sxs-lookup"><span data-stu-id="07bed-114">Property</span></span>     | <span data-ttu-id="07bed-115">类型</span><span class="sxs-lookup"><span data-stu-id="07bed-115">Type</span></span>        | <span data-ttu-id="07bed-116">说明</span><span class="sxs-lookup"><span data-stu-id="07bed-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="07bed-117">设置</span><span class="sxs-lookup"><span data-stu-id="07bed-117">settings</span></span>|[<span data-ttu-id="07bed-118">设置</span><span class="sxs-lookup"><span data-stu-id="07bed-118">settings</span></span>](settings.md)|<span data-ttu-id="07bed-119">用户使用分析 API 的当前设置。</span><span class="sxs-lookup"><span data-stu-id="07bed-119">The current settings for a user to use the analytics API.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07bed-120">关系</span><span class="sxs-lookup"><span data-stu-id="07bed-120">Relationships</span></span>

| <span data-ttu-id="07bed-121">关系</span><span class="sxs-lookup"><span data-stu-id="07bed-121">Relationship</span></span> | <span data-ttu-id="07bed-122">类型</span><span class="sxs-lookup"><span data-stu-id="07bed-122">Type</span></span>        | <span data-ttu-id="07bed-123">说明</span><span class="sxs-lookup"><span data-stu-id="07bed-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="07bed-124">activityStatistics</span><span class="sxs-lookup"><span data-stu-id="07bed-124">activityStatistics</span></span>|<span data-ttu-id="07bed-125">[activityStatistics](activitystatistics.md)集合</span><span class="sxs-lookup"><span data-stu-id="07bed-125">[activityStatistics](activitystatistics.md) collection</span></span>| <span data-ttu-id="07bed-126">用户在工作时间和工作时间之外花费时间的工作活动的集合。</span><span class="sxs-lookup"><span data-stu-id="07bed-126">The collection of work activities that a user spent time on during and outside of working hours.</span></span> <span data-ttu-id="07bed-127">只读。</span><span class="sxs-lookup"><span data-stu-id="07bed-127">Read-only.</span></span> <span data-ttu-id="07bed-128">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="07bed-128">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07bed-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07bed-129">JSON representation</span></span>

<span data-ttu-id="07bed-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07bed-130">The following is a JSON representation of the resource.</span></span>

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
