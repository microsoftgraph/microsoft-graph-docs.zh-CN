---
title: userAnalytics 资源类型
description: 用户的设置和活动统计信息。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 51e72d21cfb0e26e46a7d247f4ede59b112893ea
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450713"
---
# <a name="useranalytics-resource-type"></a><span data-ttu-id="2c58d-103">userAnalytics 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c58d-103">userAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c58d-104">用户的设置和活动统计信息。</span><span class="sxs-lookup"><span data-stu-id="2c58d-104">The user's settings and activity statistics.</span></span>

## <a name="methods"></a><span data-ttu-id="2c58d-105">方法</span><span class="sxs-lookup"><span data-stu-id="2c58d-105">Methods</span></span>

| <span data-ttu-id="2c58d-106">方法</span><span class="sxs-lookup"><span data-stu-id="2c58d-106">Method</span></span>       | <span data-ttu-id="2c58d-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="2c58d-107">Return Type</span></span> | <span data-ttu-id="2c58d-108">说明</span><span class="sxs-lookup"><span data-stu-id="2c58d-108">Description</span></span> |
|:-------------|:------------|:------------|
[<span data-ttu-id="2c58d-109">获取设置</span><span class="sxs-lookup"><span data-stu-id="2c58d-109">Get settings</span></span>](../api/useranalytics-get-settings.md) | [<span data-ttu-id="2c58d-110">settings</span><span class="sxs-lookup"><span data-stu-id="2c58d-110">settings</span></span>](settings.md) | <span data-ttu-id="2c58d-111">获取用户使用分析 API 的设置。</span><span class="sxs-lookup"><span data-stu-id="2c58d-111">Get the user's settings for using the analytics API.</span></span>|

## <a name="properties"></a><span data-ttu-id="2c58d-112">属性</span><span class="sxs-lookup"><span data-stu-id="2c58d-112">Properties</span></span>

| <span data-ttu-id="2c58d-113">属性</span><span class="sxs-lookup"><span data-stu-id="2c58d-113">Property</span></span>     | <span data-ttu-id="2c58d-114">类型</span><span class="sxs-lookup"><span data-stu-id="2c58d-114">Type</span></span>        | <span data-ttu-id="2c58d-115">说明</span><span class="sxs-lookup"><span data-stu-id="2c58d-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2c58d-116">settings</span><span class="sxs-lookup"><span data-stu-id="2c58d-116">settings</span></span>|[<span data-ttu-id="2c58d-117">settings</span><span class="sxs-lookup"><span data-stu-id="2c58d-117">settings</span></span>](settings.md)|<span data-ttu-id="2c58d-118">用户使用分析 API 的当前设置。</span><span class="sxs-lookup"><span data-stu-id="2c58d-118">The current settings for a user to use the analytics API.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c58d-119">关系</span><span class="sxs-lookup"><span data-stu-id="2c58d-119">Relationships</span></span>

| <span data-ttu-id="2c58d-120">关系</span><span class="sxs-lookup"><span data-stu-id="2c58d-120">Relationship</span></span> | <span data-ttu-id="2c58d-121">类型</span><span class="sxs-lookup"><span data-stu-id="2c58d-121">Type</span></span>        | <span data-ttu-id="2c58d-122">说明</span><span class="sxs-lookup"><span data-stu-id="2c58d-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2c58d-123">activityStatistics</span><span class="sxs-lookup"><span data-stu-id="2c58d-123">activityStatistics</span></span>|<span data-ttu-id="2c58d-124">[activityStatistics](activitystatistics.md)集合</span><span class="sxs-lookup"><span data-stu-id="2c58d-124">[activityStatistics](activitystatistics.md) collection</span></span>| <span data-ttu-id="2c58d-125">用户在工作时间和工作时间之外花费时间的工作活动的集合。</span><span class="sxs-lookup"><span data-stu-id="2c58d-125">The collection of work activities that a user spent time on during and outside of working hours.</span></span> <span data-ttu-id="2c58d-126">只读。</span><span class="sxs-lookup"><span data-stu-id="2c58d-126">Read-only.</span></span> <span data-ttu-id="2c58d-127">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2c58d-127">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c58d-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c58d-128">JSON representation</span></span>

<span data-ttu-id="2c58d-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c58d-129">The following is a JSON representation of the resource.</span></span>

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
