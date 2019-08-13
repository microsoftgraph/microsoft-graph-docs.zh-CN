---
title: deviceConfigurationUserOverview 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6d157c6e03c7a4068a3f05399b972e1d48eedfb8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332916"
---
# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="58104-103">deviceConfigurationUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="58104-103">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="58104-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="58104-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58104-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58104-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58104-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="58104-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="58104-107">方法</span><span class="sxs-lookup"><span data-stu-id="58104-107">Methods</span></span>
|<span data-ttu-id="58104-108">方法</span><span class="sxs-lookup"><span data-stu-id="58104-108">Method</span></span>|<span data-ttu-id="58104-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="58104-109">Return Type</span></span>|<span data-ttu-id="58104-110">说明</span><span class="sxs-lookup"><span data-stu-id="58104-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="58104-111">获取 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="58104-111">Get deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-get.md)|[<span data-ttu-id="58104-112">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="58104-112">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="58104-113">读取 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="58104-113">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="58104-114">更新 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="58104-114">Update deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-update.md)|[<span data-ttu-id="58104-115">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="58104-115">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="58104-116">更新 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="58104-116">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="58104-117">属性</span><span class="sxs-lookup"><span data-stu-id="58104-117">Properties</span></span>
|<span data-ttu-id="58104-118">属性</span><span class="sxs-lookup"><span data-stu-id="58104-118">Property</span></span>|<span data-ttu-id="58104-119">类型</span><span class="sxs-lookup"><span data-stu-id="58104-119">Type</span></span>|<span data-ttu-id="58104-120">说明</span><span class="sxs-lookup"><span data-stu-id="58104-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58104-121">id</span><span class="sxs-lookup"><span data-stu-id="58104-121">id</span></span>|<span data-ttu-id="58104-122">String</span><span class="sxs-lookup"><span data-stu-id="58104-122">String</span></span>|<span data-ttu-id="58104-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="58104-123">Key of the entity.</span></span>|
|<span data-ttu-id="58104-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="58104-124">pendingCount</span></span>|<span data-ttu-id="58104-125">Int32</span><span class="sxs-lookup"><span data-stu-id="58104-125">Int32</span></span>|<span data-ttu-id="58104-126">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="58104-126">Number of pending Users</span></span>|
|<span data-ttu-id="58104-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="58104-127">notApplicableCount</span></span>|<span data-ttu-id="58104-128">Int32</span><span class="sxs-lookup"><span data-stu-id="58104-128">Int32</span></span>|<span data-ttu-id="58104-129">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="58104-129">Number of not applicable users</span></span>|
|<span data-ttu-id="58104-130">successCount</span><span class="sxs-lookup"><span data-stu-id="58104-130">successCount</span></span>|<span data-ttu-id="58104-131">Int32</span><span class="sxs-lookup"><span data-stu-id="58104-131">Int32</span></span>|<span data-ttu-id="58104-132">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="58104-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="58104-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="58104-133">errorCount</span></span>|<span data-ttu-id="58104-134">Int32</span><span class="sxs-lookup"><span data-stu-id="58104-134">Int32</span></span>|<span data-ttu-id="58104-135">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="58104-135">Number of error Users</span></span>|
|<span data-ttu-id="58104-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="58104-136">failedCount</span></span>|<span data-ttu-id="58104-137">Int32</span><span class="sxs-lookup"><span data-stu-id="58104-137">Int32</span></span>|<span data-ttu-id="58104-138">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="58104-138">Number of failed Users</span></span>|
|<span data-ttu-id="58104-139">conflictCount</span><span class="sxs-lookup"><span data-stu-id="58104-139">conflictCount</span></span>|<span data-ttu-id="58104-140">Int32</span><span class="sxs-lookup"><span data-stu-id="58104-140">Int32</span></span>|<span data-ttu-id="58104-141">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="58104-141">Number of users in conflict</span></span>|
|<span data-ttu-id="58104-142">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="58104-142">lastUpdateDateTime</span></span>|<span data-ttu-id="58104-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58104-143">DateTimeOffset</span></span>|<span data-ttu-id="58104-144">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="58104-144">Last update time</span></span>|
|<span data-ttu-id="58104-145">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="58104-145">configurationVersion</span></span>|<span data-ttu-id="58104-146">Int32</span><span class="sxs-lookup"><span data-stu-id="58104-146">Int32</span></span>|<span data-ttu-id="58104-147">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="58104-147">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="58104-148">关系</span><span class="sxs-lookup"><span data-stu-id="58104-148">Relationships</span></span>
<span data-ttu-id="58104-149">无</span><span class="sxs-lookup"><span data-stu-id="58104-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58104-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58104-150">JSON Representation</span></span>
<span data-ttu-id="58104-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58104-151">Here is a JSON representation of the resource.</span></span>
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



