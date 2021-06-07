---
title: managedDeviceMobileAppConfigurationUserSummary 资源类型
description: 包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 342f3a300a50eb4a1b90c6b488ac864a827cbfb9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752222"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="6c060-103">managedDeviceMobileAppConfigurationUserSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c060-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

<span data-ttu-id="6c060-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c060-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c060-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6c060-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c060-106">包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="6c060-106">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="6c060-107">Methods</span><span class="sxs-lookup"><span data-stu-id="6c060-107">Methods</span></span>
|<span data-ttu-id="6c060-108">方法</span><span class="sxs-lookup"><span data-stu-id="6c060-108">Method</span></span>|<span data-ttu-id="6c060-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="6c060-109">Return Type</span></span>|<span data-ttu-id="6c060-110">Description</span><span class="sxs-lookup"><span data-stu-id="6c060-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6c060-111">获取 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="6c060-111">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="6c060-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="6c060-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="6c060-113">读取 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6c060-113">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="6c060-114">更新 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="6c060-114">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="6c060-115">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="6c060-115">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="6c060-116">更新 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6c060-116">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c060-117">属性</span><span class="sxs-lookup"><span data-stu-id="6c060-117">Properties</span></span>
|<span data-ttu-id="6c060-118">属性</span><span class="sxs-lookup"><span data-stu-id="6c060-118">Property</span></span>|<span data-ttu-id="6c060-119">类型</span><span class="sxs-lookup"><span data-stu-id="6c060-119">Type</span></span>|<span data-ttu-id="6c060-120">说明</span><span class="sxs-lookup"><span data-stu-id="6c060-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c060-121">id</span><span class="sxs-lookup"><span data-stu-id="6c060-121">id</span></span>|<span data-ttu-id="6c060-122">String</span><span class="sxs-lookup"><span data-stu-id="6c060-122">String</span></span>|<span data-ttu-id="6c060-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6c060-123">Key of the entity.</span></span>|
|<span data-ttu-id="6c060-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="6c060-124">pendingCount</span></span>|<span data-ttu-id="6c060-125">Int32</span><span class="sxs-lookup"><span data-stu-id="6c060-125">Int32</span></span>|<span data-ttu-id="6c060-126">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="6c060-126">Number of pending Users</span></span>|
|<span data-ttu-id="6c060-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="6c060-127">notApplicableCount</span></span>|<span data-ttu-id="6c060-128">Int32</span><span class="sxs-lookup"><span data-stu-id="6c060-128">Int32</span></span>|<span data-ttu-id="6c060-129">不适用用户的数量</span><span class="sxs-lookup"><span data-stu-id="6c060-129">Number of not applicable users</span></span>|
|<span data-ttu-id="6c060-130">successCount</span><span class="sxs-lookup"><span data-stu-id="6c060-130">successCount</span></span>|<span data-ttu-id="6c060-131">Int32</span><span class="sxs-lookup"><span data-stu-id="6c060-131">Int32</span></span>|<span data-ttu-id="6c060-132">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="6c060-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="6c060-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="6c060-133">errorCount</span></span>|<span data-ttu-id="6c060-134">Int32</span><span class="sxs-lookup"><span data-stu-id="6c060-134">Int32</span></span>|<span data-ttu-id="6c060-135">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="6c060-135">Number of error Users</span></span>|
|<span data-ttu-id="6c060-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="6c060-136">failedCount</span></span>|<span data-ttu-id="6c060-137">Int32</span><span class="sxs-lookup"><span data-stu-id="6c060-137">Int32</span></span>|<span data-ttu-id="6c060-138">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="6c060-138">Number of failed Users</span></span>|
|<span data-ttu-id="6c060-139">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="6c060-139">lastUpdateDateTime</span></span>|<span data-ttu-id="6c060-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c060-140">DateTimeOffset</span></span>|<span data-ttu-id="6c060-141">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="6c060-141">Last update time</span></span>|
|<span data-ttu-id="6c060-142">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="6c060-142">configurationVersion</span></span>|<span data-ttu-id="6c060-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6c060-143">Int32</span></span>|<span data-ttu-id="6c060-144">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="6c060-144">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c060-145">关系</span><span class="sxs-lookup"><span data-stu-id="6c060-145">Relationships</span></span>
<span data-ttu-id="6c060-146">无</span><span class="sxs-lookup"><span data-stu-id="6c060-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c060-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c060-147">JSON Representation</span></span>
<span data-ttu-id="6c060-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c060-148">Here is a JSON representation of the resource.</span></span>
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




