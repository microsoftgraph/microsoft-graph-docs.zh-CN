---
title: deviceManagementIntentUserStateSummary 资源类型
description: 表示意向的用户状态摘要的实体
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 77613d72f616fcaa3e179b56fcea1deed1053aef
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43389296"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a><span data-ttu-id="5e0fe-103">deviceManagementIntentUserStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e0fe-103">deviceManagementIntentUserStateSummary resource type</span></span>

<span data-ttu-id="5e0fe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e0fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e0fe-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5e0fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e0fe-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e0fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e0fe-107">表示意向的用户状态摘要的实体</span><span class="sxs-lookup"><span data-stu-id="5e0fe-107">Entity that represents user state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="5e0fe-108">方法</span><span class="sxs-lookup"><span data-stu-id="5e0fe-108">Methods</span></span>
|<span data-ttu-id="5e0fe-109">方法</span><span class="sxs-lookup"><span data-stu-id="5e0fe-109">Method</span></span>|<span data-ttu-id="5e0fe-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5e0fe-110">Return Type</span></span>|<span data-ttu-id="5e0fe-111">说明</span><span class="sxs-lookup"><span data-stu-id="5e0fe-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5e0fe-112">获取 deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="5e0fe-112">Get deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[<span data-ttu-id="5e0fe-113">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="5e0fe-113">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="5e0fe-114">读取[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5e0fe-114">Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|
|[<span data-ttu-id="5e0fe-115">更新 deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="5e0fe-115">Update deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[<span data-ttu-id="5e0fe-116">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="5e0fe-116">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="5e0fe-117">更新[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5e0fe-117">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e0fe-118">属性</span><span class="sxs-lookup"><span data-stu-id="5e0fe-118">Properties</span></span>
|<span data-ttu-id="5e0fe-119">属性</span><span class="sxs-lookup"><span data-stu-id="5e0fe-119">Property</span></span>|<span data-ttu-id="5e0fe-120">类型</span><span class="sxs-lookup"><span data-stu-id="5e0fe-120">Type</span></span>|<span data-ttu-id="5e0fe-121">说明</span><span class="sxs-lookup"><span data-stu-id="5e0fe-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e0fe-122">id</span><span class="sxs-lookup"><span data-stu-id="5e0fe-122">id</span></span>|<span data-ttu-id="5e0fe-123">字符串</span><span class="sxs-lookup"><span data-stu-id="5e0fe-123">String</span></span>|<span data-ttu-id="5e0fe-124">ID</span><span class="sxs-lookup"><span data-stu-id="5e0fe-124">The ID</span></span>|
|<span data-ttu-id="5e0fe-125">conflictCount</span><span class="sxs-lookup"><span data-stu-id="5e0fe-125">conflictCount</span></span>|<span data-ttu-id="5e0fe-126">Int32</span><span class="sxs-lookup"><span data-stu-id="5e0fe-126">Int32</span></span>|<span data-ttu-id="5e0fe-127">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="5e0fe-127">Number of users in conflict</span></span>|
|<span data-ttu-id="5e0fe-128">errorCount</span><span class="sxs-lookup"><span data-stu-id="5e0fe-128">errorCount</span></span>|<span data-ttu-id="5e0fe-129">Int32</span><span class="sxs-lookup"><span data-stu-id="5e0fe-129">Int32</span></span>|<span data-ttu-id="5e0fe-130">错误用户数</span><span class="sxs-lookup"><span data-stu-id="5e0fe-130">Number of error users</span></span>|
|<span data-ttu-id="5e0fe-131">failedCount</span><span class="sxs-lookup"><span data-stu-id="5e0fe-131">failedCount</span></span>|<span data-ttu-id="5e0fe-132">Int32</span><span class="sxs-lookup"><span data-stu-id="5e0fe-132">Int32</span></span>|<span data-ttu-id="5e0fe-133">失败的用户数</span><span class="sxs-lookup"><span data-stu-id="5e0fe-133">Number of failed users</span></span>|
|<span data-ttu-id="5e0fe-134">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="5e0fe-134">notApplicableCount</span></span>|<span data-ttu-id="5e0fe-135">Int32</span><span class="sxs-lookup"><span data-stu-id="5e0fe-135">Int32</span></span>|<span data-ttu-id="5e0fe-136">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="5e0fe-136">Number of not applicable users</span></span>|
|<span data-ttu-id="5e0fe-137">successCount</span><span class="sxs-lookup"><span data-stu-id="5e0fe-137">successCount</span></span>|<span data-ttu-id="5e0fe-138">Int32</span><span class="sxs-lookup"><span data-stu-id="5e0fe-138">Int32</span></span>|<span data-ttu-id="5e0fe-139">成功的用户数</span><span class="sxs-lookup"><span data-stu-id="5e0fe-139">Number of succeeded users</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e0fe-140">关系</span><span class="sxs-lookup"><span data-stu-id="5e0fe-140">Relationships</span></span>
<span data-ttu-id="5e0fe-141">无</span><span class="sxs-lookup"><span data-stu-id="5e0fe-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e0fe-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e0fe-142">JSON Representation</span></span>
<span data-ttu-id="5e0fe-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e0fe-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024
}
```



