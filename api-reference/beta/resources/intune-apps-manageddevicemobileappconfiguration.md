---
title: managedDeviceMobileAppConfiguration 资源类型
description: 已注册设备移动应用配置的抽象类
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a532c39a38ea033a3ed1675183528432e4e87211
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950156"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="ed350-103">managedDeviceMobileAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed350-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="ed350-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ed350-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed350-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ed350-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed350-106">已注册设备移动应用配置的抽象类</span><span class="sxs-lookup"><span data-stu-id="ed350-106">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="ed350-107">方法</span><span class="sxs-lookup"><span data-stu-id="ed350-107">Methods</span></span>
|<span data-ttu-id="ed350-108">方法</span><span class="sxs-lookup"><span data-stu-id="ed350-108">Method</span></span>|<span data-ttu-id="ed350-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ed350-109">Return Type</span></span>|<span data-ttu-id="ed350-110">说明</span><span class="sxs-lookup"><span data-stu-id="ed350-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ed350-111">List managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="ed350-111">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="ed350-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed350-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="ed350-113">列出 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ed350-113">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="ed350-114">Get managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ed350-114">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="ed350-115">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ed350-115">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="ed350-116">读取 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ed350-116">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ed350-117">分配操作</span><span class="sxs-lookup"><span data-stu-id="ed350-117">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="ed350-118">无</span><span class="sxs-lookup"><span data-stu-id="ed350-118">None</span></span>|<span data-ttu-id="ed350-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ed350-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ed350-120">属性</span><span class="sxs-lookup"><span data-stu-id="ed350-120">Properties</span></span>
|<span data-ttu-id="ed350-121">属性</span><span class="sxs-lookup"><span data-stu-id="ed350-121">Property</span></span>|<span data-ttu-id="ed350-122">类型</span><span class="sxs-lookup"><span data-stu-id="ed350-122">Type</span></span>|<span data-ttu-id="ed350-123">说明</span><span class="sxs-lookup"><span data-stu-id="ed350-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed350-124">id</span><span class="sxs-lookup"><span data-stu-id="ed350-124">id</span></span>|<span data-ttu-id="ed350-125">字符串</span><span class="sxs-lookup"><span data-stu-id="ed350-125">String</span></span>|<span data-ttu-id="ed350-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ed350-126">Key of the entity.</span></span>|
|<span data-ttu-id="ed350-127">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="ed350-127">targetedMobileApps</span></span>|<span data-ttu-id="ed350-128">String 集合</span><span class="sxs-lookup"><span data-stu-id="ed350-128">String collection</span></span>|<span data-ttu-id="ed350-129">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="ed350-129">the associated app.</span></span>|
|<span data-ttu-id="ed350-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ed350-130">roleScopeTagIds</span></span>|<span data-ttu-id="ed350-131">String collection</span><span class="sxs-lookup"><span data-stu-id="ed350-131">String collection</span></span>|<span data-ttu-id="ed350-132">此应用配置实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ed350-132">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="ed350-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed350-133">createdDateTime</span></span>|<span data-ttu-id="ed350-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed350-134">DateTimeOffset</span></span>|<span data-ttu-id="ed350-135">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ed350-135">DateTime the object was created.</span></span>|
|<span data-ttu-id="ed350-136">说明</span><span class="sxs-lookup"><span data-stu-id="ed350-136">description</span></span>|<span data-ttu-id="ed350-137">String</span><span class="sxs-lookup"><span data-stu-id="ed350-137">String</span></span>|<span data-ttu-id="ed350-138">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="ed350-138">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="ed350-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed350-139">lastModifiedDateTime</span></span>|<span data-ttu-id="ed350-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed350-140">DateTimeOffset</span></span>|<span data-ttu-id="ed350-141">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ed350-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="ed350-142">displayName</span><span class="sxs-lookup"><span data-stu-id="ed350-142">displayName</span></span>|<span data-ttu-id="ed350-143">String</span><span class="sxs-lookup"><span data-stu-id="ed350-143">String</span></span>|<span data-ttu-id="ed350-144">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="ed350-144">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="ed350-145">version</span><span class="sxs-lookup"><span data-stu-id="ed350-145">version</span></span>|<span data-ttu-id="ed350-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ed350-146">Int32</span></span>|<span data-ttu-id="ed350-147">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ed350-147">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed350-148">关系</span><span class="sxs-lookup"><span data-stu-id="ed350-148">Relationships</span></span>
|<span data-ttu-id="ed350-149">关系</span><span class="sxs-lookup"><span data-stu-id="ed350-149">Relationship</span></span>|<span data-ttu-id="ed350-150">类型</span><span class="sxs-lookup"><span data-stu-id="ed350-150">Type</span></span>|<span data-ttu-id="ed350-151">说明</span><span class="sxs-lookup"><span data-stu-id="ed350-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed350-152">assignments</span><span class="sxs-lookup"><span data-stu-id="ed350-152">assignments</span></span>|<span data-ttu-id="ed350-153">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed350-153">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ed350-154">应用配置的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="ed350-154">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="ed350-155">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="ed350-155">deviceStatuses</span></span>|<span data-ttu-id="ed350-156">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="ed350-156">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="ed350-157">ManagedDeviceMobileAppConfigurationDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="ed350-157">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="ed350-158">userStatuses</span><span class="sxs-lookup"><span data-stu-id="ed350-158">userStatuses</span></span>|<span data-ttu-id="ed350-159">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed350-159">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="ed350-160">ManagedDeviceMobileAppConfigurationUserStatus 列表</span><span class="sxs-lookup"><span data-stu-id="ed350-160">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="ed350-161">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="ed350-161">deviceStatusSummary</span></span>|[<span data-ttu-id="ed350-162">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="ed350-162">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="ed350-163">应用配置设备状态摘要。</span><span class="sxs-lookup"><span data-stu-id="ed350-163">App configuration device status summary.</span></span>|
|<span data-ttu-id="ed350-164">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="ed350-164">userStatusSummary</span></span>|[<span data-ttu-id="ed350-165">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="ed350-165">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="ed350-166">应用配置用户状态摘要。</span><span class="sxs-lookup"><span data-stu-id="ed350-166">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed350-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed350-167">JSON Representation</span></span>
<span data-ttu-id="ed350-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed350-168">Here is a JSON representation of the resource.</span></span>
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
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```




