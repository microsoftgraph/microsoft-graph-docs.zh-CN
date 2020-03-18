---
title: iosLobAppProvisioningConfiguration 资源类型
description: 本主题提供由 iOS Lob 应用程序设置配置资源公开的已声明方法、属性和关系的说明。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cdf220c0d2399eb3a7876fcab438c96e869cc21d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769988"
---
# <a name="ioslobappprovisioningconfiguration-resource-type"></a><span data-ttu-id="2b1ee-103">iosLobAppProvisioningConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b1ee-103">iosLobAppProvisioningConfiguration resource type</span></span>

> <span data-ttu-id="2b1ee-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b1ee-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b1ee-106">本主题提供由 iOS Lob 应用程序设置配置资源公开的已声明方法、属性和关系的说明。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-106">This topic provides descriptions of the declared methods, properties and relationships exposed by the iOS Lob App Provisioning Configuration resource.</span></span>

## <a name="methods"></a><span data-ttu-id="2b1ee-107">方法</span><span class="sxs-lookup"><span data-stu-id="2b1ee-107">Methods</span></span>
|<span data-ttu-id="2b1ee-108">方法</span><span class="sxs-lookup"><span data-stu-id="2b1ee-108">Method</span></span>|<span data-ttu-id="2b1ee-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2b1ee-109">Return Type</span></span>|<span data-ttu-id="2b1ee-110">说明</span><span class="sxs-lookup"><span data-stu-id="2b1ee-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2b1ee-111">列出 iosLobAppProvisioningConfigurations</span><span class="sxs-lookup"><span data-stu-id="2b1ee-111">List iosLobAppProvisioningConfigurations</span></span>](../api/intune-shared-ioslobappprovisioningconfiguration-list.md)|<span data-ttu-id="2b1ee-112">[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b1ee-112">[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) collection</span></span>|<span data-ttu-id="2b1ee-113">列出[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-113">List properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="2b1ee-114">获取 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b1ee-114">Get iosLobAppProvisioningConfiguration</span></span>](../api/intune-shared-ioslobappprovisioningconfiguration-get.md)|[<span data-ttu-id="2b1ee-115">iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b1ee-115">iosLobAppProvisioningConfiguration</span></span>](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|<span data-ttu-id="2b1ee-116">读取[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-116">Read properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>|
|[<span data-ttu-id="2b1ee-117">创建 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b1ee-117">Create iosLobAppProvisioningConfiguration</span></span>](../api/intune-shared-ioslobappprovisioningconfiguration-create.md)|[<span data-ttu-id="2b1ee-118">iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b1ee-118">iosLobAppProvisioningConfiguration</span></span>](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|<span data-ttu-id="2b1ee-119">创建新的[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-119">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>|
|[<span data-ttu-id="2b1ee-120">删除 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b1ee-120">Delete iosLobAppProvisioningConfiguration</span></span>](../api/intune-shared-ioslobappprovisioningconfiguration-delete.md)|<span data-ttu-id="2b1ee-121">None</span><span class="sxs-lookup"><span data-stu-id="2b1ee-121">None</span></span>|<span data-ttu-id="2b1ee-122">删除[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-122">Deletes a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span></span>|
|[<span data-ttu-id="2b1ee-123">更新 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b1ee-123">Update iosLobAppProvisioningConfiguration</span></span>](../api/intune-shared-ioslobappprovisioningconfiguration-update.md)|[<span data-ttu-id="2b1ee-124">iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b1ee-124">iosLobAppProvisioningConfiguration</span></span>](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|<span data-ttu-id="2b1ee-125">更新[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-125">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>|
|<span data-ttu-id="2b1ee-126">**应用**</span><span class="sxs-lookup"><span data-stu-id="2b1ee-126">**Apps**</span></span>|
|[<span data-ttu-id="2b1ee-127">分配操作</span><span class="sxs-lookup"><span data-stu-id="2b1ee-127">assign action</span></span>](../api/intune-shared-ioslobappprovisioningconfiguration-assign.md)|<span data-ttu-id="2b1ee-128">无</span><span class="sxs-lookup"><span data-stu-id="2b1ee-128">None</span></span>|<span data-ttu-id="2b1ee-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2b1ee-129">Not yet documented</span></span>|
|<span data-ttu-id="2b1ee-130">**策略集**</span><span class="sxs-lookup"><span data-stu-id="2b1ee-130">**Policy Set**</span></span>|
|[<span data-ttu-id="2b1ee-131">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="2b1ee-131">hasPayloadLinks action</span></span>](../api/intune-shared-ioslobappprovisioningconfiguration-haspayloadlinks.md)|<span data-ttu-id="2b1ee-132">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b1ee-132">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="2b1ee-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2b1ee-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2b1ee-134">属性</span><span class="sxs-lookup"><span data-stu-id="2b1ee-134">Properties</span></span>
|<span data-ttu-id="2b1ee-135">属性</span><span class="sxs-lookup"><span data-stu-id="2b1ee-135">Property</span></span>|<span data-ttu-id="2b1ee-136">类型</span><span class="sxs-lookup"><span data-stu-id="2b1ee-136">Type</span></span>|<span data-ttu-id="2b1ee-137">说明</span><span class="sxs-lookup"><span data-stu-id="2b1ee-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b1ee-138">id</span><span class="sxs-lookup"><span data-stu-id="2b1ee-138">id</span></span>|<span data-ttu-id="2b1ee-139">字符串</span><span class="sxs-lookup"><span data-stu-id="2b1ee-139">String</span></span>|<span data-ttu-id="2b1ee-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-140">Key of the entity.</span></span>|
|<span data-ttu-id="2b1ee-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2b1ee-141">expirationDateTime</span></span>|<span data-ttu-id="2b1ee-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b1ee-142">DateTimeOffset</span></span>|<span data-ttu-id="2b1ee-143">可选的配置文件到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-143">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="2b1ee-144">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="2b1ee-144">payloadFileName</span></span>|<span data-ttu-id="2b1ee-145">String</span><span class="sxs-lookup"><span data-stu-id="2b1ee-145">String</span></span>|<span data-ttu-id="2b1ee-146">有效负载文件名（\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="2b1ee-146">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="2b1ee-147">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-147">\*.xml).</span></span>|
|<span data-ttu-id="2b1ee-148">payload</span><span class="sxs-lookup"><span data-stu-id="2b1ee-148">payload</span></span>|<span data-ttu-id="2b1ee-149">Binary</span><span class="sxs-lookup"><span data-stu-id="2b1ee-149">Binary</span></span>|<span data-ttu-id="2b1ee-150">有效负载。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-150">Payload.</span></span> <span data-ttu-id="2b1ee-151">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="2b1ee-151">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="2b1ee-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2b1ee-152">roleScopeTagIds</span></span>|<span data-ttu-id="2b1ee-153">String collection</span><span class="sxs-lookup"><span data-stu-id="2b1ee-153">String collection</span></span>|<span data-ttu-id="2b1ee-154">此 iOS LOB 应用设置配置实体的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-154">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="2b1ee-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b1ee-155">createdDateTime</span></span>|<span data-ttu-id="2b1ee-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b1ee-156">DateTimeOffset</span></span>|<span data-ttu-id="2b1ee-157">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-157">DateTime the object was created.</span></span>|
|<span data-ttu-id="2b1ee-158">说明</span><span class="sxs-lookup"><span data-stu-id="2b1ee-158">description</span></span>|<span data-ttu-id="2b1ee-159">String</span><span class="sxs-lookup"><span data-stu-id="2b1ee-159">String</span></span>|<span data-ttu-id="2b1ee-160">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-160">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="2b1ee-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b1ee-161">lastModifiedDateTime</span></span>|<span data-ttu-id="2b1ee-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b1ee-162">DateTimeOffset</span></span>|<span data-ttu-id="2b1ee-163">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-163">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="2b1ee-164">displayName</span><span class="sxs-lookup"><span data-stu-id="2b1ee-164">displayName</span></span>|<span data-ttu-id="2b1ee-165">String</span><span class="sxs-lookup"><span data-stu-id="2b1ee-165">String</span></span>|<span data-ttu-id="2b1ee-166">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-166">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="2b1ee-167">version</span><span class="sxs-lookup"><span data-stu-id="2b1ee-167">version</span></span>|<span data-ttu-id="2b1ee-168">Int32</span><span class="sxs-lookup"><span data-stu-id="2b1ee-168">Int32</span></span>|<span data-ttu-id="2b1ee-169">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-169">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b1ee-170">关系</span><span class="sxs-lookup"><span data-stu-id="2b1ee-170">Relationships</span></span>
|<span data-ttu-id="2b1ee-171">关系</span><span class="sxs-lookup"><span data-stu-id="2b1ee-171">Relationship</span></span>|<span data-ttu-id="2b1ee-172">类型</span><span class="sxs-lookup"><span data-stu-id="2b1ee-172">Type</span></span>|<span data-ttu-id="2b1ee-173">说明</span><span class="sxs-lookup"><span data-stu-id="2b1ee-173">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b1ee-174">**应用**</span><span class="sxs-lookup"><span data-stu-id="2b1ee-174">**Apps**</span></span>|
|<span data-ttu-id="2b1ee-175">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="2b1ee-175">groupAssignments</span></span>|<span data-ttu-id="2b1ee-176">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b1ee-176">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="2b1ee-177">关联的组分配。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-177">The associated group assignments.</span></span>|
|<span data-ttu-id="2b1ee-178">assignments</span><span class="sxs-lookup"><span data-stu-id="2b1ee-178">assignments</span></span>|<span data-ttu-id="2b1ee-179">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b1ee-179">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2b1ee-180">IosLobAppProvisioningConfiguration 的关联组分配。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-180">The associated group assignments for IosLobAppProvisioningConfiguration.</span></span>|
|<span data-ttu-id="2b1ee-181">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="2b1ee-181">deviceStatuses</span></span>|<span data-ttu-id="2b1ee-182">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b1ee-182">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="2b1ee-183">此移动应用配置的设备安装状态的列表。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-183">The list of device installation states for this mobile app configuration.</span></span>|
|<span data-ttu-id="2b1ee-184">userStatuses</span><span class="sxs-lookup"><span data-stu-id="2b1ee-184">userStatuses</span></span>|<span data-ttu-id="2b1ee-185">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2b1ee-185">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="2b1ee-186">此移动应用配置的用户安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-186">The list of user installation states for this mobile app configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b1ee-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b1ee-187">JSON Representation</span></span>
<span data-ttu-id="2b1ee-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b1ee-188">Here is a JSON representation of the resource.</span></span>
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



