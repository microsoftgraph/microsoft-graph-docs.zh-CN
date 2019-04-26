---
title: deviceConfigurationUserOverview 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a36d7bb5aa3680252db848e0733186536819cf5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567254"
---
# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="ed258-103">deviceConfigurationUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed258-103">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="ed258-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ed258-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed258-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ed258-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed258-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ed258-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="ed258-107">方法</span><span class="sxs-lookup"><span data-stu-id="ed258-107">Methods</span></span>
|<span data-ttu-id="ed258-108">方法</span><span class="sxs-lookup"><span data-stu-id="ed258-108">Method</span></span>|<span data-ttu-id="ed258-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ed258-109">Return Type</span></span>|<span data-ttu-id="ed258-110">说明</span><span class="sxs-lookup"><span data-stu-id="ed258-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ed258-111">获取 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="ed258-111">Get deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-get.md)|[<span data-ttu-id="ed258-112">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="ed258-112">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="ed258-113">读取 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ed258-113">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="ed258-114">更新 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="ed258-114">Update deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-update.md)|[<span data-ttu-id="ed258-115">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="ed258-115">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="ed258-116">更新 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ed258-116">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ed258-117">属性</span><span class="sxs-lookup"><span data-stu-id="ed258-117">Properties</span></span>
|<span data-ttu-id="ed258-118">属性</span><span class="sxs-lookup"><span data-stu-id="ed258-118">Property</span></span>|<span data-ttu-id="ed258-119">类型</span><span class="sxs-lookup"><span data-stu-id="ed258-119">Type</span></span>|<span data-ttu-id="ed258-120">说明</span><span class="sxs-lookup"><span data-stu-id="ed258-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed258-121">id</span><span class="sxs-lookup"><span data-stu-id="ed258-121">id</span></span>|<span data-ttu-id="ed258-122">String</span><span class="sxs-lookup"><span data-stu-id="ed258-122">String</span></span>|<span data-ttu-id="ed258-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ed258-123">Key of the entity.</span></span>|
|<span data-ttu-id="ed258-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="ed258-124">pendingCount</span></span>|<span data-ttu-id="ed258-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ed258-125">Int32</span></span>|<span data-ttu-id="ed258-126">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="ed258-126">Number of pending Users</span></span>|
|<span data-ttu-id="ed258-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="ed258-127">notApplicableCount</span></span>|<span data-ttu-id="ed258-128">Int32</span><span class="sxs-lookup"><span data-stu-id="ed258-128">Int32</span></span>|<span data-ttu-id="ed258-129">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="ed258-129">Number of not applicable users</span></span>|
|<span data-ttu-id="ed258-130">successCount</span><span class="sxs-lookup"><span data-stu-id="ed258-130">successCount</span></span>|<span data-ttu-id="ed258-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ed258-131">Int32</span></span>|<span data-ttu-id="ed258-132">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="ed258-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="ed258-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="ed258-133">errorCount</span></span>|<span data-ttu-id="ed258-134">Int32</span><span class="sxs-lookup"><span data-stu-id="ed258-134">Int32</span></span>|<span data-ttu-id="ed258-135">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="ed258-135">Number of error Users</span></span>|
|<span data-ttu-id="ed258-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="ed258-136">failedCount</span></span>|<span data-ttu-id="ed258-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ed258-137">Int32</span></span>|<span data-ttu-id="ed258-138">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="ed258-138">Number of failed Users</span></span>|
|<span data-ttu-id="ed258-139">conflictCount</span><span class="sxs-lookup"><span data-stu-id="ed258-139">conflictCount</span></span>|<span data-ttu-id="ed258-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ed258-140">Int32</span></span>|<span data-ttu-id="ed258-141">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="ed258-141">Number of users in conflict</span></span>|
|<span data-ttu-id="ed258-142">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="ed258-142">lastUpdateDateTime</span></span>|<span data-ttu-id="ed258-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed258-143">DateTimeOffset</span></span>|<span data-ttu-id="ed258-144">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="ed258-144">Last update time</span></span>|
|<span data-ttu-id="ed258-145">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="ed258-145">configurationVersion</span></span>|<span data-ttu-id="ed258-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ed258-146">Int32</span></span>|<span data-ttu-id="ed258-147">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="ed258-147">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed258-148">关系</span><span class="sxs-lookup"><span data-stu-id="ed258-148">Relationships</span></span>
<span data-ttu-id="ed258-149">无</span><span class="sxs-lookup"><span data-stu-id="ed258-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed258-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed258-150">JSON Representation</span></span>
<span data-ttu-id="ed258-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed258-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
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





