---
title: deviceConfigurationUserOverview 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3e3a5f04ebef0f918b6078a7d1135ccbf05b5c73
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532565"
---
# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="632c6-103">deviceConfigurationUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="632c6-103">deviceConfigurationUserOverview resource type</span></span>

<span data-ttu-id="632c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="632c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="632c6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="632c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="632c6-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="632c6-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="632c6-107">Methods</span><span class="sxs-lookup"><span data-stu-id="632c6-107">Methods</span></span>
|<span data-ttu-id="632c6-108">方法</span><span class="sxs-lookup"><span data-stu-id="632c6-108">Method</span></span>|<span data-ttu-id="632c6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="632c6-109">Return Type</span></span>|<span data-ttu-id="632c6-110">说明</span><span class="sxs-lookup"><span data-stu-id="632c6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="632c6-111">获取 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="632c6-111">Get deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-get.md)|[<span data-ttu-id="632c6-112">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="632c6-112">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="632c6-113">读取 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="632c6-113">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="632c6-114">更新 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="632c6-114">Update deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-update.md)|[<span data-ttu-id="632c6-115">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="632c6-115">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="632c6-116">更新 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="632c6-116">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="632c6-117">属性</span><span class="sxs-lookup"><span data-stu-id="632c6-117">Properties</span></span>
|<span data-ttu-id="632c6-118">属性</span><span class="sxs-lookup"><span data-stu-id="632c6-118">Property</span></span>|<span data-ttu-id="632c6-119">类型</span><span class="sxs-lookup"><span data-stu-id="632c6-119">Type</span></span>|<span data-ttu-id="632c6-120">说明</span><span class="sxs-lookup"><span data-stu-id="632c6-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="632c6-121">id</span><span class="sxs-lookup"><span data-stu-id="632c6-121">id</span></span>|<span data-ttu-id="632c6-122">字符串</span><span class="sxs-lookup"><span data-stu-id="632c6-122">String</span></span>|<span data-ttu-id="632c6-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="632c6-123">Key of the entity.</span></span>|
|<span data-ttu-id="632c6-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="632c6-124">pendingCount</span></span>|<span data-ttu-id="632c6-125">Int32</span><span class="sxs-lookup"><span data-stu-id="632c6-125">Int32</span></span>|<span data-ttu-id="632c6-126">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="632c6-126">Number of pending Users</span></span>|
|<span data-ttu-id="632c6-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="632c6-127">notApplicableCount</span></span>|<span data-ttu-id="632c6-128">Int32</span><span class="sxs-lookup"><span data-stu-id="632c6-128">Int32</span></span>|<span data-ttu-id="632c6-129">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="632c6-129">Number of not applicable users</span></span>|
|<span data-ttu-id="632c6-130">successCount</span><span class="sxs-lookup"><span data-stu-id="632c6-130">successCount</span></span>|<span data-ttu-id="632c6-131">Int32</span><span class="sxs-lookup"><span data-stu-id="632c6-131">Int32</span></span>|<span data-ttu-id="632c6-132">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="632c6-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="632c6-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="632c6-133">errorCount</span></span>|<span data-ttu-id="632c6-134">Int32</span><span class="sxs-lookup"><span data-stu-id="632c6-134">Int32</span></span>|<span data-ttu-id="632c6-135">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="632c6-135">Number of error Users</span></span>|
|<span data-ttu-id="632c6-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="632c6-136">failedCount</span></span>|<span data-ttu-id="632c6-137">Int32</span><span class="sxs-lookup"><span data-stu-id="632c6-137">Int32</span></span>|<span data-ttu-id="632c6-138">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="632c6-138">Number of failed Users</span></span>|
|<span data-ttu-id="632c6-139">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="632c6-139">lastUpdateDateTime</span></span>|<span data-ttu-id="632c6-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="632c6-140">DateTimeOffset</span></span>|<span data-ttu-id="632c6-141">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="632c6-141">Last update time</span></span>|
|<span data-ttu-id="632c6-142">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="632c6-142">configurationVersion</span></span>|<span data-ttu-id="632c6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="632c6-143">Int32</span></span>|<span data-ttu-id="632c6-144">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="632c6-144">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="632c6-145">关系</span><span class="sxs-lookup"><span data-stu-id="632c6-145">Relationships</span></span>
<span data-ttu-id="632c6-146">无</span><span class="sxs-lookup"><span data-stu-id="632c6-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="632c6-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="632c6-147">JSON Representation</span></span>
<span data-ttu-id="632c6-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="632c6-148">Here is a JSON representation of the resource.</span></span>
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
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```




