---
title: deviceConfigurationUserOverview 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 74f56723702b50e855cc99f108950c708545fa5c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303778"
---
# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="686b2-103">deviceConfigurationUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="686b2-103">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="686b2-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="686b2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="686b2-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="686b2-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="686b2-106">方法</span><span class="sxs-lookup"><span data-stu-id="686b2-106">Methods</span></span>
|<span data-ttu-id="686b2-107">方法</span><span class="sxs-lookup"><span data-stu-id="686b2-107">Method</span></span>|<span data-ttu-id="686b2-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="686b2-108">Return Type</span></span>|<span data-ttu-id="686b2-109">说明</span><span class="sxs-lookup"><span data-stu-id="686b2-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="686b2-110">获取 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="686b2-110">Get deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-get.md)|[<span data-ttu-id="686b2-111">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="686b2-111">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="686b2-112">读取 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="686b2-112">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="686b2-113">更新 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="686b2-113">Update deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-update.md)|[<span data-ttu-id="686b2-114">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="686b2-114">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="686b2-115">更新 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="686b2-115">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="686b2-116">属性</span><span class="sxs-lookup"><span data-stu-id="686b2-116">Properties</span></span>
|<span data-ttu-id="686b2-117">属性</span><span class="sxs-lookup"><span data-stu-id="686b2-117">Property</span></span>|<span data-ttu-id="686b2-118">类型</span><span class="sxs-lookup"><span data-stu-id="686b2-118">Type</span></span>|<span data-ttu-id="686b2-119">说明</span><span class="sxs-lookup"><span data-stu-id="686b2-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="686b2-120">id</span><span class="sxs-lookup"><span data-stu-id="686b2-120">id</span></span>|<span data-ttu-id="686b2-121">String</span><span class="sxs-lookup"><span data-stu-id="686b2-121">String</span></span>|<span data-ttu-id="686b2-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="686b2-122">Key of the entity.</span></span>|
|<span data-ttu-id="686b2-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="686b2-123">pendingCount</span></span>|<span data-ttu-id="686b2-124">Int32</span><span class="sxs-lookup"><span data-stu-id="686b2-124">Int32</span></span>|<span data-ttu-id="686b2-125">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="686b2-125">Number of pending Users</span></span>|
|<span data-ttu-id="686b2-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="686b2-126">notApplicableCount</span></span>|<span data-ttu-id="686b2-127">Int32</span><span class="sxs-lookup"><span data-stu-id="686b2-127">Int32</span></span>|<span data-ttu-id="686b2-128">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="686b2-128">Number of not applicable users</span></span>|
|<span data-ttu-id="686b2-129">successCount</span><span class="sxs-lookup"><span data-stu-id="686b2-129">successCount</span></span>|<span data-ttu-id="686b2-130">Int32</span><span class="sxs-lookup"><span data-stu-id="686b2-130">Int32</span></span>|<span data-ttu-id="686b2-131">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="686b2-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="686b2-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="686b2-132">errorCount</span></span>|<span data-ttu-id="686b2-133">Int32</span><span class="sxs-lookup"><span data-stu-id="686b2-133">Int32</span></span>|<span data-ttu-id="686b2-134">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="686b2-134">Number of error Users</span></span>|
|<span data-ttu-id="686b2-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="686b2-135">failedCount</span></span>|<span data-ttu-id="686b2-136">Int32</span><span class="sxs-lookup"><span data-stu-id="686b2-136">Int32</span></span>|<span data-ttu-id="686b2-137">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="686b2-137">Number of failed Users</span></span>|
|<span data-ttu-id="686b2-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="686b2-138">lastUpdateDateTime</span></span>|<span data-ttu-id="686b2-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="686b2-139">DateTimeOffset</span></span>|<span data-ttu-id="686b2-140">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="686b2-140">Last update time</span></span>|
|<span data-ttu-id="686b2-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="686b2-141">configurationVersion</span></span>|<span data-ttu-id="686b2-142">Int32</span><span class="sxs-lookup"><span data-stu-id="686b2-142">Int32</span></span>|<span data-ttu-id="686b2-143">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="686b2-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="686b2-144">关系</span><span class="sxs-lookup"><span data-stu-id="686b2-144">Relationships</span></span>
<span data-ttu-id="686b2-145">无</span><span class="sxs-lookup"><span data-stu-id="686b2-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="686b2-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="686b2-146">JSON Representation</span></span>
<span data-ttu-id="686b2-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="686b2-147">Here is a JSON representation of the resource.</span></span>
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



