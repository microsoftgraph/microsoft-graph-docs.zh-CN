---
title: deviceComplianceUserOverview 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 177c66d9c09ce8ee1ac546e987e9475c5df3264f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567527"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="32f36-103">deviceComplianceUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="32f36-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="32f36-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="32f36-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32f36-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="32f36-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="32f36-106">方法</span><span class="sxs-lookup"><span data-stu-id="32f36-106">Methods</span></span>
|<span data-ttu-id="32f36-107">方法</span><span class="sxs-lookup"><span data-stu-id="32f36-107">Method</span></span>|<span data-ttu-id="32f36-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="32f36-108">Return Type</span></span>|<span data-ttu-id="32f36-109">说明</span><span class="sxs-lookup"><span data-stu-id="32f36-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="32f36-110">获取 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="32f36-110">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="32f36-111">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="32f36-111">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="32f36-112">读取 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="32f36-112">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="32f36-113">更新 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="32f36-113">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="32f36-114">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="32f36-114">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="32f36-115">更新 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="32f36-115">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="32f36-116">属性</span><span class="sxs-lookup"><span data-stu-id="32f36-116">Properties</span></span>
|<span data-ttu-id="32f36-117">属性</span><span class="sxs-lookup"><span data-stu-id="32f36-117">Property</span></span>|<span data-ttu-id="32f36-118">类型</span><span class="sxs-lookup"><span data-stu-id="32f36-118">Type</span></span>|<span data-ttu-id="32f36-119">说明</span><span class="sxs-lookup"><span data-stu-id="32f36-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32f36-120">id</span><span class="sxs-lookup"><span data-stu-id="32f36-120">id</span></span>|<span data-ttu-id="32f36-121">String</span><span class="sxs-lookup"><span data-stu-id="32f36-121">String</span></span>|<span data-ttu-id="32f36-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="32f36-122">Key of the entity.</span></span>|
|<span data-ttu-id="32f36-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="32f36-123">pendingCount</span></span>|<span data-ttu-id="32f36-124">Int32</span><span class="sxs-lookup"><span data-stu-id="32f36-124">Int32</span></span>|<span data-ttu-id="32f36-125">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="32f36-125">Number of pending Users</span></span>|
|<span data-ttu-id="32f36-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="32f36-126">notApplicableCount</span></span>|<span data-ttu-id="32f36-127">Int32</span><span class="sxs-lookup"><span data-stu-id="32f36-127">Int32</span></span>|<span data-ttu-id="32f36-128">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="32f36-128">Number of not applicable users</span></span>|
|<span data-ttu-id="32f36-129">successCount</span><span class="sxs-lookup"><span data-stu-id="32f36-129">successCount</span></span>|<span data-ttu-id="32f36-130">Int32</span><span class="sxs-lookup"><span data-stu-id="32f36-130">Int32</span></span>|<span data-ttu-id="32f36-131">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="32f36-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="32f36-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="32f36-132">errorCount</span></span>|<span data-ttu-id="32f36-133">Int32</span><span class="sxs-lookup"><span data-stu-id="32f36-133">Int32</span></span>|<span data-ttu-id="32f36-134">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="32f36-134">Number of error Users</span></span>|
|<span data-ttu-id="32f36-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="32f36-135">failedCount</span></span>|<span data-ttu-id="32f36-136">Int32</span><span class="sxs-lookup"><span data-stu-id="32f36-136">Int32</span></span>|<span data-ttu-id="32f36-137">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="32f36-137">Number of failed Users</span></span>|
|<span data-ttu-id="32f36-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="32f36-138">lastUpdateDateTime</span></span>|<span data-ttu-id="32f36-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32f36-139">DateTimeOffset</span></span>|<span data-ttu-id="32f36-140">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="32f36-140">Last update time</span></span>|
|<span data-ttu-id="32f36-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="32f36-141">configurationVersion</span></span>|<span data-ttu-id="32f36-142">Int32</span><span class="sxs-lookup"><span data-stu-id="32f36-142">Int32</span></span>|<span data-ttu-id="32f36-143">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="32f36-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="32f36-144">关系</span><span class="sxs-lookup"><span data-stu-id="32f36-144">Relationships</span></span>
<span data-ttu-id="32f36-145">无</span><span class="sxs-lookup"><span data-stu-id="32f36-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32f36-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32f36-146">JSON Representation</span></span>
<span data-ttu-id="32f36-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32f36-147">Here is a JSON representation of the resource.</span></span>
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
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



