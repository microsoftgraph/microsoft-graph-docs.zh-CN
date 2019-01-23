---
title: deviceConfigurationUserOverview 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3a100c5d7acfa352641e0d009f22bb498a8dbce
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415493"
---
# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="921cc-103">deviceConfigurationUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="921cc-103">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="921cc-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="921cc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="921cc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="921cc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="921cc-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="921cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="921cc-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="921cc-107">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="921cc-108">方法</span><span class="sxs-lookup"><span data-stu-id="921cc-108">Methods</span></span>
|<span data-ttu-id="921cc-109">方法</span><span class="sxs-lookup"><span data-stu-id="921cc-109">Method</span></span>|<span data-ttu-id="921cc-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="921cc-110">Return Type</span></span>|<span data-ttu-id="921cc-111">说明</span><span class="sxs-lookup"><span data-stu-id="921cc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="921cc-112">获取 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="921cc-112">Get deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-get.md)|[<span data-ttu-id="921cc-113">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="921cc-113">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="921cc-114">读取 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="921cc-114">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="921cc-115">更新 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="921cc-115">Update deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-update.md)|[<span data-ttu-id="921cc-116">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="921cc-116">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="921cc-117">更新 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="921cc-117">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="921cc-118">属性</span><span class="sxs-lookup"><span data-stu-id="921cc-118">Properties</span></span>
|<span data-ttu-id="921cc-119">属性</span><span class="sxs-lookup"><span data-stu-id="921cc-119">Property</span></span>|<span data-ttu-id="921cc-120">类型</span><span class="sxs-lookup"><span data-stu-id="921cc-120">Type</span></span>|<span data-ttu-id="921cc-121">说明</span><span class="sxs-lookup"><span data-stu-id="921cc-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="921cc-122">id</span><span class="sxs-lookup"><span data-stu-id="921cc-122">id</span></span>|<span data-ttu-id="921cc-123">String</span><span class="sxs-lookup"><span data-stu-id="921cc-123">String</span></span>|<span data-ttu-id="921cc-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="921cc-124">Key of the entity.</span></span>|
|<span data-ttu-id="921cc-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="921cc-125">pendingCount</span></span>|<span data-ttu-id="921cc-126">Int32</span><span class="sxs-lookup"><span data-stu-id="921cc-126">Int32</span></span>|<span data-ttu-id="921cc-127">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="921cc-127">Number of pending Users</span></span>|
|<span data-ttu-id="921cc-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="921cc-128">notApplicableCount</span></span>|<span data-ttu-id="921cc-129">Int32</span><span class="sxs-lookup"><span data-stu-id="921cc-129">Int32</span></span>|<span data-ttu-id="921cc-130">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="921cc-130">Number of not applicable users</span></span>|
|<span data-ttu-id="921cc-131">successCount</span><span class="sxs-lookup"><span data-stu-id="921cc-131">successCount</span></span>|<span data-ttu-id="921cc-132">Int32</span><span class="sxs-lookup"><span data-stu-id="921cc-132">Int32</span></span>|<span data-ttu-id="921cc-133">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="921cc-133">Number of succeeded Users</span></span>|
|<span data-ttu-id="921cc-134">errorCount</span><span class="sxs-lookup"><span data-stu-id="921cc-134">errorCount</span></span>|<span data-ttu-id="921cc-135">Int32</span><span class="sxs-lookup"><span data-stu-id="921cc-135">Int32</span></span>|<span data-ttu-id="921cc-136">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="921cc-136">Number of error Users</span></span>|
|<span data-ttu-id="921cc-137">failedCount</span><span class="sxs-lookup"><span data-stu-id="921cc-137">failedCount</span></span>|<span data-ttu-id="921cc-138">Int32</span><span class="sxs-lookup"><span data-stu-id="921cc-138">Int32</span></span>|<span data-ttu-id="921cc-139">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="921cc-139">Number of failed Users</span></span>|
|<span data-ttu-id="921cc-140">conflictCount</span><span class="sxs-lookup"><span data-stu-id="921cc-140">conflictCount</span></span>|<span data-ttu-id="921cc-141">Int32</span><span class="sxs-lookup"><span data-stu-id="921cc-141">Int32</span></span>|<span data-ttu-id="921cc-142">存在冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="921cc-142">Number of users in conflict</span></span>|
|<span data-ttu-id="921cc-143">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="921cc-143">lastUpdateDateTime</span></span>|<span data-ttu-id="921cc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="921cc-144">DateTimeOffset</span></span>|<span data-ttu-id="921cc-145">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="921cc-145">Last update time</span></span>|
|<span data-ttu-id="921cc-146">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="921cc-146">configurationVersion</span></span>|<span data-ttu-id="921cc-147">Int32</span><span class="sxs-lookup"><span data-stu-id="921cc-147">Int32</span></span>|<span data-ttu-id="921cc-148">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="921cc-148">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="921cc-149">关系</span><span class="sxs-lookup"><span data-stu-id="921cc-149">Relationships</span></span>
<span data-ttu-id="921cc-150">无</span><span class="sxs-lookup"><span data-stu-id="921cc-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="921cc-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="921cc-151">JSON Representation</span></span>
<span data-ttu-id="921cc-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="921cc-152">Here is a JSON representation of the resource.</span></span>
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




