---
title: managedDeviceMobileAppConfiguration 资源类型
description: 已注册设备移动应用配置的抽象类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f01078ef5e5d65140b9599e7dc25abc7f18ec8f4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49281500"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="b21ed-103">managedDeviceMobileAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="b21ed-103">managedDeviceMobileAppConfiguration resource type</span></span>

<span data-ttu-id="b21ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b21ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b21ed-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b21ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b21ed-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b21ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b21ed-107">已注册设备移动应用配置的抽象类</span><span class="sxs-lookup"><span data-stu-id="b21ed-107">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="b21ed-108">Methods</span><span class="sxs-lookup"><span data-stu-id="b21ed-108">Methods</span></span>
|<span data-ttu-id="b21ed-109">方法</span><span class="sxs-lookup"><span data-stu-id="b21ed-109">Method</span></span>|<span data-ttu-id="b21ed-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b21ed-110">Return Type</span></span>|<span data-ttu-id="b21ed-111">Description</span><span class="sxs-lookup"><span data-stu-id="b21ed-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b21ed-112">List managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="b21ed-112">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="b21ed-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b21ed-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="b21ed-114">列出 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b21ed-114">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="b21ed-115">Get managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b21ed-115">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="b21ed-116">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b21ed-116">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="b21ed-117">读取 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b21ed-117">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="b21ed-118">分配操作</span><span class="sxs-lookup"><span data-stu-id="b21ed-118">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="b21ed-119">无</span><span class="sxs-lookup"><span data-stu-id="b21ed-119">None</span></span>|<span data-ttu-id="b21ed-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b21ed-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b21ed-121">属性</span><span class="sxs-lookup"><span data-stu-id="b21ed-121">Properties</span></span>
|<span data-ttu-id="b21ed-122">属性</span><span class="sxs-lookup"><span data-stu-id="b21ed-122">Property</span></span>|<span data-ttu-id="b21ed-123">类型</span><span class="sxs-lookup"><span data-stu-id="b21ed-123">Type</span></span>|<span data-ttu-id="b21ed-124">说明</span><span class="sxs-lookup"><span data-stu-id="b21ed-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b21ed-125">id</span><span class="sxs-lookup"><span data-stu-id="b21ed-125">id</span></span>|<span data-ttu-id="b21ed-126">字符串</span><span class="sxs-lookup"><span data-stu-id="b21ed-126">String</span></span>|<span data-ttu-id="b21ed-127">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b21ed-127">Key of the entity.</span></span>|
|<span data-ttu-id="b21ed-128">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="b21ed-128">targetedMobileApps</span></span>|<span data-ttu-id="b21ed-129">String 集合</span><span class="sxs-lookup"><span data-stu-id="b21ed-129">String collection</span></span>|<span data-ttu-id="b21ed-130">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="b21ed-130">the associated app.</span></span>|
|<span data-ttu-id="b21ed-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b21ed-131">roleScopeTagIds</span></span>|<span data-ttu-id="b21ed-132">String 集合</span><span class="sxs-lookup"><span data-stu-id="b21ed-132">String collection</span></span>|<span data-ttu-id="b21ed-133">此应用配置实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b21ed-133">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="b21ed-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b21ed-134">createdDateTime</span></span>|<span data-ttu-id="b21ed-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b21ed-135">DateTimeOffset</span></span>|<span data-ttu-id="b21ed-136">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b21ed-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="b21ed-137">description</span><span class="sxs-lookup"><span data-stu-id="b21ed-137">description</span></span>|<span data-ttu-id="b21ed-138">字符串</span><span class="sxs-lookup"><span data-stu-id="b21ed-138">String</span></span>|<span data-ttu-id="b21ed-139">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="b21ed-139">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="b21ed-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b21ed-140">lastModifiedDateTime</span></span>|<span data-ttu-id="b21ed-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b21ed-141">DateTimeOffset</span></span>|<span data-ttu-id="b21ed-142">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b21ed-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="b21ed-143">displayName</span><span class="sxs-lookup"><span data-stu-id="b21ed-143">displayName</span></span>|<span data-ttu-id="b21ed-144">字符串</span><span class="sxs-lookup"><span data-stu-id="b21ed-144">String</span></span>|<span data-ttu-id="b21ed-145">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="b21ed-145">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="b21ed-146">version</span><span class="sxs-lookup"><span data-stu-id="b21ed-146">version</span></span>|<span data-ttu-id="b21ed-147">Int32</span><span class="sxs-lookup"><span data-stu-id="b21ed-147">Int32</span></span>|<span data-ttu-id="b21ed-148">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b21ed-148">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b21ed-149">关系</span><span class="sxs-lookup"><span data-stu-id="b21ed-149">Relationships</span></span>
|<span data-ttu-id="b21ed-150">关系</span><span class="sxs-lookup"><span data-stu-id="b21ed-150">Relationship</span></span>|<span data-ttu-id="b21ed-151">类型</span><span class="sxs-lookup"><span data-stu-id="b21ed-151">Type</span></span>|<span data-ttu-id="b21ed-152">Description</span><span class="sxs-lookup"><span data-stu-id="b21ed-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b21ed-153">assignments</span><span class="sxs-lookup"><span data-stu-id="b21ed-153">assignments</span></span>|<span data-ttu-id="b21ed-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b21ed-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b21ed-155">应用配置的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="b21ed-155">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="b21ed-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="b21ed-156">deviceStatuses</span></span>|<span data-ttu-id="b21ed-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b21ed-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="b21ed-158">ManagedDeviceMobileAppConfigurationDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="b21ed-158">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="b21ed-159">userStatuses</span><span class="sxs-lookup"><span data-stu-id="b21ed-159">userStatuses</span></span>|<span data-ttu-id="b21ed-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b21ed-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="b21ed-161">ManagedDeviceMobileAppConfigurationUserStatus 列表</span><span class="sxs-lookup"><span data-stu-id="b21ed-161">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="b21ed-162">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="b21ed-162">deviceStatusSummary</span></span>|[<span data-ttu-id="b21ed-163">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="b21ed-163">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="b21ed-164">应用配置设备状态摘要。</span><span class="sxs-lookup"><span data-stu-id="b21ed-164">App configuration device status summary.</span></span>|
|<span data-ttu-id="b21ed-165">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="b21ed-165">userStatusSummary</span></span>|[<span data-ttu-id="b21ed-166">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="b21ed-166">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="b21ed-167">应用配置用户状态摘要。</span><span class="sxs-lookup"><span data-stu-id="b21ed-167">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b21ed-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b21ed-168">JSON Representation</span></span>
<span data-ttu-id="b21ed-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b21ed-169">Here is a JSON representation of the resource.</span></span>
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




