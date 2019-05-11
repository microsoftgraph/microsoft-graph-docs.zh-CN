---
title: deviceManagementIntentUserStateSummary 资源类型
description: 表示意向的用户状态摘要的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b4b13d4dc368c52686aa4d003a0f5995762ec56
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943450"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a><span data-ttu-id="8665b-103">deviceManagementIntentUserStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="8665b-103">deviceManagementIntentUserStateSummary resource type</span></span>

> <span data-ttu-id="8665b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8665b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8665b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8665b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8665b-106">表示意向的用户状态摘要的实体</span><span class="sxs-lookup"><span data-stu-id="8665b-106">Entity that represents user state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="8665b-107">方法</span><span class="sxs-lookup"><span data-stu-id="8665b-107">Methods</span></span>
|<span data-ttu-id="8665b-108">方法</span><span class="sxs-lookup"><span data-stu-id="8665b-108">Method</span></span>|<span data-ttu-id="8665b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8665b-109">Return Type</span></span>|<span data-ttu-id="8665b-110">说明</span><span class="sxs-lookup"><span data-stu-id="8665b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8665b-111">获取 deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="8665b-111">Get deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[<span data-ttu-id="8665b-112">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="8665b-112">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="8665b-113">读取[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8665b-113">Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|
|[<span data-ttu-id="8665b-114">更新 deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="8665b-114">Update deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[<span data-ttu-id="8665b-115">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="8665b-115">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="8665b-116">更新[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8665b-116">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8665b-117">属性</span><span class="sxs-lookup"><span data-stu-id="8665b-117">Properties</span></span>
|<span data-ttu-id="8665b-118">属性</span><span class="sxs-lookup"><span data-stu-id="8665b-118">Property</span></span>|<span data-ttu-id="8665b-119">类型</span><span class="sxs-lookup"><span data-stu-id="8665b-119">Type</span></span>|<span data-ttu-id="8665b-120">说明</span><span class="sxs-lookup"><span data-stu-id="8665b-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8665b-121">id</span><span class="sxs-lookup"><span data-stu-id="8665b-121">id</span></span>|<span data-ttu-id="8665b-122">String</span><span class="sxs-lookup"><span data-stu-id="8665b-122">String</span></span>|<span data-ttu-id="8665b-123">ID</span><span class="sxs-lookup"><span data-stu-id="8665b-123">The ID</span></span>|
|<span data-ttu-id="8665b-124">conflictCount</span><span class="sxs-lookup"><span data-stu-id="8665b-124">conflictCount</span></span>|<span data-ttu-id="8665b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="8665b-125">Int32</span></span>|<span data-ttu-id="8665b-126">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="8665b-126">Number of users in conflict</span></span>|
|<span data-ttu-id="8665b-127">errorCount</span><span class="sxs-lookup"><span data-stu-id="8665b-127">errorCount</span></span>|<span data-ttu-id="8665b-128">Int32</span><span class="sxs-lookup"><span data-stu-id="8665b-128">Int32</span></span>|<span data-ttu-id="8665b-129">错误用户数</span><span class="sxs-lookup"><span data-stu-id="8665b-129">Number of error users</span></span>|
|<span data-ttu-id="8665b-130">failedCount</span><span class="sxs-lookup"><span data-stu-id="8665b-130">failedCount</span></span>|<span data-ttu-id="8665b-131">Int32</span><span class="sxs-lookup"><span data-stu-id="8665b-131">Int32</span></span>|<span data-ttu-id="8665b-132">失败的用户数</span><span class="sxs-lookup"><span data-stu-id="8665b-132">Number of failed users</span></span>|
|<span data-ttu-id="8665b-133">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="8665b-133">notApplicableCount</span></span>|<span data-ttu-id="8665b-134">Int32</span><span class="sxs-lookup"><span data-stu-id="8665b-134">Int32</span></span>|<span data-ttu-id="8665b-135">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="8665b-135">Number of not applicable users</span></span>|
|<span data-ttu-id="8665b-136">successCount</span><span class="sxs-lookup"><span data-stu-id="8665b-136">successCount</span></span>|<span data-ttu-id="8665b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8665b-137">Int32</span></span>|<span data-ttu-id="8665b-138">成功的用户数</span><span class="sxs-lookup"><span data-stu-id="8665b-138">Number of succeeded users</span></span>|

## <a name="relationships"></a><span data-ttu-id="8665b-139">关系</span><span class="sxs-lookup"><span data-stu-id="8665b-139">Relationships</span></span>
<span data-ttu-id="8665b-140">无</span><span class="sxs-lookup"><span data-stu-id="8665b-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8665b-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8665b-141">JSON Representation</span></span>
<span data-ttu-id="8665b-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8665b-142">Here is a JSON representation of the resource.</span></span>
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




