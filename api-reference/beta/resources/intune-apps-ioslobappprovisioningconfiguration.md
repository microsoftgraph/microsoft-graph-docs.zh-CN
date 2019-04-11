---
title: iosLobAppProvisioningConfiguration 资源类型
description: 本主题提供由 iOS Lob 应用程序设置配置资源公开的已声明方法、属性和关系的说明。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a5a85b0b5467835a1ecb3d81997e0300ab08eee
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796239"
---
# <a name="ioslobappprovisioningconfiguration-resource-type"></a><span data-ttu-id="15f56-103">iosLobAppProvisioningConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="15f56-103">iosLobAppProvisioningConfiguration resource type</span></span>

> <span data-ttu-id="15f56-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="15f56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15f56-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="15f56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15f56-106">本主题提供由 iOS Lob 应用程序设置配置资源公开的已声明方法、属性和关系的说明。</span><span class="sxs-lookup"><span data-stu-id="15f56-106">This topic provides descriptions of the declared methods, properties and relationships exposed by the iOS Lob App Provisioning Configuration resource.</span></span>

## <a name="methods"></a><span data-ttu-id="15f56-107">方法</span><span class="sxs-lookup"><span data-stu-id="15f56-107">Methods</span></span>
|<span data-ttu-id="15f56-108">方法</span><span class="sxs-lookup"><span data-stu-id="15f56-108">Method</span></span>|<span data-ttu-id="15f56-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="15f56-109">Return Type</span></span>|<span data-ttu-id="15f56-110">说明</span><span class="sxs-lookup"><span data-stu-id="15f56-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="15f56-111">列出 iosLobAppProvisioningConfigurations</span><span class="sxs-lookup"><span data-stu-id="15f56-111">List iosLobAppProvisioningConfigurations</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-list.md)|<span data-ttu-id="15f56-112">[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="15f56-112">[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) collection</span></span>|<span data-ttu-id="15f56-113">列出[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="15f56-113">List properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="15f56-114">获取 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="15f56-114">Get iosLobAppProvisioningConfiguration</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-get.md)|[<span data-ttu-id="15f56-115">iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="15f56-115">iosLobAppProvisioningConfiguration</span></span>](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|<span data-ttu-id="15f56-116">读取[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="15f56-116">Read properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>|
|[<span data-ttu-id="15f56-117">创建 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="15f56-117">Create iosLobAppProvisioningConfiguration</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-create.md)|[<span data-ttu-id="15f56-118">iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="15f56-118">iosLobAppProvisioningConfiguration</span></span>](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|<span data-ttu-id="15f56-119">创建新的[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="15f56-119">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>|
|[<span data-ttu-id="15f56-120">删除 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="15f56-120">Delete iosLobAppProvisioningConfiguration</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-delete.md)|<span data-ttu-id="15f56-121">无</span><span class="sxs-lookup"><span data-stu-id="15f56-121">None</span></span>|<span data-ttu-id="15f56-122">删除[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="15f56-122">Deletes a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>|
|[<span data-ttu-id="15f56-123">更新 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="15f56-123">Update iosLobAppProvisioningConfiguration</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-update.md)|[<span data-ttu-id="15f56-124">iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="15f56-124">iosLobAppProvisioningConfiguration</span></span>](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|<span data-ttu-id="15f56-125">更新[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="15f56-125">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>|
|[<span data-ttu-id="15f56-126">分配操作</span><span class="sxs-lookup"><span data-stu-id="15f56-126">assign action</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-assign.md)|<span data-ttu-id="15f56-127">无</span><span class="sxs-lookup"><span data-stu-id="15f56-127">None</span></span>|<span data-ttu-id="15f56-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="15f56-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="15f56-129">属性</span><span class="sxs-lookup"><span data-stu-id="15f56-129">Properties</span></span>
|<span data-ttu-id="15f56-130">属性</span><span class="sxs-lookup"><span data-stu-id="15f56-130">Property</span></span>|<span data-ttu-id="15f56-131">类型</span><span class="sxs-lookup"><span data-stu-id="15f56-131">Type</span></span>|<span data-ttu-id="15f56-132">说明</span><span class="sxs-lookup"><span data-stu-id="15f56-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15f56-133">id</span><span class="sxs-lookup"><span data-stu-id="15f56-133">id</span></span>|<span data-ttu-id="15f56-134">String</span><span class="sxs-lookup"><span data-stu-id="15f56-134">String</span></span>|<span data-ttu-id="15f56-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="15f56-135">Key of the entity.</span></span>|
|<span data-ttu-id="15f56-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="15f56-136">expirationDateTime</span></span>|<span data-ttu-id="15f56-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15f56-137">DateTimeOffset</span></span>|<span data-ttu-id="15f56-138">可选的配置文件到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="15f56-138">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="15f56-139">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="15f56-139">payloadFileName</span></span>|<span data-ttu-id="15f56-140">String</span><span class="sxs-lookup"><span data-stu-id="15f56-140">String</span></span>|<span data-ttu-id="15f56-141">有效负载文件名 (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="15f56-141">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="15f56-142">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="15f56-142">\*.xml).</span></span>|
|<span data-ttu-id="15f56-143">payload</span><span class="sxs-lookup"><span data-stu-id="15f56-143">payload</span></span>|<span data-ttu-id="15f56-144">Binary</span><span class="sxs-lookup"><span data-stu-id="15f56-144">Binary</span></span>|<span data-ttu-id="15f56-145">有效负载。</span><span class="sxs-lookup"><span data-stu-id="15f56-145">Payload.</span></span> <span data-ttu-id="15f56-146">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="15f56-146">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="15f56-147">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="15f56-147">roleScopeTagIds</span></span>|<span data-ttu-id="15f56-148">String 集合</span><span class="sxs-lookup"><span data-stu-id="15f56-148">String collection</span></span>|<span data-ttu-id="15f56-149">此 iOS LOB 应用设置配置实体的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="15f56-149">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="15f56-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15f56-150">createdDateTime</span></span>|<span data-ttu-id="15f56-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15f56-151">DateTimeOffset</span></span>|<span data-ttu-id="15f56-152">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="15f56-152">DateTime the object was created.</span></span>|
|<span data-ttu-id="15f56-153">description</span><span class="sxs-lookup"><span data-stu-id="15f56-153">description</span></span>|<span data-ttu-id="15f56-154">String</span><span class="sxs-lookup"><span data-stu-id="15f56-154">String</span></span>|<span data-ttu-id="15f56-155">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="15f56-155">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="15f56-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15f56-156">lastModifiedDateTime</span></span>|<span data-ttu-id="15f56-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15f56-157">DateTimeOffset</span></span>|<span data-ttu-id="15f56-158">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="15f56-158">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="15f56-159">displayName</span><span class="sxs-lookup"><span data-stu-id="15f56-159">displayName</span></span>|<span data-ttu-id="15f56-160">String</span><span class="sxs-lookup"><span data-stu-id="15f56-160">String</span></span>|<span data-ttu-id="15f56-161">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="15f56-161">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="15f56-162">version</span><span class="sxs-lookup"><span data-stu-id="15f56-162">version</span></span>|<span data-ttu-id="15f56-163">Int32</span><span class="sxs-lookup"><span data-stu-id="15f56-163">Int32</span></span>|<span data-ttu-id="15f56-164">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="15f56-164">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15f56-165">关系</span><span class="sxs-lookup"><span data-stu-id="15f56-165">Relationships</span></span>
|<span data-ttu-id="15f56-166">关系</span><span class="sxs-lookup"><span data-stu-id="15f56-166">Relationship</span></span>|<span data-ttu-id="15f56-167">类型</span><span class="sxs-lookup"><span data-stu-id="15f56-167">Type</span></span>|<span data-ttu-id="15f56-168">说明</span><span class="sxs-lookup"><span data-stu-id="15f56-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15f56-169">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="15f56-169">groupAssignments</span></span>|<span data-ttu-id="15f56-170">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="15f56-170">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="15f56-171">关联的组分配。</span><span class="sxs-lookup"><span data-stu-id="15f56-171">The associated group assignments.</span></span>|
|<span data-ttu-id="15f56-172">assignments</span><span class="sxs-lookup"><span data-stu-id="15f56-172">assignments</span></span>|<span data-ttu-id="15f56-173">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="15f56-173">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="15f56-174">IosLobAppProvisioningConfiguration 的关联组分配。</span><span class="sxs-lookup"><span data-stu-id="15f56-174">The associated group assignments for IosLobAppProvisioningConfiguration.</span></span>|
|<span data-ttu-id="15f56-175">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="15f56-175">deviceStatuses</span></span>|<span data-ttu-id="15f56-176">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="15f56-176">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="15f56-177">此移动应用配置的设备安装状态的列表。</span><span class="sxs-lookup"><span data-stu-id="15f56-177">The list of device installation states for this mobile app configuration.</span></span>|
|<span data-ttu-id="15f56-178">userStatuses</span><span class="sxs-lookup"><span data-stu-id="15f56-178">userStatuses</span></span>|<span data-ttu-id="15f56-179">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="15f56-179">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="15f56-180">此移动应用配置的用户安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="15f56-180">The list of user installation states for this mobile app configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="15f56-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15f56-181">JSON Representation</span></span>
<span data-ttu-id="15f56-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15f56-182">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosLobAppProvisioningConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "String (identifier)",
  "expirationDateTime": "String (timestamp)",
  "payloadFileName": "String",
  "payload": "binary",
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





