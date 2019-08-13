---
title: userExperienceAnalyticsInsight 资源类型
description: 用户体验分析见解是改进用户体验分析分数的建议。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 36277b147e7eabc6f28aef3877538ebbc429f381
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36341216"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a><span data-ttu-id="d6404-103">userExperienceAnalyticsInsight 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6404-103">userExperienceAnalyticsInsight resource type</span></span>

> <span data-ttu-id="d6404-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d6404-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6404-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6404-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6404-106">用户体验分析见解是改进用户体验分析分数的建议。</span><span class="sxs-lookup"><span data-stu-id="d6404-106">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="d6404-107">属性</span><span class="sxs-lookup"><span data-stu-id="d6404-107">Properties</span></span>
|<span data-ttu-id="d6404-108">属性</span><span class="sxs-lookup"><span data-stu-id="d6404-108">Property</span></span>|<span data-ttu-id="d6404-109">类型</span><span class="sxs-lookup"><span data-stu-id="d6404-109">Type</span></span>|<span data-ttu-id="d6404-110">说明</span><span class="sxs-lookup"><span data-stu-id="d6404-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6404-111">userExperienceAnalyticsMetricId</span><span class="sxs-lookup"><span data-stu-id="d6404-111">userExperienceAnalyticsMetricId</span></span>|<span data-ttu-id="d6404-112">String</span><span class="sxs-lookup"><span data-stu-id="d6404-112">String</span></span>|<span data-ttu-id="d6404-113">用户体验分析洞察力的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d6404-113">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="d6404-114">insightId</span><span class="sxs-lookup"><span data-stu-id="d6404-114">insightId</span></span>|<span data-ttu-id="d6404-115">String</span><span class="sxs-lookup"><span data-stu-id="d6404-115">String</span></span>|<span data-ttu-id="d6404-116">用户体验分析洞察力的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d6404-116">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="d6404-117">值</span><span class="sxs-lookup"><span data-stu-id="d6404-117">value</span></span>|<span data-ttu-id="d6404-118">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="d6404-118">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md) collection</span></span>|<span data-ttu-id="d6404-119">用户体验分析洞察力的价值。</span><span class="sxs-lookup"><span data-stu-id="d6404-119">The value of the user experience analytics insight.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6404-120">关系</span><span class="sxs-lookup"><span data-stu-id="d6404-120">Relationships</span></span>
<span data-ttu-id="d6404-121">无</span><span class="sxs-lookup"><span data-stu-id="d6404-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6404-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6404-122">JSON Representation</span></span>
<span data-ttu-id="d6404-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6404-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsInsight",
  "userExperienceAnalyticsMetricId": "String",
  "insightId": "String",
  "value": [
    {
      "@odata.type": "microsoft.graph.insightValueDouble"
    }
  ]
}
```



