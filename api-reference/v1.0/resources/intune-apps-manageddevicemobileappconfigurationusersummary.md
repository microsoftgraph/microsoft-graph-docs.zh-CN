---
title: managedDeviceMobileAppConfigurationUserSummary 资源类型
description: 包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4db930c4c36fd0f3e6d26347f17dbb739e19e188
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531177"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="97283-103">managedDeviceMobileAppConfigurationUserSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="97283-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

<span data-ttu-id="97283-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97283-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97283-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="97283-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97283-106">包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="97283-106">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="97283-107">Methods</span><span class="sxs-lookup"><span data-stu-id="97283-107">Methods</span></span>
|<span data-ttu-id="97283-108">方法</span><span class="sxs-lookup"><span data-stu-id="97283-108">Method</span></span>|<span data-ttu-id="97283-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="97283-109">Return Type</span></span>|<span data-ttu-id="97283-110">说明</span><span class="sxs-lookup"><span data-stu-id="97283-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="97283-111">获取 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="97283-111">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="97283-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="97283-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="97283-113">读取 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="97283-113">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="97283-114">更新 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="97283-114">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="97283-115">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="97283-115">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="97283-116">更新 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="97283-116">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="97283-117">属性</span><span class="sxs-lookup"><span data-stu-id="97283-117">Properties</span></span>
|<span data-ttu-id="97283-118">属性</span><span class="sxs-lookup"><span data-stu-id="97283-118">Property</span></span>|<span data-ttu-id="97283-119">类型</span><span class="sxs-lookup"><span data-stu-id="97283-119">Type</span></span>|<span data-ttu-id="97283-120">说明</span><span class="sxs-lookup"><span data-stu-id="97283-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97283-121">id</span><span class="sxs-lookup"><span data-stu-id="97283-121">id</span></span>|<span data-ttu-id="97283-122">字符串</span><span class="sxs-lookup"><span data-stu-id="97283-122">String</span></span>|<span data-ttu-id="97283-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="97283-123">Key of the entity.</span></span>|
|<span data-ttu-id="97283-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="97283-124">pendingCount</span></span>|<span data-ttu-id="97283-125">Int32</span><span class="sxs-lookup"><span data-stu-id="97283-125">Int32</span></span>|<span data-ttu-id="97283-126">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="97283-126">Number of pending Users</span></span>|
|<span data-ttu-id="97283-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="97283-127">notApplicableCount</span></span>|<span data-ttu-id="97283-128">Int32</span><span class="sxs-lookup"><span data-stu-id="97283-128">Int32</span></span>|<span data-ttu-id="97283-129">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="97283-129">Number of not applicable users</span></span>|
|<span data-ttu-id="97283-130">successCount</span><span class="sxs-lookup"><span data-stu-id="97283-130">successCount</span></span>|<span data-ttu-id="97283-131">Int32</span><span class="sxs-lookup"><span data-stu-id="97283-131">Int32</span></span>|<span data-ttu-id="97283-132">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="97283-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="97283-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="97283-133">errorCount</span></span>|<span data-ttu-id="97283-134">Int32</span><span class="sxs-lookup"><span data-stu-id="97283-134">Int32</span></span>|<span data-ttu-id="97283-135">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="97283-135">Number of error Users</span></span>|
|<span data-ttu-id="97283-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="97283-136">failedCount</span></span>|<span data-ttu-id="97283-137">Int32</span><span class="sxs-lookup"><span data-stu-id="97283-137">Int32</span></span>|<span data-ttu-id="97283-138">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="97283-138">Number of failed Users</span></span>|
|<span data-ttu-id="97283-139">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="97283-139">lastUpdateDateTime</span></span>|<span data-ttu-id="97283-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97283-140">DateTimeOffset</span></span>|<span data-ttu-id="97283-141">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="97283-141">Last update time</span></span>|
|<span data-ttu-id="97283-142">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="97283-142">configurationVersion</span></span>|<span data-ttu-id="97283-143">Int32</span><span class="sxs-lookup"><span data-stu-id="97283-143">Int32</span></span>|<span data-ttu-id="97283-144">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="97283-144">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="97283-145">关系</span><span class="sxs-lookup"><span data-stu-id="97283-145">Relationships</span></span>
<span data-ttu-id="97283-146">无</span><span class="sxs-lookup"><span data-stu-id="97283-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97283-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97283-147">JSON Representation</span></span>
<span data-ttu-id="97283-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97283-148">Here is a JSON representation of the resource.</span></span>
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
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```




