---
title: deviceConfigurationUserOverview 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: c844fd17e3287707a5ecacfb89c7b622497e2aac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310659"
---
# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="1df3c-103">deviceConfigurationUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="1df3c-103">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="1df3c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1df3c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1df3c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1df3c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1df3c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1df3c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1df3c-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1df3c-107">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="1df3c-108">方法</span><span class="sxs-lookup"><span data-stu-id="1df3c-108">Methods</span></span>
|<span data-ttu-id="1df3c-109">方法</span><span class="sxs-lookup"><span data-stu-id="1df3c-109">Method</span></span>|<span data-ttu-id="1df3c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1df3c-110">Return Type</span></span>|<span data-ttu-id="1df3c-111">说明</span><span class="sxs-lookup"><span data-stu-id="1df3c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1df3c-112">获取 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="1df3c-112">Get deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-get.md)|[<span data-ttu-id="1df3c-113">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="1df3c-113">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="1df3c-114">读取 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1df3c-114">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="1df3c-115">更新 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="1df3c-115">Update deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-update.md)|[<span data-ttu-id="1df3c-116">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="1df3c-116">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="1df3c-117">更新 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1df3c-117">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1df3c-118">属性</span><span class="sxs-lookup"><span data-stu-id="1df3c-118">Properties</span></span>
|<span data-ttu-id="1df3c-119">属性</span><span class="sxs-lookup"><span data-stu-id="1df3c-119">Property</span></span>|<span data-ttu-id="1df3c-120">类型</span><span class="sxs-lookup"><span data-stu-id="1df3c-120">Type</span></span>|<span data-ttu-id="1df3c-121">说明</span><span class="sxs-lookup"><span data-stu-id="1df3c-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1df3c-122">id</span><span class="sxs-lookup"><span data-stu-id="1df3c-122">id</span></span>|<span data-ttu-id="1df3c-123">String</span><span class="sxs-lookup"><span data-stu-id="1df3c-123">String</span></span>|<span data-ttu-id="1df3c-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1df3c-124">Key of the entity.</span></span>|
|<span data-ttu-id="1df3c-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="1df3c-125">pendingCount</span></span>|<span data-ttu-id="1df3c-126">Int32</span><span class="sxs-lookup"><span data-stu-id="1df3c-126">Int32</span></span>|<span data-ttu-id="1df3c-127">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="1df3c-127">Number of pending Users</span></span>|
|<span data-ttu-id="1df3c-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="1df3c-128">notApplicableCount</span></span>|<span data-ttu-id="1df3c-129">Int32</span><span class="sxs-lookup"><span data-stu-id="1df3c-129">Int32</span></span>|<span data-ttu-id="1df3c-130">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="1df3c-130">Number of not applicable users</span></span>|
|<span data-ttu-id="1df3c-131">successCount</span><span class="sxs-lookup"><span data-stu-id="1df3c-131">successCount</span></span>|<span data-ttu-id="1df3c-132">Int32</span><span class="sxs-lookup"><span data-stu-id="1df3c-132">Int32</span></span>|<span data-ttu-id="1df3c-133">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="1df3c-133">Number of succeeded Users</span></span>|
|<span data-ttu-id="1df3c-134">errorCount</span><span class="sxs-lookup"><span data-stu-id="1df3c-134">errorCount</span></span>|<span data-ttu-id="1df3c-135">Int32</span><span class="sxs-lookup"><span data-stu-id="1df3c-135">Int32</span></span>|<span data-ttu-id="1df3c-136">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="1df3c-136">Number of error Users</span></span>|
|<span data-ttu-id="1df3c-137">failedCount</span><span class="sxs-lookup"><span data-stu-id="1df3c-137">failedCount</span></span>|<span data-ttu-id="1df3c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="1df3c-138">Int32</span></span>|<span data-ttu-id="1df3c-139">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="1df3c-139">Number of failed Users</span></span>|
|<span data-ttu-id="1df3c-140">conflictCount</span><span class="sxs-lookup"><span data-stu-id="1df3c-140">conflictCount</span></span>|<span data-ttu-id="1df3c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="1df3c-141">Int32</span></span>|<span data-ttu-id="1df3c-142">存在冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="1df3c-142">Number of users in conflict</span></span>|
|<span data-ttu-id="1df3c-143">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="1df3c-143">lastUpdateDateTime</span></span>|<span data-ttu-id="1df3c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1df3c-144">DateTimeOffset</span></span>|<span data-ttu-id="1df3c-145">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="1df3c-145">Last update time</span></span>|
|<span data-ttu-id="1df3c-146">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="1df3c-146">configurationVersion</span></span>|<span data-ttu-id="1df3c-147">Int32</span><span class="sxs-lookup"><span data-stu-id="1df3c-147">Int32</span></span>|<span data-ttu-id="1df3c-148">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="1df3c-148">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="1df3c-149">关系</span><span class="sxs-lookup"><span data-stu-id="1df3c-149">Relationships</span></span>
<span data-ttu-id="1df3c-150">无</span><span class="sxs-lookup"><span data-stu-id="1df3c-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1df3c-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1df3c-151">JSON Representation</span></span>
<span data-ttu-id="1df3c-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1df3c-152">Here is a JSON representation of the resource.</span></span>
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





