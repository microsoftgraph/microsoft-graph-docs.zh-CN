---
title: serviceAnnouncementBase 资源类型
description: 这是 serviceHealthIssue 和 serviceUpdateMessage 的抽象基类型。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 46e1e6428d1371683a8ad1febae990146a9fe898
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109098"
---
# <a name="serviceannouncementbase-resource-type"></a><span data-ttu-id="0d3c6-103">serviceAnnouncementBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="0d3c6-103">serviceAnnouncementBase resource type</span></span>

<span data-ttu-id="0d3c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d3c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d3c6-105">这是 [serviceHealthIssue](../resources/servicehealthissue.md) 和 [serviceUpdateMessage](../resources/serviceupdatemessage.md)的抽象基类型。</span><span class="sxs-lookup"><span data-stu-id="0d3c6-105">This is an abstract base type for [serviceHealthIssue](../resources/servicehealthissue.md) and [serviceUpdateMessage](../resources/serviceupdatemessage.md).</span></span>

<span data-ttu-id="0d3c6-106">继承自 [实体](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="0d3c6-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0d3c6-107">方法</span><span class="sxs-lookup"><span data-stu-id="0d3c6-107">Methods</span></span>
<span data-ttu-id="0d3c6-108">无。</span><span class="sxs-lookup"><span data-stu-id="0d3c6-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="0d3c6-109">属性</span><span class="sxs-lookup"><span data-stu-id="0d3c6-109">Properties</span></span>
|<span data-ttu-id="0d3c6-110">属性</span><span class="sxs-lookup"><span data-stu-id="0d3c6-110">Property</span></span>|<span data-ttu-id="0d3c6-111">类型</span><span class="sxs-lookup"><span data-stu-id="0d3c6-111">Type</span></span>|<span data-ttu-id="0d3c6-112">说明</span><span class="sxs-lookup"><span data-stu-id="0d3c6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d3c6-113">详细信息</span><span class="sxs-lookup"><span data-stu-id="0d3c6-113">details</span></span>|<span data-ttu-id="0d3c6-114">collection ([keyValuePair](../resources/keyvaluepair.md)) </span><span class="sxs-lookup"><span data-stu-id="0d3c6-114">Collection([keyValuePair](../resources/keyvaluepair.md))</span></span>|<span data-ttu-id="0d3c6-115">有关服务事件的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="0d3c6-115">Additional details about service event.</span></span> <span data-ttu-id="0d3c6-116">此属性不支持筛选器。</span><span class="sxs-lookup"><span data-stu-id="0d3c6-116">This property doesn't support filters.</span></span>|
|<span data-ttu-id="0d3c6-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0d3c6-117">endDateTime</span></span>|<span data-ttu-id="0d3c6-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d3c6-118">DateTimeOffset</span></span>|<span data-ttu-id="0d3c6-119">服务事件的结束时间。</span><span class="sxs-lookup"><span data-stu-id="0d3c6-119">The end time of the service event.</span></span>|
|<span data-ttu-id="0d3c6-120">id</span><span class="sxs-lookup"><span data-stu-id="0d3c6-120">id</span></span>|<span data-ttu-id="0d3c6-121">字符串</span><span class="sxs-lookup"><span data-stu-id="0d3c6-121">String</span></span>|<span data-ttu-id="0d3c6-122">服务事件的 ID。</span><span class="sxs-lookup"><span data-stu-id="0d3c6-122">The id of the service event.</span></span>|
|<span data-ttu-id="0d3c6-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d3c6-123">lastModifiedDateTime</span></span>|<span data-ttu-id="0d3c6-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d3c6-124">DateTimeOffset</span></span>|<span data-ttu-id="0d3c6-125">服务事件的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="0d3c6-125">The last modified time of the service event.</span></span>|
|<span data-ttu-id="0d3c6-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0d3c6-126">startDateTime</span></span>|<span data-ttu-id="0d3c6-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d3c6-127">DateTimeOffset</span></span>|<span data-ttu-id="0d3c6-128">服务事件的开始时间。</span><span class="sxs-lookup"><span data-stu-id="0d3c6-128">The start time of the service event.</span></span>|
|<span data-ttu-id="0d3c6-129">title</span><span class="sxs-lookup"><span data-stu-id="0d3c6-129">title</span></span>|<span data-ttu-id="0d3c6-130">String</span><span class="sxs-lookup"><span data-stu-id="0d3c6-130">String</span></span>|<span data-ttu-id="0d3c6-131">服务事件的标题。</span><span class="sxs-lookup"><span data-stu-id="0d3c6-131">The title of the service event.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d3c6-132">关系</span><span class="sxs-lookup"><span data-stu-id="0d3c6-132">Relationships</span></span>
<span data-ttu-id="0d3c6-133">无。</span><span class="sxs-lookup"><span data-stu-id="0d3c6-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d3c6-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d3c6-134">JSON representation</span></span>
<span data-ttu-id="0d3c6-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d3c6-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceAnnouncementBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceAnnouncementBase",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```