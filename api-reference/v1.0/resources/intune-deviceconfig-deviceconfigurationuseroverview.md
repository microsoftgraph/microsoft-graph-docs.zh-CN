---
title: deviceConfigurationUserOverview 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c3595687f21b5121272255857dc5daeae0e01c2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573380"
---
# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="bc8d1-103">deviceConfigurationUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc8d1-103">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="bc8d1-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc8d1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc8d1-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bc8d1-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="bc8d1-106">方法</span><span class="sxs-lookup"><span data-stu-id="bc8d1-106">Methods</span></span>
|<span data-ttu-id="bc8d1-107">方法</span><span class="sxs-lookup"><span data-stu-id="bc8d1-107">Method</span></span>|<span data-ttu-id="bc8d1-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="bc8d1-108">Return Type</span></span>|<span data-ttu-id="bc8d1-109">说明</span><span class="sxs-lookup"><span data-stu-id="bc8d1-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc8d1-110">获取 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="bc8d1-110">Get deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-get.md)|[<span data-ttu-id="bc8d1-111">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="bc8d1-111">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="bc8d1-112">读取 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bc8d1-112">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="bc8d1-113">更新 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="bc8d1-113">Update deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-update.md)|[<span data-ttu-id="bc8d1-114">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="bc8d1-114">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="bc8d1-115">更新 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bc8d1-115">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc8d1-116">属性</span><span class="sxs-lookup"><span data-stu-id="bc8d1-116">Properties</span></span>
|<span data-ttu-id="bc8d1-117">属性</span><span class="sxs-lookup"><span data-stu-id="bc8d1-117">Property</span></span>|<span data-ttu-id="bc8d1-118">类型</span><span class="sxs-lookup"><span data-stu-id="bc8d1-118">Type</span></span>|<span data-ttu-id="bc8d1-119">说明</span><span class="sxs-lookup"><span data-stu-id="bc8d1-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc8d1-120">id</span><span class="sxs-lookup"><span data-stu-id="bc8d1-120">id</span></span>|<span data-ttu-id="bc8d1-121">String</span><span class="sxs-lookup"><span data-stu-id="bc8d1-121">String</span></span>|<span data-ttu-id="bc8d1-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bc8d1-122">Key of the entity.</span></span>|
|<span data-ttu-id="bc8d1-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="bc8d1-123">pendingCount</span></span>|<span data-ttu-id="bc8d1-124">Int32</span><span class="sxs-lookup"><span data-stu-id="bc8d1-124">Int32</span></span>|<span data-ttu-id="bc8d1-125">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="bc8d1-125">Number of pending Users</span></span>|
|<span data-ttu-id="bc8d1-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="bc8d1-126">notApplicableCount</span></span>|<span data-ttu-id="bc8d1-127">Int32</span><span class="sxs-lookup"><span data-stu-id="bc8d1-127">Int32</span></span>|<span data-ttu-id="bc8d1-128">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="bc8d1-128">Number of not applicable users</span></span>|
|<span data-ttu-id="bc8d1-129">successCount</span><span class="sxs-lookup"><span data-stu-id="bc8d1-129">successCount</span></span>|<span data-ttu-id="bc8d1-130">Int32</span><span class="sxs-lookup"><span data-stu-id="bc8d1-130">Int32</span></span>|<span data-ttu-id="bc8d1-131">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="bc8d1-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="bc8d1-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="bc8d1-132">errorCount</span></span>|<span data-ttu-id="bc8d1-133">Int32</span><span class="sxs-lookup"><span data-stu-id="bc8d1-133">Int32</span></span>|<span data-ttu-id="bc8d1-134">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="bc8d1-134">Number of error Users</span></span>|
|<span data-ttu-id="bc8d1-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="bc8d1-135">failedCount</span></span>|<span data-ttu-id="bc8d1-136">Int32</span><span class="sxs-lookup"><span data-stu-id="bc8d1-136">Int32</span></span>|<span data-ttu-id="bc8d1-137">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="bc8d1-137">Number of failed Users</span></span>|
|<span data-ttu-id="bc8d1-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="bc8d1-138">lastUpdateDateTime</span></span>|<span data-ttu-id="bc8d1-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc8d1-139">DateTimeOffset</span></span>|<span data-ttu-id="bc8d1-140">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="bc8d1-140">Last update time</span></span>|
|<span data-ttu-id="bc8d1-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="bc8d1-141">configurationVersion</span></span>|<span data-ttu-id="bc8d1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="bc8d1-142">Int32</span></span>|<span data-ttu-id="bc8d1-143">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="bc8d1-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc8d1-144">关系</span><span class="sxs-lookup"><span data-stu-id="bc8d1-144">Relationships</span></span>
<span data-ttu-id="bc8d1-145">无</span><span class="sxs-lookup"><span data-stu-id="bc8d1-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc8d1-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc8d1-146">JSON Representation</span></span>
<span data-ttu-id="bc8d1-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc8d1-147">Here is a JSON representation of the resource.</span></span>
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



