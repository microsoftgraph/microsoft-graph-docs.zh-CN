---
title: userExperienceAnalyticsInsight 资源类型
description: 用户体验分析见解是改进用户体验分析分数的建议。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d000afacb82365e06c5728dd8eedc2e6eb4217dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080892"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a><span data-ttu-id="3adc7-103">userExperienceAnalyticsInsight 资源类型</span><span class="sxs-lookup"><span data-stu-id="3adc7-103">userExperienceAnalyticsInsight resource type</span></span>

<span data-ttu-id="3adc7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3adc7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3adc7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3adc7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3adc7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3adc7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3adc7-107">用户体验分析见解是改进用户体验分析分数的建议。</span><span class="sxs-lookup"><span data-stu-id="3adc7-107">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="3adc7-108">属性</span><span class="sxs-lookup"><span data-stu-id="3adc7-108">Properties</span></span>
|<span data-ttu-id="3adc7-109">属性</span><span class="sxs-lookup"><span data-stu-id="3adc7-109">Property</span></span>|<span data-ttu-id="3adc7-110">类型</span><span class="sxs-lookup"><span data-stu-id="3adc7-110">Type</span></span>|<span data-ttu-id="3adc7-111">说明</span><span class="sxs-lookup"><span data-stu-id="3adc7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3adc7-112">userExperienceAnalyticsMetricId</span><span class="sxs-lookup"><span data-stu-id="3adc7-112">userExperienceAnalyticsMetricId</span></span>|<span data-ttu-id="3adc7-113">字符串</span><span class="sxs-lookup"><span data-stu-id="3adc7-113">String</span></span>|<span data-ttu-id="3adc7-114">用户体验分析洞察力的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3adc7-114">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="3adc7-115">insightId</span><span class="sxs-lookup"><span data-stu-id="3adc7-115">insightId</span></span>|<span data-ttu-id="3adc7-116">字符串</span><span class="sxs-lookup"><span data-stu-id="3adc7-116">String</span></span>|<span data-ttu-id="3adc7-117">用户体验分析洞察力的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3adc7-117">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="3adc7-118">values</span><span class="sxs-lookup"><span data-stu-id="3adc7-118">values</span></span>|<span data-ttu-id="3adc7-119">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3adc7-119">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md) collection</span></span>|<span data-ttu-id="3adc7-120">用户体验分析洞察力的价值。</span><span class="sxs-lookup"><span data-stu-id="3adc7-120">The value of the user experience analytics insight.</span></span>|
|<span data-ttu-id="3adc7-121">severity</span><span class="sxs-lookup"><span data-stu-id="3adc7-121">severity</span></span>|[<span data-ttu-id="3adc7-122">userExperienceAnalyticsInsightSeverity</span><span class="sxs-lookup"><span data-stu-id="3adc7-122">userExperienceAnalyticsInsightSeverity</span></span>](../resources/intune-devices-userexperienceanalyticsinsightseverity.md)|<span data-ttu-id="3adc7-123">用户体验分析洞察力的价值。</span><span class="sxs-lookup"><span data-stu-id="3adc7-123">The value of the user experience analytics insight.</span></span> <span data-ttu-id="3adc7-124">可取值为：`none`、`informational`、`warning`、`error`。</span><span class="sxs-lookup"><span data-stu-id="3adc7-124">Possible values are: `none`, `informational`, `warning`, `error`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3adc7-125">关系</span><span class="sxs-lookup"><span data-stu-id="3adc7-125">Relationships</span></span>
<span data-ttu-id="3adc7-126">无</span><span class="sxs-lookup"><span data-stu-id="3adc7-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3adc7-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3adc7-127">JSON Representation</span></span>
<span data-ttu-id="3adc7-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3adc7-128">Here is a JSON representation of the resource.</span></span>
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
  "values": [
    {
      "@odata.type": "microsoft.graph.insightValueDouble",
      "value": "4.2"
    }
  ],
  "severity": "String"
}
```






