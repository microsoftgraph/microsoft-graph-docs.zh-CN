---
title: deviceComplianceUserOverview 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1643857a9e2dd90dab7dba983d5233bf86e5f7e1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062799"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="685ef-103">deviceComplianceUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="685ef-103">deviceComplianceUserOverview resource type</span></span>

<span data-ttu-id="685ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="685ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="685ef-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="685ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="685ef-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="685ef-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="685ef-107">方法</span><span class="sxs-lookup"><span data-stu-id="685ef-107">Methods</span></span>
|<span data-ttu-id="685ef-108">方法</span><span class="sxs-lookup"><span data-stu-id="685ef-108">Method</span></span>|<span data-ttu-id="685ef-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="685ef-109">Return Type</span></span>|<span data-ttu-id="685ef-110">说明</span><span class="sxs-lookup"><span data-stu-id="685ef-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="685ef-111">获取 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="685ef-111">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="685ef-112">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="685ef-112">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="685ef-113">读取 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="685ef-113">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="685ef-114">更新 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="685ef-114">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="685ef-115">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="685ef-115">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="685ef-116">更新 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="685ef-116">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="685ef-117">属性</span><span class="sxs-lookup"><span data-stu-id="685ef-117">Properties</span></span>
|<span data-ttu-id="685ef-118">属性</span><span class="sxs-lookup"><span data-stu-id="685ef-118">Property</span></span>|<span data-ttu-id="685ef-119">类型</span><span class="sxs-lookup"><span data-stu-id="685ef-119">Type</span></span>|<span data-ttu-id="685ef-120">说明</span><span class="sxs-lookup"><span data-stu-id="685ef-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="685ef-121">id</span><span class="sxs-lookup"><span data-stu-id="685ef-121">id</span></span>|<span data-ttu-id="685ef-122">String</span><span class="sxs-lookup"><span data-stu-id="685ef-122">String</span></span>|<span data-ttu-id="685ef-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="685ef-123">Key of the entity.</span></span>|
|<span data-ttu-id="685ef-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="685ef-124">pendingCount</span></span>|<span data-ttu-id="685ef-125">Int32</span><span class="sxs-lookup"><span data-stu-id="685ef-125">Int32</span></span>|<span data-ttu-id="685ef-126">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="685ef-126">Number of pending Users</span></span>|
|<span data-ttu-id="685ef-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="685ef-127">notApplicableCount</span></span>|<span data-ttu-id="685ef-128">Int32</span><span class="sxs-lookup"><span data-stu-id="685ef-128">Int32</span></span>|<span data-ttu-id="685ef-129">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="685ef-129">Number of not applicable users</span></span>|
|<span data-ttu-id="685ef-130">successCount</span><span class="sxs-lookup"><span data-stu-id="685ef-130">successCount</span></span>|<span data-ttu-id="685ef-131">Int32</span><span class="sxs-lookup"><span data-stu-id="685ef-131">Int32</span></span>|<span data-ttu-id="685ef-132">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="685ef-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="685ef-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="685ef-133">errorCount</span></span>|<span data-ttu-id="685ef-134">Int32</span><span class="sxs-lookup"><span data-stu-id="685ef-134">Int32</span></span>|<span data-ttu-id="685ef-135">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="685ef-135">Number of error Users</span></span>|
|<span data-ttu-id="685ef-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="685ef-136">failedCount</span></span>|<span data-ttu-id="685ef-137">Int32</span><span class="sxs-lookup"><span data-stu-id="685ef-137">Int32</span></span>|<span data-ttu-id="685ef-138">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="685ef-138">Number of failed Users</span></span>|
|<span data-ttu-id="685ef-139">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="685ef-139">lastUpdateDateTime</span></span>|<span data-ttu-id="685ef-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="685ef-140">DateTimeOffset</span></span>|<span data-ttu-id="685ef-141">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="685ef-141">Last update time</span></span>|
|<span data-ttu-id="685ef-142">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="685ef-142">configurationVersion</span></span>|<span data-ttu-id="685ef-143">Int32</span><span class="sxs-lookup"><span data-stu-id="685ef-143">Int32</span></span>|<span data-ttu-id="685ef-144">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="685ef-144">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="685ef-145">关系</span><span class="sxs-lookup"><span data-stu-id="685ef-145">Relationships</span></span>
<span data-ttu-id="685ef-146">无</span><span class="sxs-lookup"><span data-stu-id="685ef-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="685ef-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="685ef-147">JSON Representation</span></span>
<span data-ttu-id="685ef-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="685ef-148">Here is a JSON representation of the resource.</span></span>
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









