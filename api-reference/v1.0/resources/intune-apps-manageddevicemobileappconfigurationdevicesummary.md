---
title: managedDeviceMobileAppConfigurationDeviceSummary 资源类型
description: 包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。
ms.openlocfilehash: 459d97fd57987fba1c760f1c716553fa71233c2f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011420"
---
# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="10307-103">managedDeviceMobileAppConfigurationDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="10307-103">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

> <span data-ttu-id="10307-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="10307-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10307-105">包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="10307-105">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="10307-106">方法</span><span class="sxs-lookup"><span data-stu-id="10307-106">Methods</span></span>
|<span data-ttu-id="10307-107">方法</span><span class="sxs-lookup"><span data-stu-id="10307-107">Method</span></span>|<span data-ttu-id="10307-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="10307-108">Return Type</span></span>|<span data-ttu-id="10307-109">说明</span><span class="sxs-lookup"><span data-stu-id="10307-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="10307-110">获取 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="10307-110">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-get.md)|[<span data-ttu-id="10307-111">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="10307-111">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="10307-112">读取 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10307-112">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="10307-113">更新 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="10307-113">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-update.md)|[<span data-ttu-id="10307-114">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="10307-114">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="10307-115">更新 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="10307-115">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="10307-116">属性</span><span class="sxs-lookup"><span data-stu-id="10307-116">Properties</span></span>
|<span data-ttu-id="10307-117">属性</span><span class="sxs-lookup"><span data-stu-id="10307-117">Property</span></span>|<span data-ttu-id="10307-118">类型</span><span class="sxs-lookup"><span data-stu-id="10307-118">Type</span></span>|<span data-ttu-id="10307-119">说明</span><span class="sxs-lookup"><span data-stu-id="10307-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10307-120">id</span><span class="sxs-lookup"><span data-stu-id="10307-120">id</span></span>|<span data-ttu-id="10307-121">String</span><span class="sxs-lookup"><span data-stu-id="10307-121">String</span></span>|<span data-ttu-id="10307-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="10307-122">Key of the entity.</span></span>|
|<span data-ttu-id="10307-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="10307-123">pendingCount</span></span>|<span data-ttu-id="10307-124">Int32</span><span class="sxs-lookup"><span data-stu-id="10307-124">Int32</span></span>|<span data-ttu-id="10307-125">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="10307-125">Number of pending devices</span></span>|
|<span data-ttu-id="10307-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="10307-126">notApplicableCount</span></span>|<span data-ttu-id="10307-127">Int32</span><span class="sxs-lookup"><span data-stu-id="10307-127">Int32</span></span>|<span data-ttu-id="10307-128">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="10307-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="10307-129">successCount</span><span class="sxs-lookup"><span data-stu-id="10307-129">successCount</span></span>|<span data-ttu-id="10307-130">Int32</span><span class="sxs-lookup"><span data-stu-id="10307-130">Int32</span></span>|<span data-ttu-id="10307-131">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="10307-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="10307-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="10307-132">errorCount</span></span>|<span data-ttu-id="10307-133">Int32</span><span class="sxs-lookup"><span data-stu-id="10307-133">Int32</span></span>|<span data-ttu-id="10307-134">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="10307-134">Number of error devices</span></span>|
|<span data-ttu-id="10307-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="10307-135">failedCount</span></span>|<span data-ttu-id="10307-136">Int32</span><span class="sxs-lookup"><span data-stu-id="10307-136">Int32</span></span>|<span data-ttu-id="10307-137">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="10307-137">Number of failed devices</span></span>|
|<span data-ttu-id="10307-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="10307-138">lastUpdateDateTime</span></span>|<span data-ttu-id="10307-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10307-139">DateTimeOffset</span></span>|<span data-ttu-id="10307-140">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="10307-140">Last update time</span></span>|
|<span data-ttu-id="10307-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="10307-141">configurationVersion</span></span>|<span data-ttu-id="10307-142">Int32</span><span class="sxs-lookup"><span data-stu-id="10307-142">Int32</span></span>|<span data-ttu-id="10307-143">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="10307-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="10307-144">关系</span><span class="sxs-lookup"><span data-stu-id="10307-144">Relationships</span></span>
<span data-ttu-id="10307-145">无</span><span class="sxs-lookup"><span data-stu-id="10307-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="10307-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10307-146">JSON Representation</span></span>
<span data-ttu-id="10307-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10307-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
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



