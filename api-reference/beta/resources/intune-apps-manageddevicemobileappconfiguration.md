---
title: managedDeviceMobileAppConfiguration 资源类型
description: 已注册设备移动应用配置的抽象类
ms.openlocfilehash: c829e720e8d998428e778e5b7bf20e5fe465dfd6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041366"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="be730-103">managedDeviceMobileAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="be730-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="be730-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="be730-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be730-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="be730-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be730-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="be730-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be730-107">已注册设备移动应用配置的抽象类</span><span class="sxs-lookup"><span data-stu-id="be730-107">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="be730-108">方法</span><span class="sxs-lookup"><span data-stu-id="be730-108">Methods</span></span>
|<span data-ttu-id="be730-109">方法</span><span class="sxs-lookup"><span data-stu-id="be730-109">Method</span></span>|<span data-ttu-id="be730-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="be730-110">Return Type</span></span>|<span data-ttu-id="be730-111">说明</span><span class="sxs-lookup"><span data-stu-id="be730-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="be730-112">List managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="be730-112">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="be730-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be730-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="be730-114">列出 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="be730-114">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="be730-115">Get managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="be730-115">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="be730-116">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="be730-116">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="be730-117">读取 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="be730-117">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="be730-118">assign 操作</span><span class="sxs-lookup"><span data-stu-id="be730-118">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="be730-119">无</span><span class="sxs-lookup"><span data-stu-id="be730-119">None</span></span>|<span data-ttu-id="be730-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="be730-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="be730-121">属性</span><span class="sxs-lookup"><span data-stu-id="be730-121">Properties</span></span>
|<span data-ttu-id="be730-122">属性</span><span class="sxs-lookup"><span data-stu-id="be730-122">Property</span></span>|<span data-ttu-id="be730-123">类型</span><span class="sxs-lookup"><span data-stu-id="be730-123">Type</span></span>|<span data-ttu-id="be730-124">说明</span><span class="sxs-lookup"><span data-stu-id="be730-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be730-125">id</span><span class="sxs-lookup"><span data-stu-id="be730-125">id</span></span>|<span data-ttu-id="be730-126">String</span><span class="sxs-lookup"><span data-stu-id="be730-126">String</span></span>|<span data-ttu-id="be730-127">实体的键。</span><span class="sxs-lookup"><span data-stu-id="be730-127">Key of the entity.</span></span>|
|<span data-ttu-id="be730-128">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="be730-128">targetedMobileApps</span></span>|<span data-ttu-id="be730-129">String 集合</span><span class="sxs-lookup"><span data-stu-id="be730-129">String collection</span></span>|<span data-ttu-id="be730-130">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="be730-130">the associated app.</span></span>|
|<span data-ttu-id="be730-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="be730-131">roleScopeTagIds</span></span>|<span data-ttu-id="be730-132">String 集合</span><span class="sxs-lookup"><span data-stu-id="be730-132">String collection</span></span>|<span data-ttu-id="be730-133">此应用程序配置实体范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="be730-133">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="be730-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be730-134">createdDateTime</span></span>|<span data-ttu-id="be730-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be730-135">DateTimeOffset</span></span>|<span data-ttu-id="be730-136">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="be730-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="be730-137">description</span><span class="sxs-lookup"><span data-stu-id="be730-137">description</span></span>|<span data-ttu-id="be730-138">String</span><span class="sxs-lookup"><span data-stu-id="be730-138">String</span></span>|<span data-ttu-id="be730-139">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="be730-139">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="be730-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be730-140">lastModifiedDateTime</span></span>|<span data-ttu-id="be730-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be730-141">DateTimeOffset</span></span>|<span data-ttu-id="be730-142">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="be730-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="be730-143">displayName</span><span class="sxs-lookup"><span data-stu-id="be730-143">displayName</span></span>|<span data-ttu-id="be730-144">String</span><span class="sxs-lookup"><span data-stu-id="be730-144">String</span></span>|<span data-ttu-id="be730-145">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="be730-145">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="be730-146">version</span><span class="sxs-lookup"><span data-stu-id="be730-146">version</span></span>|<span data-ttu-id="be730-147">Int32</span><span class="sxs-lookup"><span data-stu-id="be730-147">Int32</span></span>|<span data-ttu-id="be730-148">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="be730-148">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be730-149">关系</span><span class="sxs-lookup"><span data-stu-id="be730-149">Relationships</span></span>
|<span data-ttu-id="be730-150">关系</span><span class="sxs-lookup"><span data-stu-id="be730-150">Relationship</span></span>|<span data-ttu-id="be730-151">类型</span><span class="sxs-lookup"><span data-stu-id="be730-151">Type</span></span>|<span data-ttu-id="be730-152">说明</span><span class="sxs-lookup"><span data-stu-id="be730-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be730-153">assignments</span><span class="sxs-lookup"><span data-stu-id="be730-153">assignments</span></span>|<span data-ttu-id="be730-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be730-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="be730-155">应用配置的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="be730-155">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="be730-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="be730-156">deviceStatuses</span></span>|<span data-ttu-id="be730-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="be730-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="be730-158">ManagedDeviceMobileAppConfigurationDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="be730-158">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="be730-159">userStatuses</span><span class="sxs-lookup"><span data-stu-id="be730-159">userStatuses</span></span>|<span data-ttu-id="be730-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be730-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="be730-161">ManagedDeviceMobileAppConfigurationUserStatus 列表</span><span class="sxs-lookup"><span data-stu-id="be730-161">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="be730-162">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="be730-162">deviceStatusSummary</span></span>|[<span data-ttu-id="be730-163">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="be730-163">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="be730-164">应用配置设备状态摘要。</span><span class="sxs-lookup"><span data-stu-id="be730-164">App configuration device status summary.</span></span>|
|<span data-ttu-id="be730-165">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="be730-165">userStatusSummary</span></span>|[<span data-ttu-id="be730-166">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="be730-166">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="be730-167">应用配置用户状态摘要。</span><span class="sxs-lookup"><span data-stu-id="be730-167">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be730-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be730-168">JSON Representation</span></span>
<span data-ttu-id="be730-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be730-169">Here is a JSON representation of the resource.</span></span>
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





