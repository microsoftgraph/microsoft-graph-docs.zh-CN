---
title: deviceConfigurationUserOverview 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c3595687f21b5121272255857dc5daeae0e01c2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259694"
---
# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="c1814-103">deviceConfigurationUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1814-103">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="c1814-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1814-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1814-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c1814-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="c1814-106">方法</span><span class="sxs-lookup"><span data-stu-id="c1814-106">Methods</span></span>
|<span data-ttu-id="c1814-107">方法</span><span class="sxs-lookup"><span data-stu-id="c1814-107">Method</span></span>|<span data-ttu-id="c1814-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c1814-108">Return Type</span></span>|<span data-ttu-id="c1814-109">说明</span><span class="sxs-lookup"><span data-stu-id="c1814-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c1814-110">获取 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="c1814-110">Get deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-get.md)|[<span data-ttu-id="c1814-111">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="c1814-111">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="c1814-112">读取 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c1814-112">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="c1814-113">更新 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="c1814-113">Update deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-update.md)|[<span data-ttu-id="c1814-114">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="c1814-114">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="c1814-115">更新 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c1814-115">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c1814-116">属性</span><span class="sxs-lookup"><span data-stu-id="c1814-116">Properties</span></span>
|<span data-ttu-id="c1814-117">属性</span><span class="sxs-lookup"><span data-stu-id="c1814-117">Property</span></span>|<span data-ttu-id="c1814-118">类型</span><span class="sxs-lookup"><span data-stu-id="c1814-118">Type</span></span>|<span data-ttu-id="c1814-119">说明</span><span class="sxs-lookup"><span data-stu-id="c1814-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1814-120">id</span><span class="sxs-lookup"><span data-stu-id="c1814-120">id</span></span>|<span data-ttu-id="c1814-121">String</span><span class="sxs-lookup"><span data-stu-id="c1814-121">String</span></span>|<span data-ttu-id="c1814-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c1814-122">Key of the entity.</span></span>|
|<span data-ttu-id="c1814-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="c1814-123">pendingCount</span></span>|<span data-ttu-id="c1814-124">Int32</span><span class="sxs-lookup"><span data-stu-id="c1814-124">Int32</span></span>|<span data-ttu-id="c1814-125">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="c1814-125">Number of pending Users</span></span>|
|<span data-ttu-id="c1814-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="c1814-126">notApplicableCount</span></span>|<span data-ttu-id="c1814-127">Int32</span><span class="sxs-lookup"><span data-stu-id="c1814-127">Int32</span></span>|<span data-ttu-id="c1814-128">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="c1814-128">Number of not applicable users</span></span>|
|<span data-ttu-id="c1814-129">successCount</span><span class="sxs-lookup"><span data-stu-id="c1814-129">successCount</span></span>|<span data-ttu-id="c1814-130">Int32</span><span class="sxs-lookup"><span data-stu-id="c1814-130">Int32</span></span>|<span data-ttu-id="c1814-131">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="c1814-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="c1814-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="c1814-132">errorCount</span></span>|<span data-ttu-id="c1814-133">Int32</span><span class="sxs-lookup"><span data-stu-id="c1814-133">Int32</span></span>|<span data-ttu-id="c1814-134">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="c1814-134">Number of error Users</span></span>|
|<span data-ttu-id="c1814-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="c1814-135">failedCount</span></span>|<span data-ttu-id="c1814-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c1814-136">Int32</span></span>|<span data-ttu-id="c1814-137">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="c1814-137">Number of failed Users</span></span>|
|<span data-ttu-id="c1814-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="c1814-138">lastUpdateDateTime</span></span>|<span data-ttu-id="c1814-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1814-139">DateTimeOffset</span></span>|<span data-ttu-id="c1814-140">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="c1814-140">Last update time</span></span>|
|<span data-ttu-id="c1814-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="c1814-141">configurationVersion</span></span>|<span data-ttu-id="c1814-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c1814-142">Int32</span></span>|<span data-ttu-id="c1814-143">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="c1814-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1814-144">关系</span><span class="sxs-lookup"><span data-stu-id="c1814-144">Relationships</span></span>
<span data-ttu-id="c1814-145">无</span><span class="sxs-lookup"><span data-stu-id="c1814-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1814-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1814-146">JSON Representation</span></span>
<span data-ttu-id="c1814-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1814-147">Here is a JSON representation of the resource.</span></span>
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



