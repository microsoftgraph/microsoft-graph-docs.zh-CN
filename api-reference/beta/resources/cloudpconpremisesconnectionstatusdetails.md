---
title: cloudPcOnPremisesConnectionStatusDetails 资源类型
description: 云电脑本地连接的状态详细信息。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 7ef9847190fb851482d29535d0709f3d74bbf3aa
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722172"
---
# <a name="cloudpconpremisesconnectionstatusdetails-resource-type"></a><span data-ttu-id="07ffc-103">cloudPcOnPremisesConnectionStatusDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="07ffc-103">cloudPcOnPremisesConnectionStatusDetails resource type</span></span>

<span data-ttu-id="07ffc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07ffc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07ffc-105">[cloudPcOnPremisesConnection 的状态详细信息](../resources/cloudpconpremisesconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="07ffc-105">The status details of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="07ffc-106">属性</span><span class="sxs-lookup"><span data-stu-id="07ffc-106">Properties</span></span>

|<span data-ttu-id="07ffc-107">属性</span><span class="sxs-lookup"><span data-stu-id="07ffc-107">Property</span></span>|<span data-ttu-id="07ffc-108">类型</span><span class="sxs-lookup"><span data-stu-id="07ffc-108">Type</span></span>|<span data-ttu-id="07ffc-109">说明</span><span class="sxs-lookup"><span data-stu-id="07ffc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07ffc-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="07ffc-110">startDateTime</span></span>|<span data-ttu-id="07ffc-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07ffc-111">DateTimeOffset</span></span>|<span data-ttu-id="07ffc-112">连接运行状况检查的开始时间。</span><span class="sxs-lookup"><span data-stu-id="07ffc-112">The start time of the connection health check.</span></span> <span data-ttu-id="07ffc-113">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="07ffc-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="07ffc-114">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="07ffc-114">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="07ffc-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="07ffc-115">endDateTime</span></span>|<span data-ttu-id="07ffc-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07ffc-116">DateTimeOffset</span></span>|<span data-ttu-id="07ffc-117">连接运行状况检查的结束时间。</span><span class="sxs-lookup"><span data-stu-id="07ffc-117">The end time of the connection health check.</span></span> <span data-ttu-id="07ffc-118">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="07ffc-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="07ffc-119">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="07ffc-119">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="07ffc-120">healthChecks</span><span class="sxs-lookup"><span data-stu-id="07ffc-120">healthChecks</span></span>|<span data-ttu-id="07ffc-121">[cloudPcOnPremisesConnectionHealthCheck](../resources/cloudpconpremisesconnectionhealthcheck.md) 集合</span><span class="sxs-lookup"><span data-stu-id="07ffc-121">[cloudPcOnPremisesConnectionHealthCheck](../resources/cloudpconpremisesconnectionhealthcheck.md) collection</span></span>|<span data-ttu-id="07ffc-122">对连接执行的所有检查。</span><span class="sxs-lookup"><span data-stu-id="07ffc-122">All checks that are done on the connection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07ffc-123">关系</span><span class="sxs-lookup"><span data-stu-id="07ffc-123">Relationships</span></span>

<span data-ttu-id="07ffc-124">无。</span><span class="sxs-lookup"><span data-stu-id="07ffc-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="07ffc-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07ffc-125">JSON representation</span></span>

<span data-ttu-id="07ffc-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07ffc-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionStatusDetails"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnectionStatusDetails",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "healthChecks": [
    {
      "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
      "displayName": "String",
      "status": "String",
      "startDateTime": "String (timestamp)",
      "endDateTime": "String (timestamp)",
      "errorType": "String",
      "recommendedAction": "String",
      "additionalDetails": "String"
    }
  ]
}
```
