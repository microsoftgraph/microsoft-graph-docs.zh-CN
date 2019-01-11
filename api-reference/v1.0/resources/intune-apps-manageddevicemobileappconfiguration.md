---
title: managedDeviceMobileAppConfiguration 资源类型
description: 已注册设备移动应用配置的抽象类
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8e2ad71a4927f2b0156d085bad54cf59d45f97c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811646"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="66fd2-103">managedDeviceMobileAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="66fd2-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="66fd2-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="66fd2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66fd2-105">已注册设备移动应用配置的抽象类</span><span class="sxs-lookup"><span data-stu-id="66fd2-105">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="66fd2-106">方法</span><span class="sxs-lookup"><span data-stu-id="66fd2-106">Methods</span></span>
|<span data-ttu-id="66fd2-107">方法</span><span class="sxs-lookup"><span data-stu-id="66fd2-107">Method</span></span>|<span data-ttu-id="66fd2-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="66fd2-108">Return Type</span></span>|<span data-ttu-id="66fd2-109">说明</span><span class="sxs-lookup"><span data-stu-id="66fd2-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="66fd2-110">List managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="66fd2-110">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="66fd2-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66fd2-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="66fd2-112">列出 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="66fd2-112">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="66fd2-113">Get managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="66fd2-113">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="66fd2-114">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="66fd2-114">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="66fd2-115">读取 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="66fd2-115">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="66fd2-116">assign 操作</span><span class="sxs-lookup"><span data-stu-id="66fd2-116">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="66fd2-117">无</span><span class="sxs-lookup"><span data-stu-id="66fd2-117">None</span></span>|<span data-ttu-id="66fd2-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="66fd2-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="66fd2-119">属性</span><span class="sxs-lookup"><span data-stu-id="66fd2-119">Properties</span></span>
|<span data-ttu-id="66fd2-120">属性</span><span class="sxs-lookup"><span data-stu-id="66fd2-120">Property</span></span>|<span data-ttu-id="66fd2-121">类型</span><span class="sxs-lookup"><span data-stu-id="66fd2-121">Type</span></span>|<span data-ttu-id="66fd2-122">说明</span><span class="sxs-lookup"><span data-stu-id="66fd2-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66fd2-123">id</span><span class="sxs-lookup"><span data-stu-id="66fd2-123">id</span></span>|<span data-ttu-id="66fd2-124">String</span><span class="sxs-lookup"><span data-stu-id="66fd2-124">String</span></span>|<span data-ttu-id="66fd2-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="66fd2-125">Key of the entity.</span></span>|
|<span data-ttu-id="66fd2-126">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="66fd2-126">targetedMobileApps</span></span>|<span data-ttu-id="66fd2-127">String 集合</span><span class="sxs-lookup"><span data-stu-id="66fd2-127">String collection</span></span>|<span data-ttu-id="66fd2-128">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="66fd2-128">the associated app.</span></span>|
|<span data-ttu-id="66fd2-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66fd2-129">createdDateTime</span></span>|<span data-ttu-id="66fd2-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66fd2-130">DateTimeOffset</span></span>|<span data-ttu-id="66fd2-131">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="66fd2-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="66fd2-132">description</span><span class="sxs-lookup"><span data-stu-id="66fd2-132">description</span></span>|<span data-ttu-id="66fd2-133">String</span><span class="sxs-lookup"><span data-stu-id="66fd2-133">String</span></span>|<span data-ttu-id="66fd2-134">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="66fd2-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="66fd2-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66fd2-135">lastModifiedDateTime</span></span>|<span data-ttu-id="66fd2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66fd2-136">DateTimeOffset</span></span>|<span data-ttu-id="66fd2-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="66fd2-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="66fd2-138">displayName</span><span class="sxs-lookup"><span data-stu-id="66fd2-138">displayName</span></span>|<span data-ttu-id="66fd2-139">String</span><span class="sxs-lookup"><span data-stu-id="66fd2-139">String</span></span>|<span data-ttu-id="66fd2-140">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="66fd2-140">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="66fd2-141">version</span><span class="sxs-lookup"><span data-stu-id="66fd2-141">version</span></span>|<span data-ttu-id="66fd2-142">Int32</span><span class="sxs-lookup"><span data-stu-id="66fd2-142">Int32</span></span>|<span data-ttu-id="66fd2-143">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="66fd2-143">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66fd2-144">关系</span><span class="sxs-lookup"><span data-stu-id="66fd2-144">Relationships</span></span>
|<span data-ttu-id="66fd2-145">关系</span><span class="sxs-lookup"><span data-stu-id="66fd2-145">Relationship</span></span>|<span data-ttu-id="66fd2-146">类型</span><span class="sxs-lookup"><span data-stu-id="66fd2-146">Type</span></span>|<span data-ttu-id="66fd2-147">说明</span><span class="sxs-lookup"><span data-stu-id="66fd2-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66fd2-148">assignments</span><span class="sxs-lookup"><span data-stu-id="66fd2-148">assignments</span></span>|<span data-ttu-id="66fd2-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66fd2-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="66fd2-150">应用配置的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="66fd2-150">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="66fd2-151">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="66fd2-151">deviceStatuses</span></span>|<span data-ttu-id="66fd2-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="66fd2-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="66fd2-153">ManagedDeviceMobileAppConfigurationDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="66fd2-153">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="66fd2-154">userStatuses</span><span class="sxs-lookup"><span data-stu-id="66fd2-154">userStatuses</span></span>|<span data-ttu-id="66fd2-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66fd2-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="66fd2-156">ManagedDeviceMobileAppConfigurationUserStatus 列表</span><span class="sxs-lookup"><span data-stu-id="66fd2-156">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="66fd2-157">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="66fd2-157">deviceStatusSummary</span></span>|[<span data-ttu-id="66fd2-158">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="66fd2-158">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="66fd2-159">应用配置设备状态摘要。</span><span class="sxs-lookup"><span data-stu-id="66fd2-159">App configuration device status summary.</span></span>|
|<span data-ttu-id="66fd2-160">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="66fd2-160">userStatusSummary</span></span>|[<span data-ttu-id="66fd2-161">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="66fd2-161">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="66fd2-162">应用配置用户状态摘要。</span><span class="sxs-lookup"><span data-stu-id="66fd2-162">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66fd2-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66fd2-163">JSON Representation</span></span>
<span data-ttu-id="66fd2-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66fd2-164">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



