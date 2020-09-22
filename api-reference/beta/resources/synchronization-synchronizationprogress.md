---
title: synchronizationProgress 资源类型
description: 表示 synchronizationJob 的进度向完成。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5040cb32b664497f2cbed9dc9ca77ce2a2a54ee7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023826"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="1348b-103">synchronizationProgress 资源类型</span><span class="sxs-lookup"><span data-stu-id="1348b-103">synchronizationProgress resource type</span></span>

<span data-ttu-id="1348b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1348b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1348b-105">表示 [synchronizationJob](synchronization-synchronizationjob.md) 的进度向完成。</span><span class="sxs-lookup"><span data-stu-id="1348b-105">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="1348b-106">属性</span><span class="sxs-lookup"><span data-stu-id="1348b-106">Properties</span></span>

| <span data-ttu-id="1348b-107">属性</span><span class="sxs-lookup"><span data-stu-id="1348b-107">Property</span></span>                              | <span data-ttu-id="1348b-108">类型</span><span class="sxs-lookup"><span data-stu-id="1348b-108">Type</span></span>      | <span data-ttu-id="1348b-109">说明</span><span class="sxs-lookup"><span data-stu-id="1348b-109">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="1348b-110">completedUnits</span><span class="sxs-lookup"><span data-stu-id="1348b-110">completedUnits</span></span>|<span data-ttu-id="1348b-111">Int32</span><span class="sxs-lookup"><span data-stu-id="1348b-111">Int32</span></span>|<span data-ttu-id="1348b-112">进度比率的分子;已处理的更改的单位数。</span><span class="sxs-lookup"><span data-stu-id="1348b-112">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="1348b-113">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="1348b-113">progressObservationDateTime</span></span>|<span data-ttu-id="1348b-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1348b-114">DateTimeOffset</span></span>|<span data-ttu-id="1348b-115">进度观察的时间，作为从 UTC 的偏移量（以分钟为单位）。</span><span class="sxs-lookup"><span data-stu-id="1348b-115">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="1348b-116">totalUnits</span><span class="sxs-lookup"><span data-stu-id="1348b-116">totalUnits</span></span>|<span data-ttu-id="1348b-117">Int32</span><span class="sxs-lookup"><span data-stu-id="1348b-117">Int32</span></span>|<span data-ttu-id="1348b-118">进度比率的分母;要处理的用于完成同步的更改的多个单元。</span><span class="sxs-lookup"><span data-stu-id="1348b-118">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="1348b-119">units</span><span class="sxs-lookup"><span data-stu-id="1348b-119">units</span></span>|<span data-ttu-id="1348b-120">String</span><span class="sxs-lookup"><span data-stu-id="1348b-120">String</span></span>|<span data-ttu-id="1348b-121">单位的可选说明。</span><span class="sxs-lookup"><span data-stu-id="1348b-121">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="1348b-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1348b-122">JSON representation</span></span>

<span data-ttu-id="1348b-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1348b-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationProgress"
}-->

```json
{
  "completedUnits": 1025,
  "progressObservationDateTime": "2017-10-10T17:00:00Z",
  "totalUnits": 3024,
  "units": "pages"
}

```

<!-- uuid: 15571993-7e2f-4842-84d5-01ceb67cdc05
20185-08-14 22:30:00 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


