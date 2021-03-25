---
title: assignmentFilterStatusDetails 资源类型
description: 表示设备和有效负载以及所有关联的已应用筛选器的状态详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: be36fae74e412395bd74a24b11b36b48cbf165ff
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155972"
---
# <a name="assignmentfilterstatusdetails-resource-type"></a><span data-ttu-id="5e868-103">assignmentFilterStatusDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e868-103">assignmentFilterStatusDetails resource type</span></span>

<span data-ttu-id="5e868-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e868-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e868-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5e868-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e868-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e868-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e868-107">表示设备和有效负载以及所有关联的已应用筛选器的状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="5e868-107">Represent status details for device and payload and all associated applied filters.</span></span>

## <a name="properties"></a><span data-ttu-id="5e868-108">属性</span><span class="sxs-lookup"><span data-stu-id="5e868-108">Properties</span></span>
|<span data-ttu-id="5e868-109">属性</span><span class="sxs-lookup"><span data-stu-id="5e868-109">Property</span></span>|<span data-ttu-id="5e868-110">类型</span><span class="sxs-lookup"><span data-stu-id="5e868-110">Type</span></span>|<span data-ttu-id="5e868-111">说明</span><span class="sxs-lookup"><span data-stu-id="5e868-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e868-112">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="5e868-112">managedDeviceId</span></span>|<span data-ttu-id="5e868-113">String</span><span class="sxs-lookup"><span data-stu-id="5e868-113">String</span></span>|<span data-ttu-id="5e868-114">设备对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5e868-114">Unique identifier for the device object.</span></span>|
|<span data-ttu-id="5e868-115">payloadId</span><span class="sxs-lookup"><span data-stu-id="5e868-115">payloadId</span></span>|<span data-ttu-id="5e868-116">String</span><span class="sxs-lookup"><span data-stu-id="5e868-116">String</span></span>|<span data-ttu-id="5e868-117">有效负载对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5e868-117">Unique identifier for payload object.</span></span>|
|<span data-ttu-id="5e868-118">userId</span><span class="sxs-lookup"><span data-stu-id="5e868-118">userId</span></span>|<span data-ttu-id="5e868-119">String</span><span class="sxs-lookup"><span data-stu-id="5e868-119">String</span></span>|<span data-ttu-id="5e868-120">UserId 对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5e868-120">Unique identifier for UserId object.</span></span> <span data-ttu-id="5e868-121">可以是 null</span><span class="sxs-lookup"><span data-stu-id="5e868-121">Can be null</span></span>|
|<span data-ttu-id="5e868-122">deviceProperties</span><span class="sxs-lookup"><span data-stu-id="5e868-122">deviceProperties</span></span>|<span data-ttu-id="5e868-123">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5e868-123">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="5e868-124">在设备签入期间用于筛选器评估的设备属性。</span><span class="sxs-lookup"><span data-stu-id="5e868-124">Device properties used for filter evaluation during device check-in time.</span></span>|
|<span data-ttu-id="5e868-125">evalutionSummaries</span><span class="sxs-lookup"><span data-stu-id="5e868-125">evalutionSummaries</span></span>|<span data-ttu-id="5e868-126">[assignmentFilterEvaluationSummary](../resources/intune-policyset-assignmentfilterevaluationsummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5e868-126">[assignmentFilterEvaluationSummary](../resources/intune-policyset-assignmentfilterevaluationsummary.md) collection</span></span>|<span data-ttu-id="5e868-127">与设备和负载关联的每个筛选器的评估结果摘要</span><span class="sxs-lookup"><span data-stu-id="5e868-127">Evaluation result summaries for each filter associated to device and payload</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e868-128">关系</span><span class="sxs-lookup"><span data-stu-id="5e868-128">Relationships</span></span>
<span data-ttu-id="5e868-129">无</span><span class="sxs-lookup"><span data-stu-id="5e868-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e868-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e868-130">JSON Representation</span></span>
<span data-ttu-id="5e868-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e868-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterStatusDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterStatusDetails",
  "managedDeviceId": "String",
  "payloadId": "String",
  "userId": "String",
  "deviceProperties": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "evalutionSummaries": [
    {
      "@odata.type": "microsoft.graph.assignmentFilterEvaluationSummary",
      "assignmentFilterId": "String",
      "assignmentFilterLastModifiedDateTime": "String (timestamp)",
      "assignmentFilterDisplayName": "String",
      "assignmentFilterPlatform": "String",
      "evaluationResult": "String",
      "evaluationDateTime": "String (timestamp)",
      "assignmentFilterType": "String",
      "assignmentFilterTypeAndEvaluationResults": [
        {
          "@odata.type": "microsoft.graph.assignmentFilterTypeAndEvaluationResult",
          "assignmentFilterType": "String",
          "evaluationResult": "String"
        }
      ]
    }
  ]
}
```




