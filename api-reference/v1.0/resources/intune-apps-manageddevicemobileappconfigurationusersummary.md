---
title: managedDeviceMobileAppConfigurationUserSummary 资源类型
description: 包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 96ec2f44864e29f374ab9ccf3f63a65a91692087
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564020"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="4a660-103">managedDeviceMobileAppConfigurationUserSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a660-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="4a660-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4a660-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a660-105">包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="4a660-105">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="4a660-106">方法</span><span class="sxs-lookup"><span data-stu-id="4a660-106">Methods</span></span>
|<span data-ttu-id="4a660-107">方法</span><span class="sxs-lookup"><span data-stu-id="4a660-107">Method</span></span>|<span data-ttu-id="4a660-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4a660-108">Return Type</span></span>|<span data-ttu-id="4a660-109">说明</span><span class="sxs-lookup"><span data-stu-id="4a660-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4a660-110">获取 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="4a660-110">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="4a660-111">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="4a660-111">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="4a660-112">读取 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4a660-112">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="4a660-113">更新 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="4a660-113">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="4a660-114">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="4a660-114">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="4a660-115">更新 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4a660-115">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4a660-116">属性</span><span class="sxs-lookup"><span data-stu-id="4a660-116">Properties</span></span>
|<span data-ttu-id="4a660-117">属性</span><span class="sxs-lookup"><span data-stu-id="4a660-117">Property</span></span>|<span data-ttu-id="4a660-118">类型</span><span class="sxs-lookup"><span data-stu-id="4a660-118">Type</span></span>|<span data-ttu-id="4a660-119">说明</span><span class="sxs-lookup"><span data-stu-id="4a660-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a660-120">id</span><span class="sxs-lookup"><span data-stu-id="4a660-120">id</span></span>|<span data-ttu-id="4a660-121">String</span><span class="sxs-lookup"><span data-stu-id="4a660-121">String</span></span>|<span data-ttu-id="4a660-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4a660-122">Key of the entity.</span></span>|
|<span data-ttu-id="4a660-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="4a660-123">pendingCount</span></span>|<span data-ttu-id="4a660-124">Int32</span><span class="sxs-lookup"><span data-stu-id="4a660-124">Int32</span></span>|<span data-ttu-id="4a660-125">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="4a660-125">Number of pending Users</span></span>|
|<span data-ttu-id="4a660-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="4a660-126">notApplicableCount</span></span>|<span data-ttu-id="4a660-127">Int32</span><span class="sxs-lookup"><span data-stu-id="4a660-127">Int32</span></span>|<span data-ttu-id="4a660-128">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="4a660-128">Number of not applicable users</span></span>|
|<span data-ttu-id="4a660-129">successCount</span><span class="sxs-lookup"><span data-stu-id="4a660-129">successCount</span></span>|<span data-ttu-id="4a660-130">Int32</span><span class="sxs-lookup"><span data-stu-id="4a660-130">Int32</span></span>|<span data-ttu-id="4a660-131">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="4a660-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="4a660-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="4a660-132">errorCount</span></span>|<span data-ttu-id="4a660-133">Int32</span><span class="sxs-lookup"><span data-stu-id="4a660-133">Int32</span></span>|<span data-ttu-id="4a660-134">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="4a660-134">Number of error Users</span></span>|
|<span data-ttu-id="4a660-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="4a660-135">failedCount</span></span>|<span data-ttu-id="4a660-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4a660-136">Int32</span></span>|<span data-ttu-id="4a660-137">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="4a660-137">Number of failed Users</span></span>|
|<span data-ttu-id="4a660-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="4a660-138">lastUpdateDateTime</span></span>|<span data-ttu-id="4a660-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a660-139">DateTimeOffset</span></span>|<span data-ttu-id="4a660-140">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="4a660-140">Last update time</span></span>|
|<span data-ttu-id="4a660-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="4a660-141">configurationVersion</span></span>|<span data-ttu-id="4a660-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4a660-142">Int32</span></span>|<span data-ttu-id="4a660-143">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="4a660-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a660-144">关系</span><span class="sxs-lookup"><span data-stu-id="4a660-144">Relationships</span></span>
<span data-ttu-id="4a660-145">无</span><span class="sxs-lookup"><span data-stu-id="4a660-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a660-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a660-146">JSON Representation</span></span>
<span data-ttu-id="4a660-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a660-147">Here is a JSON representation of the resource.</span></span>
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



