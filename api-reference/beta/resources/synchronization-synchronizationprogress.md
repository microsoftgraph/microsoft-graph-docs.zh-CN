---
title: synchronizationProgress 资源类型
description: 代表完成 synchronizationJob 的进度。
ms.openlocfilehash: 412b7754dac97a36efe082026ab360569c0fe789
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049095"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="6adf7-103">synchronizationProgress 资源类型</span><span class="sxs-lookup"><span data-stu-id="6adf7-103">synchronizationProgress resource type</span></span>

> <span data-ttu-id="6adf7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6adf7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6adf7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6adf7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6adf7-106">代表完成[synchronizationJob](synchronization-synchronizationjob.md)的进度。</span><span class="sxs-lookup"><span data-stu-id="6adf7-106">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="6adf7-107">属性</span><span class="sxs-lookup"><span data-stu-id="6adf7-107">Properties</span></span>

| <span data-ttu-id="6adf7-108">属性</span><span class="sxs-lookup"><span data-stu-id="6adf7-108">Property</span></span>                              | <span data-ttu-id="6adf7-109">类型</span><span class="sxs-lookup"><span data-stu-id="6adf7-109">Type</span></span>      | <span data-ttu-id="6adf7-110">说明</span><span class="sxs-lookup"><span data-stu-id="6adf7-110">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="6adf7-111">completedUnits</span><span class="sxs-lookup"><span data-stu-id="6adf7-111">completedUnits</span></span>|<span data-ttu-id="6adf7-112">Int32</span><span class="sxs-lookup"><span data-stu-id="6adf7-112">Int32</span></span>|<span data-ttu-id="6adf7-113">进度比例; 分子已处理的更改的单位数。</span><span class="sxs-lookup"><span data-stu-id="6adf7-113">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="6adf7-114">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="6adf7-114">progressObservationDateTime</span></span>|<span data-ttu-id="6adf7-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6adf7-115">DateTimeOffset</span></span>|<span data-ttu-id="6adf7-116">进度观察值作为偏移量，以分钟为单位从 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="6adf7-116">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="6adf7-117">totalUnits</span><span class="sxs-lookup"><span data-stu-id="6adf7-117">totalUnits</span></span>|<span data-ttu-id="6adf7-118">Int32</span><span class="sxs-lookup"><span data-stu-id="6adf7-118">Int32</span></span>|<span data-ttu-id="6adf7-119">进度比例; 分母处理以完成同步更改的单位数。</span><span class="sxs-lookup"><span data-stu-id="6adf7-119">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="6adf7-120">单位</span><span class="sxs-lookup"><span data-stu-id="6adf7-120">units</span></span>|<span data-ttu-id="6adf7-121">字符串</span><span class="sxs-lookup"><span data-stu-id="6adf7-121">String</span></span>|<span data-ttu-id="6adf7-122">单位的可选说明。</span><span class="sxs-lookup"><span data-stu-id="6adf7-122">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="6adf7-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6adf7-123">JSON representation</span></span>

<span data-ttu-id="6adf7-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6adf7-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
