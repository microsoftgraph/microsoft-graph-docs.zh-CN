---
title: managedDeviceMobileAppConfigurationUserSummary 资源类型
description: 包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 17924a16893f42a130c5bde593bccaf6b5729bca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032254"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="dc806-103">managedDeviceMobileAppConfigurationUserSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc806-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="dc806-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dc806-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc806-105">包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="dc806-105">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="dc806-106">方法</span><span class="sxs-lookup"><span data-stu-id="dc806-106">Methods</span></span>
|<span data-ttu-id="dc806-107">方法</span><span class="sxs-lookup"><span data-stu-id="dc806-107">Method</span></span>|<span data-ttu-id="dc806-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="dc806-108">Return Type</span></span>|<span data-ttu-id="dc806-109">说明</span><span class="sxs-lookup"><span data-stu-id="dc806-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dc806-110">获取 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="dc806-110">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="dc806-111">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="dc806-111">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="dc806-112">读取 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dc806-112">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="dc806-113">更新 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="dc806-113">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="dc806-114">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="dc806-114">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="dc806-115">更新 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dc806-115">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc806-116">属性</span><span class="sxs-lookup"><span data-stu-id="dc806-116">Properties</span></span>
|<span data-ttu-id="dc806-117">属性</span><span class="sxs-lookup"><span data-stu-id="dc806-117">Property</span></span>|<span data-ttu-id="dc806-118">类型</span><span class="sxs-lookup"><span data-stu-id="dc806-118">Type</span></span>|<span data-ttu-id="dc806-119">说明</span><span class="sxs-lookup"><span data-stu-id="dc806-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc806-120">id</span><span class="sxs-lookup"><span data-stu-id="dc806-120">id</span></span>|<span data-ttu-id="dc806-121">String</span><span class="sxs-lookup"><span data-stu-id="dc806-121">String</span></span>|<span data-ttu-id="dc806-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dc806-122">Key of the entity.</span></span>|
|<span data-ttu-id="dc806-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="dc806-123">pendingCount</span></span>|<span data-ttu-id="dc806-124">Int32</span><span class="sxs-lookup"><span data-stu-id="dc806-124">Int32</span></span>|<span data-ttu-id="dc806-125">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="dc806-125">Number of pending Users</span></span>|
|<span data-ttu-id="dc806-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="dc806-126">notApplicableCount</span></span>|<span data-ttu-id="dc806-127">Int32</span><span class="sxs-lookup"><span data-stu-id="dc806-127">Int32</span></span>|<span data-ttu-id="dc806-128">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="dc806-128">Number of not applicable users</span></span>|
|<span data-ttu-id="dc806-129">successCount</span><span class="sxs-lookup"><span data-stu-id="dc806-129">successCount</span></span>|<span data-ttu-id="dc806-130">Int32</span><span class="sxs-lookup"><span data-stu-id="dc806-130">Int32</span></span>|<span data-ttu-id="dc806-131">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="dc806-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="dc806-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="dc806-132">errorCount</span></span>|<span data-ttu-id="dc806-133">Int32</span><span class="sxs-lookup"><span data-stu-id="dc806-133">Int32</span></span>|<span data-ttu-id="dc806-134">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="dc806-134">Number of error Users</span></span>|
|<span data-ttu-id="dc806-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="dc806-135">failedCount</span></span>|<span data-ttu-id="dc806-136">Int32</span><span class="sxs-lookup"><span data-stu-id="dc806-136">Int32</span></span>|<span data-ttu-id="dc806-137">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="dc806-137">Number of failed Users</span></span>|
|<span data-ttu-id="dc806-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="dc806-138">lastUpdateDateTime</span></span>|<span data-ttu-id="dc806-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc806-139">DateTimeOffset</span></span>|<span data-ttu-id="dc806-140">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="dc806-140">Last update time</span></span>|
|<span data-ttu-id="dc806-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="dc806-141">configurationVersion</span></span>|<span data-ttu-id="dc806-142">Int32</span><span class="sxs-lookup"><span data-stu-id="dc806-142">Int32</span></span>|<span data-ttu-id="dc806-143">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="dc806-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc806-144">关系</span><span class="sxs-lookup"><span data-stu-id="dc806-144">Relationships</span></span>
<span data-ttu-id="dc806-145">无</span><span class="sxs-lookup"><span data-stu-id="dc806-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc806-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc806-146">JSON Representation</span></span>
<span data-ttu-id="dc806-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc806-147">Here is a JSON representation of the resource.</span></span>
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



