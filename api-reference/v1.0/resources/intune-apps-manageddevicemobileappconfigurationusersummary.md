---
title: managedDeviceMobileAppConfigurationUserSummary 资源类型
description: 包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。
ms.openlocfilehash: 7d49218220854b2d8bba38b74d2103adace810ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008494"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="3aa77-103">managedDeviceMobileAppConfigurationUserSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="3aa77-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="3aa77-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3aa77-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3aa77-105">包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="3aa77-105">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="3aa77-106">方法</span><span class="sxs-lookup"><span data-stu-id="3aa77-106">Methods</span></span>
|<span data-ttu-id="3aa77-107">方法</span><span class="sxs-lookup"><span data-stu-id="3aa77-107">Method</span></span>|<span data-ttu-id="3aa77-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3aa77-108">Return Type</span></span>|<span data-ttu-id="3aa77-109">说明</span><span class="sxs-lookup"><span data-stu-id="3aa77-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3aa77-110">获取 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="3aa77-110">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="3aa77-111">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="3aa77-111">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="3aa77-112">读取 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3aa77-112">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="3aa77-113">更新 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="3aa77-113">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="3aa77-114">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="3aa77-114">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="3aa77-115">更新 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3aa77-115">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3aa77-116">属性</span><span class="sxs-lookup"><span data-stu-id="3aa77-116">Properties</span></span>
|<span data-ttu-id="3aa77-117">属性</span><span class="sxs-lookup"><span data-stu-id="3aa77-117">Property</span></span>|<span data-ttu-id="3aa77-118">类型</span><span class="sxs-lookup"><span data-stu-id="3aa77-118">Type</span></span>|<span data-ttu-id="3aa77-119">说明</span><span class="sxs-lookup"><span data-stu-id="3aa77-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3aa77-120">id</span><span class="sxs-lookup"><span data-stu-id="3aa77-120">id</span></span>|<span data-ttu-id="3aa77-121">String</span><span class="sxs-lookup"><span data-stu-id="3aa77-121">String</span></span>|<span data-ttu-id="3aa77-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3aa77-122">Key of the entity.</span></span>|
|<span data-ttu-id="3aa77-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="3aa77-123">pendingCount</span></span>|<span data-ttu-id="3aa77-124">Int32</span><span class="sxs-lookup"><span data-stu-id="3aa77-124">Int32</span></span>|<span data-ttu-id="3aa77-125">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="3aa77-125">Number of pending Users</span></span>|
|<span data-ttu-id="3aa77-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="3aa77-126">notApplicableCount</span></span>|<span data-ttu-id="3aa77-127">Int32</span><span class="sxs-lookup"><span data-stu-id="3aa77-127">Int32</span></span>|<span data-ttu-id="3aa77-128">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="3aa77-128">Number of not applicable users</span></span>|
|<span data-ttu-id="3aa77-129">successCount</span><span class="sxs-lookup"><span data-stu-id="3aa77-129">successCount</span></span>|<span data-ttu-id="3aa77-130">Int32</span><span class="sxs-lookup"><span data-stu-id="3aa77-130">Int32</span></span>|<span data-ttu-id="3aa77-131">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="3aa77-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="3aa77-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="3aa77-132">errorCount</span></span>|<span data-ttu-id="3aa77-133">Int32</span><span class="sxs-lookup"><span data-stu-id="3aa77-133">Int32</span></span>|<span data-ttu-id="3aa77-134">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="3aa77-134">Number of error Users</span></span>|
|<span data-ttu-id="3aa77-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="3aa77-135">failedCount</span></span>|<span data-ttu-id="3aa77-136">Int32</span><span class="sxs-lookup"><span data-stu-id="3aa77-136">Int32</span></span>|<span data-ttu-id="3aa77-137">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="3aa77-137">Number of failed Users</span></span>|
|<span data-ttu-id="3aa77-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="3aa77-138">lastUpdateDateTime</span></span>|<span data-ttu-id="3aa77-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3aa77-139">DateTimeOffset</span></span>|<span data-ttu-id="3aa77-140">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="3aa77-140">Last update time</span></span>|
|<span data-ttu-id="3aa77-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="3aa77-141">configurationVersion</span></span>|<span data-ttu-id="3aa77-142">Int32</span><span class="sxs-lookup"><span data-stu-id="3aa77-142">Int32</span></span>|<span data-ttu-id="3aa77-143">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="3aa77-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="3aa77-144">关系</span><span class="sxs-lookup"><span data-stu-id="3aa77-144">Relationships</span></span>
<span data-ttu-id="3aa77-145">无</span><span class="sxs-lookup"><span data-stu-id="3aa77-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3aa77-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3aa77-146">JSON Representation</span></span>
<span data-ttu-id="3aa77-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3aa77-147">Here is a JSON representation of the resource.</span></span>
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



