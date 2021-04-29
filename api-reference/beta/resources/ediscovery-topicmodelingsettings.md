---
title: topicModelingSettings 资源类型
description: 电子数据展示案例的主题建模设置
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: bd433de0aa88298961366f50425706e1af4bffde
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080741"
---
# <a name="topicmodelingsettings-resource-type"></a><span data-ttu-id="f0f79-103">topicModelingSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0f79-103">topicModelingSettings resource type</span></span>

<span data-ttu-id="f0f79-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f0f79-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0f79-105">主题建模 (电子) 展示案例的主题设置。</span><span class="sxs-lookup"><span data-stu-id="f0f79-105">Topic modeling (Themes) settings for an eDiscovery case.</span></span> <span data-ttu-id="f0f79-106">若要了解更多信息，请参阅配置[搜索和分析Advanced eDiscovery。](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery)</span><span class="sxs-lookup"><span data-stu-id="f0f79-106">To learn more, see [Configure search and analytics settings in Advanced eDiscovery](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery).</span></span>

## <a name="properties"></a><span data-ttu-id="f0f79-107">属性</span><span class="sxs-lookup"><span data-stu-id="f0f79-107">Properties</span></span>

|<span data-ttu-id="f0f79-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0f79-108">Property</span></span>|<span data-ttu-id="f0f79-109">类型</span><span class="sxs-lookup"><span data-stu-id="f0f79-109">Type</span></span>|<span data-ttu-id="f0f79-110">说明</span><span class="sxs-lookup"><span data-stu-id="f0f79-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0f79-111">dynamicallyAdjustTopicCount</span><span class="sxs-lookup"><span data-stu-id="f0f79-111">dynamicallyAdjustTopicCount</span></span>|<span data-ttu-id="f0f79-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f79-112">Boolean</span></span>|<span data-ttu-id="f0f79-113">若要了解更多信息，请参阅 [动态调整最大主题数](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)。</span><span class="sxs-lookup"><span data-stu-id="f0f79-113">To learn more, see [Adjust maximum number of themes dynamically](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).</span></span>|
|<span data-ttu-id="f0f79-114">ignoreNumbers</span><span class="sxs-lookup"><span data-stu-id="f0f79-114">ignoreNumbers</span></span>|<span data-ttu-id="f0f79-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f79-115">Boolean</span></span>|<span data-ttu-id="f0f79-116">若要了解更多信息，请参阅 [在主题中包括数字](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)。</span><span class="sxs-lookup"><span data-stu-id="f0f79-116">To learn more, see [Include numbers in themes](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).</span></span>|
|<span data-ttu-id="f0f79-117">isEnabled</span><span class="sxs-lookup"><span data-stu-id="f0f79-117">isEnabled</span></span>|<span data-ttu-id="f0f79-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f79-118">Boolean</span></span>|<span data-ttu-id="f0f79-119">指示是否针对案例启用主题。</span><span class="sxs-lookup"><span data-stu-id="f0f79-119">Indicates whether themes is enabled for the case.</span></span>|
|<span data-ttu-id="f0f79-120">topicCount</span><span class="sxs-lookup"><span data-stu-id="f0f79-120">topicCount</span></span>|<span data-ttu-id="f0f79-121">Int32</span><span class="sxs-lookup"><span data-stu-id="f0f79-121">Int32</span></span>|<span data-ttu-id="f0f79-122">若要了解更多信息，请参阅 [主题的最大数量](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)。</span><span class="sxs-lookup"><span data-stu-id="f0f79-122">To learn more, see [Maximum number of themes](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0f79-123">关系</span><span class="sxs-lookup"><span data-stu-id="f0f79-123">Relationships</span></span>

<span data-ttu-id="f0f79-124">无。</span><span class="sxs-lookup"><span data-stu-id="f0f79-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0f79-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0f79-125">JSON representation</span></span>

<span data-ttu-id="f0f79-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0f79-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ediscovery.topicModelingSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.topicModelingSettings",
  "isEnabled": "Boolean",
  "ignoreNumbers": "Boolean",
  "topicCount": "Integer",
  "dynamicallyAdjustTopicCount": "Boolean"
}
```
