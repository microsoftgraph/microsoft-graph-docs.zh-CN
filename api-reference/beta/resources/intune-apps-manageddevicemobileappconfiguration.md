---
title: managedDeviceMobileAppConfiguration 资源类型
description: 已注册设备移动应用配置的抽象类
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d4deb062c7b927712d0557aa3257ba719e45bc12
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458720"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="203f3-103">managedDeviceMobileAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="203f3-103">managedDeviceMobileAppConfiguration resource type</span></span>

<span data-ttu-id="203f3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="203f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="203f3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="203f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="203f3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="203f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="203f3-107">已注册设备移动应用配置的抽象类</span><span class="sxs-lookup"><span data-stu-id="203f3-107">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="203f3-108">方法</span><span class="sxs-lookup"><span data-stu-id="203f3-108">Methods</span></span>
|<span data-ttu-id="203f3-109">方法</span><span class="sxs-lookup"><span data-stu-id="203f3-109">Method</span></span>|<span data-ttu-id="203f3-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="203f3-110">Return Type</span></span>|<span data-ttu-id="203f3-111">说明</span><span class="sxs-lookup"><span data-stu-id="203f3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="203f3-112">List managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="203f3-112">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="203f3-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="203f3-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="203f3-114">列出 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="203f3-114">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="203f3-115">Get managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="203f3-115">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="203f3-116">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="203f3-116">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="203f3-117">读取 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="203f3-117">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="203f3-118">分配操作</span><span class="sxs-lookup"><span data-stu-id="203f3-118">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="203f3-119">无</span><span class="sxs-lookup"><span data-stu-id="203f3-119">None</span></span>|<span data-ttu-id="203f3-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="203f3-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="203f3-121">属性</span><span class="sxs-lookup"><span data-stu-id="203f3-121">Properties</span></span>
|<span data-ttu-id="203f3-122">属性</span><span class="sxs-lookup"><span data-stu-id="203f3-122">Property</span></span>|<span data-ttu-id="203f3-123">类型</span><span class="sxs-lookup"><span data-stu-id="203f3-123">Type</span></span>|<span data-ttu-id="203f3-124">说明</span><span class="sxs-lookup"><span data-stu-id="203f3-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="203f3-125">id</span><span class="sxs-lookup"><span data-stu-id="203f3-125">id</span></span>|<span data-ttu-id="203f3-126">字符串</span><span class="sxs-lookup"><span data-stu-id="203f3-126">String</span></span>|<span data-ttu-id="203f3-127">实体的键。</span><span class="sxs-lookup"><span data-stu-id="203f3-127">Key of the entity.</span></span>|
|<span data-ttu-id="203f3-128">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="203f3-128">targetedMobileApps</span></span>|<span data-ttu-id="203f3-129">String 集合</span><span class="sxs-lookup"><span data-stu-id="203f3-129">String collection</span></span>|<span data-ttu-id="203f3-130">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="203f3-130">the associated app.</span></span>|
|<span data-ttu-id="203f3-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="203f3-131">roleScopeTagIds</span></span>|<span data-ttu-id="203f3-132">String 集合</span><span class="sxs-lookup"><span data-stu-id="203f3-132">String collection</span></span>|<span data-ttu-id="203f3-133">此应用配置实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="203f3-133">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="203f3-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="203f3-134">createdDateTime</span></span>|<span data-ttu-id="203f3-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="203f3-135">DateTimeOffset</span></span>|<span data-ttu-id="203f3-136">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="203f3-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="203f3-137">description</span><span class="sxs-lookup"><span data-stu-id="203f3-137">description</span></span>|<span data-ttu-id="203f3-138">String</span><span class="sxs-lookup"><span data-stu-id="203f3-138">String</span></span>|<span data-ttu-id="203f3-139">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="203f3-139">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="203f3-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="203f3-140">lastModifiedDateTime</span></span>|<span data-ttu-id="203f3-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="203f3-141">DateTimeOffset</span></span>|<span data-ttu-id="203f3-142">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="203f3-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="203f3-143">displayName</span><span class="sxs-lookup"><span data-stu-id="203f3-143">displayName</span></span>|<span data-ttu-id="203f3-144">String</span><span class="sxs-lookup"><span data-stu-id="203f3-144">String</span></span>|<span data-ttu-id="203f3-145">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="203f3-145">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="203f3-146">version</span><span class="sxs-lookup"><span data-stu-id="203f3-146">version</span></span>|<span data-ttu-id="203f3-147">Int32</span><span class="sxs-lookup"><span data-stu-id="203f3-147">Int32</span></span>|<span data-ttu-id="203f3-148">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="203f3-148">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="203f3-149">关系</span><span class="sxs-lookup"><span data-stu-id="203f3-149">Relationships</span></span>
|<span data-ttu-id="203f3-150">关系</span><span class="sxs-lookup"><span data-stu-id="203f3-150">Relationship</span></span>|<span data-ttu-id="203f3-151">类型</span><span class="sxs-lookup"><span data-stu-id="203f3-151">Type</span></span>|<span data-ttu-id="203f3-152">说明</span><span class="sxs-lookup"><span data-stu-id="203f3-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="203f3-153">assignments</span><span class="sxs-lookup"><span data-stu-id="203f3-153">assignments</span></span>|<span data-ttu-id="203f3-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="203f3-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="203f3-155">应用配置的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="203f3-155">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="203f3-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="203f3-156">deviceStatuses</span></span>|<span data-ttu-id="203f3-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="203f3-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="203f3-158">ManagedDeviceMobileAppConfigurationDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="203f3-158">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="203f3-159">userStatuses</span><span class="sxs-lookup"><span data-stu-id="203f3-159">userStatuses</span></span>|<span data-ttu-id="203f3-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="203f3-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="203f3-161">ManagedDeviceMobileAppConfigurationUserStatus 列表</span><span class="sxs-lookup"><span data-stu-id="203f3-161">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="203f3-162">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="203f3-162">deviceStatusSummary</span></span>|[<span data-ttu-id="203f3-163">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="203f3-163">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="203f3-164">应用配置设备状态摘要。</span><span class="sxs-lookup"><span data-stu-id="203f3-164">App configuration device status summary.</span></span>|
|<span data-ttu-id="203f3-165">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="203f3-165">userStatusSummary</span></span>|[<span data-ttu-id="203f3-166">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="203f3-166">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="203f3-167">应用配置用户状态摘要。</span><span class="sxs-lookup"><span data-stu-id="203f3-167">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="203f3-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="203f3-168">JSON Representation</span></span>
<span data-ttu-id="203f3-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="203f3-169">Here is a JSON representation of the resource.</span></span>
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



