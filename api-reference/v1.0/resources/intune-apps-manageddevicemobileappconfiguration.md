---
title: managedDeviceMobileAppConfiguration 资源类型
description: 已注册设备移动应用配置的抽象类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 462533c75ebbad87409032c1769edc3d399fda4d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756041"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="d50ec-103">managedDeviceMobileAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="d50ec-103">managedDeviceMobileAppConfiguration resource type</span></span>

<span data-ttu-id="d50ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d50ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d50ec-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d50ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d50ec-106">已注册设备移动应用配置的抽象类</span><span class="sxs-lookup"><span data-stu-id="d50ec-106">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="d50ec-107">Methods</span><span class="sxs-lookup"><span data-stu-id="d50ec-107">Methods</span></span>
|<span data-ttu-id="d50ec-108">方法</span><span class="sxs-lookup"><span data-stu-id="d50ec-108">Method</span></span>|<span data-ttu-id="d50ec-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d50ec-109">Return Type</span></span>|<span data-ttu-id="d50ec-110">Description</span><span class="sxs-lookup"><span data-stu-id="d50ec-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d50ec-111">List managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="d50ec-111">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="d50ec-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d50ec-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="d50ec-113">列出 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d50ec-113">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="d50ec-114">Get managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d50ec-114">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="d50ec-115">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d50ec-115">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="d50ec-116">读取 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d50ec-116">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d50ec-117">分配操作</span><span class="sxs-lookup"><span data-stu-id="d50ec-117">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="d50ec-118">无</span><span class="sxs-lookup"><span data-stu-id="d50ec-118">None</span></span>|<span data-ttu-id="d50ec-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d50ec-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d50ec-120">属性</span><span class="sxs-lookup"><span data-stu-id="d50ec-120">Properties</span></span>
|<span data-ttu-id="d50ec-121">属性</span><span class="sxs-lookup"><span data-stu-id="d50ec-121">Property</span></span>|<span data-ttu-id="d50ec-122">类型</span><span class="sxs-lookup"><span data-stu-id="d50ec-122">Type</span></span>|<span data-ttu-id="d50ec-123">说明</span><span class="sxs-lookup"><span data-stu-id="d50ec-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d50ec-124">id</span><span class="sxs-lookup"><span data-stu-id="d50ec-124">id</span></span>|<span data-ttu-id="d50ec-125">String</span><span class="sxs-lookup"><span data-stu-id="d50ec-125">String</span></span>|<span data-ttu-id="d50ec-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d50ec-126">Key of the entity.</span></span>|
|<span data-ttu-id="d50ec-127">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="d50ec-127">targetedMobileApps</span></span>|<span data-ttu-id="d50ec-128">String 集合</span><span class="sxs-lookup"><span data-stu-id="d50ec-128">String collection</span></span>|<span data-ttu-id="d50ec-129">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="d50ec-129">the associated app.</span></span>|
|<span data-ttu-id="d50ec-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d50ec-130">createdDateTime</span></span>|<span data-ttu-id="d50ec-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d50ec-131">DateTimeOffset</span></span>|<span data-ttu-id="d50ec-132">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d50ec-132">DateTime the object was created.</span></span>|
|<span data-ttu-id="d50ec-133">说明</span><span class="sxs-lookup"><span data-stu-id="d50ec-133">description</span></span>|<span data-ttu-id="d50ec-134">String</span><span class="sxs-lookup"><span data-stu-id="d50ec-134">String</span></span>|<span data-ttu-id="d50ec-135">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="d50ec-135">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="d50ec-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d50ec-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d50ec-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d50ec-137">DateTimeOffset</span></span>|<span data-ttu-id="d50ec-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d50ec-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="d50ec-139">displayName</span><span class="sxs-lookup"><span data-stu-id="d50ec-139">displayName</span></span>|<span data-ttu-id="d50ec-140">String</span><span class="sxs-lookup"><span data-stu-id="d50ec-140">String</span></span>|<span data-ttu-id="d50ec-141">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="d50ec-141">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="d50ec-142">version</span><span class="sxs-lookup"><span data-stu-id="d50ec-142">version</span></span>|<span data-ttu-id="d50ec-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d50ec-143">Int32</span></span>|<span data-ttu-id="d50ec-144">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d50ec-144">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d50ec-145">关系</span><span class="sxs-lookup"><span data-stu-id="d50ec-145">Relationships</span></span>
|<span data-ttu-id="d50ec-146">关系</span><span class="sxs-lookup"><span data-stu-id="d50ec-146">Relationship</span></span>|<span data-ttu-id="d50ec-147">类型</span><span class="sxs-lookup"><span data-stu-id="d50ec-147">Type</span></span>|<span data-ttu-id="d50ec-148">Description</span><span class="sxs-lookup"><span data-stu-id="d50ec-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d50ec-149">assignments</span><span class="sxs-lookup"><span data-stu-id="d50ec-149">assignments</span></span>|<span data-ttu-id="d50ec-150">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d50ec-150">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d50ec-151">应用配置的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="d50ec-151">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="d50ec-152">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="d50ec-152">deviceStatuses</span></span>|<span data-ttu-id="d50ec-153">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d50ec-153">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="d50ec-154">ManagedDeviceMobileAppConfigurationDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="d50ec-154">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="d50ec-155">userStatuses</span><span class="sxs-lookup"><span data-stu-id="d50ec-155">userStatuses</span></span>|<span data-ttu-id="d50ec-156">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d50ec-156">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="d50ec-157">ManagedDeviceMobileAppConfigurationUserStatus 列表</span><span class="sxs-lookup"><span data-stu-id="d50ec-157">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="d50ec-158">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="d50ec-158">deviceStatusSummary</span></span>|[<span data-ttu-id="d50ec-159">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="d50ec-159">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="d50ec-160">应用配置设备状态摘要。</span><span class="sxs-lookup"><span data-stu-id="d50ec-160">App configuration device status summary.</span></span>|
|<span data-ttu-id="d50ec-161">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="d50ec-161">userStatusSummary</span></span>|[<span data-ttu-id="d50ec-162">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="d50ec-162">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="d50ec-163">应用配置用户状态摘要。</span><span class="sxs-lookup"><span data-stu-id="d50ec-163">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d50ec-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d50ec-164">JSON Representation</span></span>
<span data-ttu-id="d50ec-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d50ec-165">Here is a JSON representation of the resource.</span></span>
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




