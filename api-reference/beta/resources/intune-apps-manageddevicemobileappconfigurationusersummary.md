---
title: managedDeviceMobileAppConfigurationUserSummary 资源类型
description: 包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bd8bab735b4aca908734b570cde9c8b0d557e7f1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49281423"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="80405-103">managedDeviceMobileAppConfigurationUserSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="80405-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

<span data-ttu-id="80405-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80405-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80405-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="80405-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80405-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="80405-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80405-107">包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="80405-107">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="80405-108">Methods</span><span class="sxs-lookup"><span data-stu-id="80405-108">Methods</span></span>
|<span data-ttu-id="80405-109">方法</span><span class="sxs-lookup"><span data-stu-id="80405-109">Method</span></span>|<span data-ttu-id="80405-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="80405-110">Return Type</span></span>|<span data-ttu-id="80405-111">Description</span><span class="sxs-lookup"><span data-stu-id="80405-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="80405-112">获取 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="80405-112">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="80405-113">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="80405-113">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="80405-114">读取 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="80405-114">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="80405-115">更新 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="80405-115">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="80405-116">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="80405-116">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="80405-117">更新 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="80405-117">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="80405-118">属性</span><span class="sxs-lookup"><span data-stu-id="80405-118">Properties</span></span>
|<span data-ttu-id="80405-119">属性</span><span class="sxs-lookup"><span data-stu-id="80405-119">Property</span></span>|<span data-ttu-id="80405-120">类型</span><span class="sxs-lookup"><span data-stu-id="80405-120">Type</span></span>|<span data-ttu-id="80405-121">说明</span><span class="sxs-lookup"><span data-stu-id="80405-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80405-122">id</span><span class="sxs-lookup"><span data-stu-id="80405-122">id</span></span>|<span data-ttu-id="80405-123">字符串</span><span class="sxs-lookup"><span data-stu-id="80405-123">String</span></span>|<span data-ttu-id="80405-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="80405-124">Key of the entity.</span></span>|
|<span data-ttu-id="80405-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="80405-125">pendingCount</span></span>|<span data-ttu-id="80405-126">Int32</span><span class="sxs-lookup"><span data-stu-id="80405-126">Int32</span></span>|<span data-ttu-id="80405-127">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="80405-127">Number of pending Users</span></span>|
|<span data-ttu-id="80405-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="80405-128">notApplicableCount</span></span>|<span data-ttu-id="80405-129">Int32</span><span class="sxs-lookup"><span data-stu-id="80405-129">Int32</span></span>|<span data-ttu-id="80405-130">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="80405-130">Number of not applicable users</span></span>|
|<span data-ttu-id="80405-131">successCount</span><span class="sxs-lookup"><span data-stu-id="80405-131">successCount</span></span>|<span data-ttu-id="80405-132">Int32</span><span class="sxs-lookup"><span data-stu-id="80405-132">Int32</span></span>|<span data-ttu-id="80405-133">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="80405-133">Number of succeeded Users</span></span>|
|<span data-ttu-id="80405-134">errorCount</span><span class="sxs-lookup"><span data-stu-id="80405-134">errorCount</span></span>|<span data-ttu-id="80405-135">Int32</span><span class="sxs-lookup"><span data-stu-id="80405-135">Int32</span></span>|<span data-ttu-id="80405-136">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="80405-136">Number of error Users</span></span>|
|<span data-ttu-id="80405-137">failedCount</span><span class="sxs-lookup"><span data-stu-id="80405-137">failedCount</span></span>|<span data-ttu-id="80405-138">Int32</span><span class="sxs-lookup"><span data-stu-id="80405-138">Int32</span></span>|<span data-ttu-id="80405-139">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="80405-139">Number of failed Users</span></span>|
|<span data-ttu-id="80405-140">conflictCount</span><span class="sxs-lookup"><span data-stu-id="80405-140">conflictCount</span></span>|<span data-ttu-id="80405-141">Int32</span><span class="sxs-lookup"><span data-stu-id="80405-141">Int32</span></span>|<span data-ttu-id="80405-142">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="80405-142">Number of users in conflict</span></span>|
|<span data-ttu-id="80405-143">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="80405-143">lastUpdateDateTime</span></span>|<span data-ttu-id="80405-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80405-144">DateTimeOffset</span></span>|<span data-ttu-id="80405-145">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="80405-145">Last update time</span></span>|
|<span data-ttu-id="80405-146">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="80405-146">configurationVersion</span></span>|<span data-ttu-id="80405-147">Int32</span><span class="sxs-lookup"><span data-stu-id="80405-147">Int32</span></span>|<span data-ttu-id="80405-148">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="80405-148">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="80405-149">关系</span><span class="sxs-lookup"><span data-stu-id="80405-149">Relationships</span></span>
<span data-ttu-id="80405-150">无</span><span class="sxs-lookup"><span data-stu-id="80405-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80405-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80405-151">JSON Representation</span></span>
<span data-ttu-id="80405-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80405-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
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




