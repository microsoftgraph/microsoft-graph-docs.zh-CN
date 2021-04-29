---
title: redundancyDetectionSettings 资源类型
description: 电子数据展示案例的冗余设置
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: fd1ca1ea3faf03e2639896c79acd0629931c71c9
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080745"
---
# <a name="redundancydetectionsettings-resource-type"></a><span data-ttu-id="6f7aa-103">redundancyDetectionSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f7aa-103">redundancyDetectionSettings resource type</span></span>

<span data-ttu-id="6f7aa-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="6f7aa-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f7aa-105">冗余 (电子数据展示案例的电子邮件线程和) 重复检测设置。</span><span class="sxs-lookup"><span data-stu-id="6f7aa-105">Redundancy (email threading and near duplicate detection) settings for an eDiscovery case.</span></span>

## <a name="properties"></a><span data-ttu-id="6f7aa-106">属性</span><span class="sxs-lookup"><span data-stu-id="6f7aa-106">Properties</span></span>

|<span data-ttu-id="6f7aa-107">属性</span><span class="sxs-lookup"><span data-stu-id="6f7aa-107">Property</span></span>|<span data-ttu-id="6f7aa-108">类型</span><span class="sxs-lookup"><span data-stu-id="6f7aa-108">Type</span></span>|<span data-ttu-id="6f7aa-109">说明</span><span class="sxs-lookup"><span data-stu-id="6f7aa-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f7aa-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="6f7aa-110">isEnabled</span></span>|<span data-ttu-id="6f7aa-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f7aa-111">Boolean</span></span>|<span data-ttu-id="6f7aa-112">指示是否启用电子邮件线程和几乎重复检测。</span><span class="sxs-lookup"><span data-stu-id="6f7aa-112">Indicates whether email threading and near duplicate detection are enabled.</span></span>|
|<span data-ttu-id="6f7aa-113">maxWords</span><span class="sxs-lookup"><span data-stu-id="6f7aa-113">maxWords</span></span>|<span data-ttu-id="6f7aa-114">Int32</span><span class="sxs-lookup"><span data-stu-id="6f7aa-114">Int32</span></span>|<span data-ttu-id="6f7aa-115">有关详细信息 [，请参阅最小/最大](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) 单词数。</span><span class="sxs-lookup"><span data-stu-id="6f7aa-115">See [Minimum/maximum number of words](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) to learn more.</span></span>|
|<span data-ttu-id="6f7aa-116">minWords</span><span class="sxs-lookup"><span data-stu-id="6f7aa-116">minWords</span></span>|<span data-ttu-id="6f7aa-117">Int32</span><span class="sxs-lookup"><span data-stu-id="6f7aa-117">Int32</span></span>|<span data-ttu-id="6f7aa-118">有关详细信息 [，请参阅最小/最大](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) 单词数。</span><span class="sxs-lookup"><span data-stu-id="6f7aa-118">See [Minimum/maximum number of words](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) to learn more.</span></span>|
|<span data-ttu-id="6f7aa-119">similarityThreshold</span><span class="sxs-lookup"><span data-stu-id="6f7aa-119">similarityThreshold</span></span>|<span data-ttu-id="6f7aa-120">Int32</span><span class="sxs-lookup"><span data-stu-id="6f7aa-120">Int32</span></span>|<span data-ttu-id="6f7aa-121">有关详细信息 [，请参阅文档和电子邮件相似性](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) 阈值。</span><span class="sxs-lookup"><span data-stu-id="6f7aa-121">See [Document and email similarity threshold](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) to learn more.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f7aa-122">关系</span><span class="sxs-lookup"><span data-stu-id="6f7aa-122">Relationships</span></span>

<span data-ttu-id="6f7aa-123">无。</span><span class="sxs-lookup"><span data-stu-id="6f7aa-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f7aa-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f7aa-124">JSON representation</span></span>

<span data-ttu-id="6f7aa-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f7aa-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ediscovery.redundancyDetectionSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.redundancyDetectionSettings",
  "isEnabled": "Boolean",
  "similarityThreshold": "Integer",
  "minWords": "Integer",
  "maxWords": "Integer"
}
```
