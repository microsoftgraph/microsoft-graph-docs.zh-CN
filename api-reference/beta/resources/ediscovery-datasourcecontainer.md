---
title: dataSourceContainer 资源类型
description: 保管人和非保管人数据源的基类。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: e2d7d88a3d747817858853ebc6f2909b2edde65b
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080749"
---
# <a name="datasourcecontainer-resource-type"></a><span data-ttu-id="236b0-103">dataSourceContainer 资源类型</span><span class="sxs-lookup"><span data-stu-id="236b0-103">dataSourceContainer resource type</span></span>

<span data-ttu-id="236b0-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="236b0-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="236b0-105">保管人[和非](../resources/ediscovery-custodian.md)[custodialDataSource 的基类](../resources/ediscovery-noncustodialdatasource.md)。</span><span class="sxs-lookup"><span data-stu-id="236b0-105">Base class for [custodian](../resources/ediscovery-custodian.md) and [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span></span>

<span data-ttu-id="236b0-106">继承自 [实体](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="236b0-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="236b0-107">方法</span><span class="sxs-lookup"><span data-stu-id="236b0-107">Methods</span></span>

<span data-ttu-id="236b0-108">无</span><span class="sxs-lookup"><span data-stu-id="236b0-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="236b0-109">属性</span><span class="sxs-lookup"><span data-stu-id="236b0-109">Properties</span></span>

|<span data-ttu-id="236b0-110">属性</span><span class="sxs-lookup"><span data-stu-id="236b0-110">Property</span></span>|<span data-ttu-id="236b0-111">类型</span><span class="sxs-lookup"><span data-stu-id="236b0-111">Type</span></span>|<span data-ttu-id="236b0-112">说明</span><span class="sxs-lookup"><span data-stu-id="236b0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="236b0-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="236b0-113">createdDateTime</span></span>|<span data-ttu-id="236b0-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="236b0-114">DateTimeOffset</span></span>|<span data-ttu-id="236b0-115">dataSourceContainer 实体的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="236b0-115">Created date and time of the dataSourceContainer entity.</span></span>|
|<span data-ttu-id="236b0-116">displayName</span><span class="sxs-lookup"><span data-stu-id="236b0-116">displayName</span></span>|<span data-ttu-id="236b0-117">String</span><span class="sxs-lookup"><span data-stu-id="236b0-117">String</span></span>|<span data-ttu-id="236b0-118">dataSourceContainer 实体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="236b0-118">Display name of the dataSourceContainer entity.</span></span>|
|<span data-ttu-id="236b0-119">id</span><span class="sxs-lookup"><span data-stu-id="236b0-119">id</span></span>|<span data-ttu-id="236b0-120">String</span><span class="sxs-lookup"><span data-stu-id="236b0-120">String</span></span>|<span data-ttu-id="236b0-121">dataSourceContainer 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="236b0-121">Unique identifier of the dataSourceContainer.</span></span> <span data-ttu-id="236b0-122">继承自 [实体](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="236b0-122">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="236b0-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="236b0-123">lastModifiedDateTime</span></span>|<span data-ttu-id="236b0-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="236b0-124">DateTimeOffset</span></span>|<span data-ttu-id="236b0-125">dataSourceContainer 的上次修改日期和时间。</span><span class="sxs-lookup"><span data-stu-id="236b0-125">Last modified date and time of the dataSourceContainer.</span></span>|
|<span data-ttu-id="236b0-126">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="236b0-126">releasedDateTime</span></span>|<span data-ttu-id="236b0-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="236b0-127">DateTimeOffset</span></span>|<span data-ttu-id="236b0-128">从案例发布 dataSourceContainer 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="236b0-128">Date and time that the dataSourceContainer was released from the case.</span></span>|
|<span data-ttu-id="236b0-129">状态</span><span class="sxs-lookup"><span data-stu-id="236b0-129">status</span></span>|<span data-ttu-id="236b0-130">microsoft.graph.ediscovery.dataSourceContainerStatus</span><span class="sxs-lookup"><span data-stu-id="236b0-130">microsoft.graph.ediscovery.dataSourceContainerStatus</span></span>|<span data-ttu-id="236b0-131">dataSourceContainer 的最新状态。</span><span class="sxs-lookup"><span data-stu-id="236b0-131">Latest status of the dataSourceContainer.</span></span> <span data-ttu-id="236b0-132">可取值为：`Active`、`Released`。</span><span class="sxs-lookup"><span data-stu-id="236b0-132">Possible values are: `Active`, `Released`.</span></span>|

### <a name="datasourcecontainerstatus-values"></a><span data-ttu-id="236b0-133">dataSourceContainerStatus 值</span><span class="sxs-lookup"><span data-stu-id="236b0-133">dataSourceContainerStatus values</span></span>

|<span data-ttu-id="236b0-134">成员</span><span class="sxs-lookup"><span data-stu-id="236b0-134">Member</span></span>|<span data-ttu-id="236b0-135">说明</span><span class="sxs-lookup"><span data-stu-id="236b0-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="236b0-136">活动</span><span class="sxs-lookup"><span data-stu-id="236b0-136">Active</span></span>|<span data-ttu-id="236b0-137">在这种情况下，dataSourceContainer 将保留。</span><span class="sxs-lookup"><span data-stu-id="236b0-137">The dataSourceContainer is on hold in the case.</span></span>|
|<span data-ttu-id="236b0-138">已发布</span><span class="sxs-lookup"><span data-stu-id="236b0-138">Released</span></span>|<span data-ttu-id="236b0-139">在这种情况下，dataSourceContainer 从保留中释放。</span><span class="sxs-lookup"><span data-stu-id="236b0-139">The dataSourceContainer was released from hold in the case.</span></span>|

## <a name="relationships"></a><span data-ttu-id="236b0-140">关系</span><span class="sxs-lookup"><span data-stu-id="236b0-140">Relationships</span></span>

<span data-ttu-id="236b0-141">无</span><span class="sxs-lookup"><span data-stu-id="236b0-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="236b0-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="236b0-142">JSON representation</span></span>

<span data-ttu-id="236b0-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="236b0-143">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.dataSourceContainer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.dataSourceContainer",
  "id": "String (identifier)",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```
