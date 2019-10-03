---
title: managedDeviceMobileAppConfiguration 资源类型
description: 已注册设备移动应用配置的抽象类
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2973c07eb4e694f3d231adc5513e0a9cb5aa8dd0
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368258"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="cb6a4-103">managedDeviceMobileAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb6a4-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="cb6a4-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cb6a4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb6a4-105">已注册设备移动应用配置的抽象类</span><span class="sxs-lookup"><span data-stu-id="cb6a4-105">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="cb6a4-106">方法</span><span class="sxs-lookup"><span data-stu-id="cb6a4-106">Methods</span></span>
|<span data-ttu-id="cb6a4-107">方法</span><span class="sxs-lookup"><span data-stu-id="cb6a4-107">Method</span></span>|<span data-ttu-id="cb6a4-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="cb6a4-108">Return Type</span></span>|<span data-ttu-id="cb6a4-109">说明</span><span class="sxs-lookup"><span data-stu-id="cb6a4-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cb6a4-110">List managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="cb6a4-110">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="cb6a4-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cb6a4-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="cb6a4-112">列出 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cb6a4-112">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="cb6a4-113">Get managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb6a4-113">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="cb6a4-114">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb6a4-114">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="cb6a4-115">读取 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cb6a4-115">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="cb6a4-116">分配操作</span><span class="sxs-lookup"><span data-stu-id="cb6a4-116">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="cb6a4-117">无</span><span class="sxs-lookup"><span data-stu-id="cb6a4-117">None</span></span>|<span data-ttu-id="cb6a4-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cb6a4-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="cb6a4-119">属性</span><span class="sxs-lookup"><span data-stu-id="cb6a4-119">Properties</span></span>
|<span data-ttu-id="cb6a4-120">属性</span><span class="sxs-lookup"><span data-stu-id="cb6a4-120">Property</span></span>|<span data-ttu-id="cb6a4-121">类型</span><span class="sxs-lookup"><span data-stu-id="cb6a4-121">Type</span></span>|<span data-ttu-id="cb6a4-122">说明</span><span class="sxs-lookup"><span data-stu-id="cb6a4-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb6a4-123">id</span><span class="sxs-lookup"><span data-stu-id="cb6a4-123">id</span></span>|<span data-ttu-id="cb6a4-124">字符串</span><span class="sxs-lookup"><span data-stu-id="cb6a4-124">String</span></span>|<span data-ttu-id="cb6a4-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cb6a4-125">Key of the entity.</span></span>|
|<span data-ttu-id="cb6a4-126">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="cb6a4-126">targetedMobileApps</span></span>|<span data-ttu-id="cb6a4-127">String 集合</span><span class="sxs-lookup"><span data-stu-id="cb6a4-127">String collection</span></span>|<span data-ttu-id="cb6a4-128">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="cb6a4-128">the associated app.</span></span>|
|<span data-ttu-id="cb6a4-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb6a4-129">createdDateTime</span></span>|<span data-ttu-id="cb6a4-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb6a4-130">DateTimeOffset</span></span>|<span data-ttu-id="cb6a4-131">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cb6a4-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="cb6a4-132">说明</span><span class="sxs-lookup"><span data-stu-id="cb6a4-132">description</span></span>|<span data-ttu-id="cb6a4-133">String</span><span class="sxs-lookup"><span data-stu-id="cb6a4-133">String</span></span>|<span data-ttu-id="cb6a4-134">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="cb6a4-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="cb6a4-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb6a4-135">lastModifiedDateTime</span></span>|<span data-ttu-id="cb6a4-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb6a4-136">DateTimeOffset</span></span>|<span data-ttu-id="cb6a4-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cb6a4-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="cb6a4-138">displayName</span><span class="sxs-lookup"><span data-stu-id="cb6a4-138">displayName</span></span>|<span data-ttu-id="cb6a4-139">String</span><span class="sxs-lookup"><span data-stu-id="cb6a4-139">String</span></span>|<span data-ttu-id="cb6a4-140">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="cb6a4-140">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="cb6a4-141">version</span><span class="sxs-lookup"><span data-stu-id="cb6a4-141">version</span></span>|<span data-ttu-id="cb6a4-142">Int32</span><span class="sxs-lookup"><span data-stu-id="cb6a4-142">Int32</span></span>|<span data-ttu-id="cb6a4-143">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="cb6a4-143">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb6a4-144">关系</span><span class="sxs-lookup"><span data-stu-id="cb6a4-144">Relationships</span></span>
|<span data-ttu-id="cb6a4-145">关系</span><span class="sxs-lookup"><span data-stu-id="cb6a4-145">Relationship</span></span>|<span data-ttu-id="cb6a4-146">类型</span><span class="sxs-lookup"><span data-stu-id="cb6a4-146">Type</span></span>|<span data-ttu-id="cb6a4-147">说明</span><span class="sxs-lookup"><span data-stu-id="cb6a4-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb6a4-148">assignments</span><span class="sxs-lookup"><span data-stu-id="cb6a4-148">assignments</span></span>|<span data-ttu-id="cb6a4-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cb6a4-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="cb6a4-150">应用配置的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="cb6a4-150">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="cb6a4-151">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="cb6a4-151">deviceStatuses</span></span>|<span data-ttu-id="cb6a4-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="cb6a4-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="cb6a4-153">ManagedDeviceMobileAppConfigurationDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="cb6a4-153">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="cb6a4-154">userStatuses</span><span class="sxs-lookup"><span data-stu-id="cb6a4-154">userStatuses</span></span>|<span data-ttu-id="cb6a4-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cb6a4-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="cb6a4-156">ManagedDeviceMobileAppConfigurationUserStatus 列表</span><span class="sxs-lookup"><span data-stu-id="cb6a4-156">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="cb6a4-157">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="cb6a4-157">deviceStatusSummary</span></span>|[<span data-ttu-id="cb6a4-158">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="cb6a4-158">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="cb6a4-159">应用配置设备状态摘要。</span><span class="sxs-lookup"><span data-stu-id="cb6a4-159">App configuration device status summary.</span></span>|
|<span data-ttu-id="cb6a4-160">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="cb6a4-160">userStatusSummary</span></span>|[<span data-ttu-id="cb6a4-161">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="cb6a4-161">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="cb6a4-162">应用配置用户状态摘要。</span><span class="sxs-lookup"><span data-stu-id="cb6a4-162">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb6a4-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb6a4-163">JSON Representation</span></span>
<span data-ttu-id="cb6a4-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb6a4-164">Here is a JSON representation of the resource.</span></span>
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




