---
title: serviceHealth 资源类型
description: 表示服务的运行状况信息。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c11750bbffe64315c6263a26d7dbab333f42b7cf
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109097"
---
# <a name="servicehealth-resource-type"></a><span data-ttu-id="163c0-103">serviceHealth 资源类型</span><span class="sxs-lookup"><span data-stu-id="163c0-103">serviceHealth resource type</span></span>

<span data-ttu-id="163c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="163c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="163c0-105">表示服务的运行状况信息。</span><span class="sxs-lookup"><span data-stu-id="163c0-105">Represents the health information of a service.</span></span>

## <a name="methods"></a><span data-ttu-id="163c0-106">方法</span><span class="sxs-lookup"><span data-stu-id="163c0-106">Methods</span></span>
|<span data-ttu-id="163c0-107">方法</span><span class="sxs-lookup"><span data-stu-id="163c0-107">Method</span></span>|<span data-ttu-id="163c0-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="163c0-108">Return type</span></span>|<span data-ttu-id="163c0-109">说明</span><span class="sxs-lookup"><span data-stu-id="163c0-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="163c0-110">获取 serviceHealth</span><span class="sxs-lookup"><span data-stu-id="163c0-110">Get serviceHealth</span></span>](../api/servicehealth-get.md)|[<span data-ttu-id="163c0-111">serviceHealth</span><span class="sxs-lookup"><span data-stu-id="163c0-111">serviceHealth</span></span>](../resources/servicehealth.md)|<span data-ttu-id="163c0-112">检索 [serviceHealth 对象的属性和](../resources/servicehealth.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="163c0-112">Retrieve the properties and relationships of a [serviceHealth](../resources/servicehealth.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="163c0-113">属性</span><span class="sxs-lookup"><span data-stu-id="163c0-113">Properties</span></span>
|<span data-ttu-id="163c0-114">属性</span><span class="sxs-lookup"><span data-stu-id="163c0-114">Property</span></span>|<span data-ttu-id="163c0-115">类型</span><span class="sxs-lookup"><span data-stu-id="163c0-115">Type</span></span>|<span data-ttu-id="163c0-116">说明</span><span class="sxs-lookup"><span data-stu-id="163c0-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="163c0-117">id</span><span class="sxs-lookup"><span data-stu-id="163c0-117">id</span></span>|<span data-ttu-id="163c0-118">字符串</span><span class="sxs-lookup"><span data-stu-id="163c0-118">String</span></span>|<span data-ttu-id="163c0-119">服务 ID。</span><span class="sxs-lookup"><span data-stu-id="163c0-119">The service id.</span></span>|
|<span data-ttu-id="163c0-120">service</span><span class="sxs-lookup"><span data-stu-id="163c0-120">service</span></span>|<span data-ttu-id="163c0-121">String</span><span class="sxs-lookup"><span data-stu-id="163c0-121">String</span></span>|<span data-ttu-id="163c0-122">服务名称。</span><span class="sxs-lookup"><span data-stu-id="163c0-122">The service name.</span></span>|
|<span data-ttu-id="163c0-123">状态</span><span class="sxs-lookup"><span data-stu-id="163c0-123">status</span></span>|<span data-ttu-id="163c0-124">serviceHealthStatus</span><span class="sxs-lookup"><span data-stu-id="163c0-124">serviceHealthStatus</span></span>|<span data-ttu-id="163c0-125">显示一性服务运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="163c0-125">Show the overral service health status.</span></span> <span data-ttu-id="163c0-126">可能的值是 `serviceOperational` `investigating` `restoringService` ：、、、、、、、、、 `verifyingService` `serviceRestored` `postIncidentReviewPublished` `serviceDegradation` `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` `reported` `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="163c0-126">Possible values are: `serviceOperational`, `investigating`, `restoringService`, `verifyingService`, `serviceRestored`, `postIncidentReviewPublished`, `serviceDegradation`, `serviceInterruption`, `extendedRecovery`, `falsePositive`, `investigationSuspended`, `resolved`, `mitigatedExternal`, `mitigated`, `resolvedExternal`, `confirmed`, `reported`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="163c0-127">关系</span><span class="sxs-lookup"><span data-stu-id="163c0-127">Relationships</span></span>
|<span data-ttu-id="163c0-128">关系</span><span class="sxs-lookup"><span data-stu-id="163c0-128">Relationship</span></span>|<span data-ttu-id="163c0-129">类型</span><span class="sxs-lookup"><span data-stu-id="163c0-129">Type</span></span>|<span data-ttu-id="163c0-130">说明</span><span class="sxs-lookup"><span data-stu-id="163c0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="163c0-131">问题</span><span class="sxs-lookup"><span data-stu-id="163c0-131">issues</span></span>|<span data-ttu-id="163c0-132">collection ([serviceHealthIssue) ](../resources/servicehealthissue.md)</span><span class="sxs-lookup"><span data-stu-id="163c0-132">Collection([serviceHealthIssue](../resources/servicehealthissue.md))</span></span>|<span data-ttu-id="163c0-133">服务上发生的问题集合，以及每个问题的详细信息。</span><span class="sxs-lookup"><span data-stu-id="163c0-133">A collection of issues happened on the service, with detailed information for each issue.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="163c0-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="163c0-134">JSON representation</span></span>
<span data-ttu-id="163c0-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="163c0-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceHealth",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealth",
  "service": "String",
  "status": "String",
  "id": "String (identifier)"
}
```

