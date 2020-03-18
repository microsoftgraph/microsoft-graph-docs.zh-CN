---
title: userExperienceAnalyticsInsight 资源类型
description: 用户体验分析见解是改进用户体验分析分数的建议。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c28df3bc40f02948198a67850de6fd573607a366
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783793"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a><span data-ttu-id="cadf0-103">userExperienceAnalyticsInsight 资源类型</span><span class="sxs-lookup"><span data-stu-id="cadf0-103">userExperienceAnalyticsInsight resource type</span></span>

> <span data-ttu-id="cadf0-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cadf0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cadf0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cadf0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cadf0-106">用户体验分析见解是改进用户体验分析分数的建议。</span><span class="sxs-lookup"><span data-stu-id="cadf0-106">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="cadf0-107">属性</span><span class="sxs-lookup"><span data-stu-id="cadf0-107">Properties</span></span>
|<span data-ttu-id="cadf0-108">属性</span><span class="sxs-lookup"><span data-stu-id="cadf0-108">Property</span></span>|<span data-ttu-id="cadf0-109">类型</span><span class="sxs-lookup"><span data-stu-id="cadf0-109">Type</span></span>|<span data-ttu-id="cadf0-110">说明</span><span class="sxs-lookup"><span data-stu-id="cadf0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cadf0-111">userExperienceAnalyticsMetricId</span><span class="sxs-lookup"><span data-stu-id="cadf0-111">userExperienceAnalyticsMetricId</span></span>|<span data-ttu-id="cadf0-112">String</span><span class="sxs-lookup"><span data-stu-id="cadf0-112">String</span></span>|<span data-ttu-id="cadf0-113">用户体验分析洞察力的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cadf0-113">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="cadf0-114">insightId</span><span class="sxs-lookup"><span data-stu-id="cadf0-114">insightId</span></span>|<span data-ttu-id="cadf0-115">String</span><span class="sxs-lookup"><span data-stu-id="cadf0-115">String</span></span>|<span data-ttu-id="cadf0-116">用户体验分析洞察力的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cadf0-116">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="cadf0-117">values</span><span class="sxs-lookup"><span data-stu-id="cadf0-117">values</span></span>|<span data-ttu-id="cadf0-118">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="cadf0-118">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md) collection</span></span>|<span data-ttu-id="cadf0-119">用户体验分析洞察力的价值。</span><span class="sxs-lookup"><span data-stu-id="cadf0-119">The value of the user experience analytics insight.</span></span>|
|<span data-ttu-id="cadf0-120">severity</span><span class="sxs-lookup"><span data-stu-id="cadf0-120">severity</span></span>|[<span data-ttu-id="cadf0-121">userExperienceAnalyticsInsightSeverity</span><span class="sxs-lookup"><span data-stu-id="cadf0-121">userExperienceAnalyticsInsightSeverity</span></span>](../resources/intune-devices-userexperienceanalyticsinsightseverity.md)|<span data-ttu-id="cadf0-122">用户体验分析洞察力的价值。</span><span class="sxs-lookup"><span data-stu-id="cadf0-122">The value of the user experience analytics insight.</span></span> <span data-ttu-id="cadf0-123">可取值为：`none`、`informational`、`warning`、`error`。</span><span class="sxs-lookup"><span data-stu-id="cadf0-123">Possible values are: `none`, `informational`, `warning`, `error`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cadf0-124">关系</span><span class="sxs-lookup"><span data-stu-id="cadf0-124">Relationships</span></span>
<span data-ttu-id="cadf0-125">无</span><span class="sxs-lookup"><span data-stu-id="cadf0-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cadf0-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cadf0-126">JSON Representation</span></span>
<span data-ttu-id="cadf0-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cadf0-127">Here is a JSON representation of the resource.</span></span>
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
      "value": "<Unknown Primitive Type Edm.Double>"
    }
  ],
  "severity": "String"
}
```



