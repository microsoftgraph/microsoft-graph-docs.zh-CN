---
title: deviceComplianceUserOverview 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a1bf4da38dc307f60a8c58fffa7cca862a6271e2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469485"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="acccd-103">deviceComplianceUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="acccd-103">deviceComplianceUserOverview resource type</span></span>

<span data-ttu-id="acccd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acccd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="acccd-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="acccd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="acccd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="acccd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acccd-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="acccd-107">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="acccd-108">方法</span><span class="sxs-lookup"><span data-stu-id="acccd-108">Methods</span></span>
|<span data-ttu-id="acccd-109">方法</span><span class="sxs-lookup"><span data-stu-id="acccd-109">Method</span></span>|<span data-ttu-id="acccd-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="acccd-110">Return Type</span></span>|<span data-ttu-id="acccd-111">说明</span><span class="sxs-lookup"><span data-stu-id="acccd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="acccd-112">获取 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="acccd-112">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="acccd-113">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="acccd-113">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="acccd-114">读取 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="acccd-114">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="acccd-115">更新 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="acccd-115">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="acccd-116">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="acccd-116">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="acccd-117">更新 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="acccd-117">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="acccd-118">属性</span><span class="sxs-lookup"><span data-stu-id="acccd-118">Properties</span></span>
|<span data-ttu-id="acccd-119">属性</span><span class="sxs-lookup"><span data-stu-id="acccd-119">Property</span></span>|<span data-ttu-id="acccd-120">类型</span><span class="sxs-lookup"><span data-stu-id="acccd-120">Type</span></span>|<span data-ttu-id="acccd-121">说明</span><span class="sxs-lookup"><span data-stu-id="acccd-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acccd-122">id</span><span class="sxs-lookup"><span data-stu-id="acccd-122">id</span></span>|<span data-ttu-id="acccd-123">String</span><span class="sxs-lookup"><span data-stu-id="acccd-123">String</span></span>|<span data-ttu-id="acccd-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="acccd-124">Key of the entity.</span></span>|
|<span data-ttu-id="acccd-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="acccd-125">pendingCount</span></span>|<span data-ttu-id="acccd-126">Int32</span><span class="sxs-lookup"><span data-stu-id="acccd-126">Int32</span></span>|<span data-ttu-id="acccd-127">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="acccd-127">Number of pending Users</span></span>|
|<span data-ttu-id="acccd-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="acccd-128">notApplicableCount</span></span>|<span data-ttu-id="acccd-129">Int32</span><span class="sxs-lookup"><span data-stu-id="acccd-129">Int32</span></span>|<span data-ttu-id="acccd-130">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="acccd-130">Number of not applicable users</span></span>|
|<span data-ttu-id="acccd-131">successCount</span><span class="sxs-lookup"><span data-stu-id="acccd-131">successCount</span></span>|<span data-ttu-id="acccd-132">Int32</span><span class="sxs-lookup"><span data-stu-id="acccd-132">Int32</span></span>|<span data-ttu-id="acccd-133">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="acccd-133">Number of succeeded Users</span></span>|
|<span data-ttu-id="acccd-134">errorCount</span><span class="sxs-lookup"><span data-stu-id="acccd-134">errorCount</span></span>|<span data-ttu-id="acccd-135">Int32</span><span class="sxs-lookup"><span data-stu-id="acccd-135">Int32</span></span>|<span data-ttu-id="acccd-136">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="acccd-136">Number of error Users</span></span>|
|<span data-ttu-id="acccd-137">failedCount</span><span class="sxs-lookup"><span data-stu-id="acccd-137">failedCount</span></span>|<span data-ttu-id="acccd-138">Int32</span><span class="sxs-lookup"><span data-stu-id="acccd-138">Int32</span></span>|<span data-ttu-id="acccd-139">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="acccd-139">Number of failed Users</span></span>|
|<span data-ttu-id="acccd-140">conflictCount</span><span class="sxs-lookup"><span data-stu-id="acccd-140">conflictCount</span></span>|<span data-ttu-id="acccd-141">Int32</span><span class="sxs-lookup"><span data-stu-id="acccd-141">Int32</span></span>|<span data-ttu-id="acccd-142">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="acccd-142">Number of users in conflict</span></span>|
|<span data-ttu-id="acccd-143">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="acccd-143">lastUpdateDateTime</span></span>|<span data-ttu-id="acccd-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acccd-144">DateTimeOffset</span></span>|<span data-ttu-id="acccd-145">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="acccd-145">Last update time</span></span>|
|<span data-ttu-id="acccd-146">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="acccd-146">configurationVersion</span></span>|<span data-ttu-id="acccd-147">Int32</span><span class="sxs-lookup"><span data-stu-id="acccd-147">Int32</span></span>|<span data-ttu-id="acccd-148">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="acccd-148">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="acccd-149">关系</span><span class="sxs-lookup"><span data-stu-id="acccd-149">Relationships</span></span>
<span data-ttu-id="acccd-150">无</span><span class="sxs-lookup"><span data-stu-id="acccd-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="acccd-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="acccd-151">JSON Representation</span></span>
<span data-ttu-id="acccd-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="acccd-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



