---
title: cloudPcOnPremisesConnectionStatusDetails 资源类型
description: 云 PC 本地连接的状态详细信息。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: db40df3bcd89ac21eb50870e82fe6a34ced86828
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563770"
---
# <a name="cloudpconpremisesconnectionstatusdetails-resource-type"></a><span data-ttu-id="fa443-103">cloudPcOnPremisesConnectionStatusDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa443-103">cloudPcOnPremisesConnectionStatusDetails resource type</span></span>

<span data-ttu-id="fa443-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa443-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa443-105">[CloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)的状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="fa443-105">The status details of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="fa443-106">属性</span><span class="sxs-lookup"><span data-stu-id="fa443-106">Properties</span></span>

|<span data-ttu-id="fa443-107">属性</span><span class="sxs-lookup"><span data-stu-id="fa443-107">Property</span></span>|<span data-ttu-id="fa443-108">类型</span><span class="sxs-lookup"><span data-stu-id="fa443-108">Type</span></span>|<span data-ttu-id="fa443-109">说明</span><span class="sxs-lookup"><span data-stu-id="fa443-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa443-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fa443-110">startDateTime</span></span>|<span data-ttu-id="fa443-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa443-111">DateTimeOffset</span></span>|<span data-ttu-id="fa443-112">连接运行状况检查的开始时间。</span><span class="sxs-lookup"><span data-stu-id="fa443-112">The start time of the connection health check.</span></span> <span data-ttu-id="fa443-113">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="fa443-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fa443-114">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="fa443-114">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="fa443-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="fa443-115">endDateTime</span></span>|<span data-ttu-id="fa443-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa443-116">DateTimeOffset</span></span>|<span data-ttu-id="fa443-117">连接运行状况检查的结束时间。</span><span class="sxs-lookup"><span data-stu-id="fa443-117">The end time of the connection health check.</span></span> <span data-ttu-id="fa443-118">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="fa443-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fa443-119">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="fa443-119">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="fa443-120">healthChecks</span><span class="sxs-lookup"><span data-stu-id="fa443-120">healthChecks</span></span>|<span data-ttu-id="fa443-121">[cloudPcOnPremisesConnectionHealthCheck](../resources/cloudpconpremisesconnectionhealthcheck.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fa443-121">[cloudPcOnPremisesConnectionHealthCheck](../resources/cloudpconpremisesconnectionhealthcheck.md) collection</span></span>|<span data-ttu-id="fa443-122">对连接进行的所有检查。</span><span class="sxs-lookup"><span data-stu-id="fa443-122">All checks that are done on the connection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa443-123">关系</span><span class="sxs-lookup"><span data-stu-id="fa443-123">Relationships</span></span>

<span data-ttu-id="fa443-124">无。</span><span class="sxs-lookup"><span data-stu-id="fa443-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa443-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa443-125">JSON representation</span></span>

<span data-ttu-id="fa443-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa443-126">The following is a JSON representation of the resource.</span></span>
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
