---
title: iosLobAppProvisioningConfiguration 资源类型
description: 本主题提供由 iOS Lob 应用程序设置配置资源公开的已声明方法、属性和关系的说明。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8bc201ff464fbc7ebbfa9dfaaa8ff8c8adb7d6e6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366047"
---
# <a name="ioslobappprovisioningconfiguration-resource-type"></a><span data-ttu-id="b832a-103">iosLobAppProvisioningConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="b832a-103">iosLobAppProvisioningConfiguration resource type</span></span>

> <span data-ttu-id="b832a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b832a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b832a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b832a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b832a-106">本主题提供由 iOS Lob 应用程序设置配置资源公开的已声明方法、属性和关系的说明。</span><span class="sxs-lookup"><span data-stu-id="b832a-106">This topic provides descriptions of the declared methods, properties and relationships exposed by the iOS Lob App Provisioning Configuration resource.</span></span>

## <a name="methods"></a><span data-ttu-id="b832a-107">方法</span><span class="sxs-lookup"><span data-stu-id="b832a-107">Methods</span></span>
|<span data-ttu-id="b832a-108">方法</span><span class="sxs-lookup"><span data-stu-id="b832a-108">Method</span></span>|<span data-ttu-id="b832a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b832a-109">Return Type</span></span>|<span data-ttu-id="b832a-110">说明</span><span class="sxs-lookup"><span data-stu-id="b832a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b832a-111">列出 iosLobAppProvisioningConfigurations</span><span class="sxs-lookup"><span data-stu-id="b832a-111">List iosLobAppProvisioningConfigurations</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-list.md)|<span data-ttu-id="b832a-112">[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="b832a-112">[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) collection</span></span>|<span data-ttu-id="b832a-113">列出[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b832a-113">List properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="b832a-114">获取 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="b832a-114">Get iosLobAppProvisioningConfiguration</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-get.md)|[<span data-ttu-id="b832a-115">iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="b832a-115">iosLobAppProvisioningConfiguration</span></span>](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|<span data-ttu-id="b832a-116">读取[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b832a-116">Read properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>|
|[<span data-ttu-id="b832a-117">创建 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="b832a-117">Create iosLobAppProvisioningConfiguration</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-create.md)|[<span data-ttu-id="b832a-118">iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="b832a-118">iosLobAppProvisioningConfiguration</span></span>](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|<span data-ttu-id="b832a-119">创建新的[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b832a-119">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>|
|[<span data-ttu-id="b832a-120">删除 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="b832a-120">Delete iosLobAppProvisioningConfiguration</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-delete.md)|<span data-ttu-id="b832a-121">无</span><span class="sxs-lookup"><span data-stu-id="b832a-121">None</span></span>|<span data-ttu-id="b832a-122">删除[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="b832a-122">Deletes a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>|
|[<span data-ttu-id="b832a-123">更新 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="b832a-123">Update iosLobAppProvisioningConfiguration</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-update.md)|[<span data-ttu-id="b832a-124">iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="b832a-124">iosLobAppProvisioningConfiguration</span></span>](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|<span data-ttu-id="b832a-125">更新[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b832a-125">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>|
|[<span data-ttu-id="b832a-126">分配操作</span><span class="sxs-lookup"><span data-stu-id="b832a-126">assign action</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-assign.md)|<span data-ttu-id="b832a-127">无</span><span class="sxs-lookup"><span data-stu-id="b832a-127">None</span></span>|<span data-ttu-id="b832a-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b832a-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b832a-129">属性</span><span class="sxs-lookup"><span data-stu-id="b832a-129">Properties</span></span>
|<span data-ttu-id="b832a-130">属性</span><span class="sxs-lookup"><span data-stu-id="b832a-130">Property</span></span>|<span data-ttu-id="b832a-131">类型</span><span class="sxs-lookup"><span data-stu-id="b832a-131">Type</span></span>|<span data-ttu-id="b832a-132">说明</span><span class="sxs-lookup"><span data-stu-id="b832a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b832a-133">id</span><span class="sxs-lookup"><span data-stu-id="b832a-133">id</span></span>|<span data-ttu-id="b832a-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b832a-134">String</span></span>|<span data-ttu-id="b832a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b832a-135">Key of the entity.</span></span>|
|<span data-ttu-id="b832a-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b832a-136">expirationDateTime</span></span>|<span data-ttu-id="b832a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b832a-137">DateTimeOffset</span></span>|<span data-ttu-id="b832a-138">可选的配置文件到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b832a-138">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="b832a-139">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="b832a-139">payloadFileName</span></span>|<span data-ttu-id="b832a-140">String</span><span class="sxs-lookup"><span data-stu-id="b832a-140">String</span></span>|<span data-ttu-id="b832a-141">有效负载文件名 (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="b832a-141">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="b832a-142">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="b832a-142">\*.xml).</span></span>|
|<span data-ttu-id="b832a-143">payload</span><span class="sxs-lookup"><span data-stu-id="b832a-143">payload</span></span>|<span data-ttu-id="b832a-144">Binary</span><span class="sxs-lookup"><span data-stu-id="b832a-144">Binary</span></span>|<span data-ttu-id="b832a-145">有效负载。</span><span class="sxs-lookup"><span data-stu-id="b832a-145">Payload.</span></span> <span data-ttu-id="b832a-146">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="b832a-146">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="b832a-147">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b832a-147">roleScopeTagIds</span></span>|<span data-ttu-id="b832a-148">String collection</span><span class="sxs-lookup"><span data-stu-id="b832a-148">String collection</span></span>|<span data-ttu-id="b832a-149">此 iOS LOB 应用设置配置实体的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="b832a-149">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="b832a-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b832a-150">createdDateTime</span></span>|<span data-ttu-id="b832a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b832a-151">DateTimeOffset</span></span>|<span data-ttu-id="b832a-152">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b832a-152">DateTime the object was created.</span></span>|
|<span data-ttu-id="b832a-153">说明</span><span class="sxs-lookup"><span data-stu-id="b832a-153">description</span></span>|<span data-ttu-id="b832a-154">String</span><span class="sxs-lookup"><span data-stu-id="b832a-154">String</span></span>|<span data-ttu-id="b832a-155">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="b832a-155">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="b832a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b832a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b832a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b832a-157">DateTimeOffset</span></span>|<span data-ttu-id="b832a-158">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b832a-158">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="b832a-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b832a-159">displayName</span></span>|<span data-ttu-id="b832a-160">String</span><span class="sxs-lookup"><span data-stu-id="b832a-160">String</span></span>|<span data-ttu-id="b832a-161">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="b832a-161">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="b832a-162">version</span><span class="sxs-lookup"><span data-stu-id="b832a-162">version</span></span>|<span data-ttu-id="b832a-163">Int32</span><span class="sxs-lookup"><span data-stu-id="b832a-163">Int32</span></span>|<span data-ttu-id="b832a-164">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b832a-164">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b832a-165">关系</span><span class="sxs-lookup"><span data-stu-id="b832a-165">Relationships</span></span>
|<span data-ttu-id="b832a-166">关系</span><span class="sxs-lookup"><span data-stu-id="b832a-166">Relationship</span></span>|<span data-ttu-id="b832a-167">类型</span><span class="sxs-lookup"><span data-stu-id="b832a-167">Type</span></span>|<span data-ttu-id="b832a-168">说明</span><span class="sxs-lookup"><span data-stu-id="b832a-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b832a-169">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="b832a-169">groupAssignments</span></span>|<span data-ttu-id="b832a-170">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="b832a-170">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="b832a-171">关联的组分配。</span><span class="sxs-lookup"><span data-stu-id="b832a-171">The associated group assignments.</span></span>|
|<span data-ttu-id="b832a-172">assignments</span><span class="sxs-lookup"><span data-stu-id="b832a-172">assignments</span></span>|<span data-ttu-id="b832a-173">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="b832a-173">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b832a-174">IosLobAppProvisioningConfiguration 的关联组分配。</span><span class="sxs-lookup"><span data-stu-id="b832a-174">The associated group assignments for IosLobAppProvisioningConfiguration.</span></span>|
|<span data-ttu-id="b832a-175">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="b832a-175">deviceStatuses</span></span>|<span data-ttu-id="b832a-176">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="b832a-176">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="b832a-177">此移动应用配置的设备安装状态的列表。</span><span class="sxs-lookup"><span data-stu-id="b832a-177">The list of device installation states for this mobile app configuration.</span></span>|
|<span data-ttu-id="b832a-178">userStatuses</span><span class="sxs-lookup"><span data-stu-id="b832a-178">userStatuses</span></span>|<span data-ttu-id="b832a-179">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b832a-179">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="b832a-180">此移动应用配置的用户安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="b832a-180">The list of user installation states for this mobile app configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b832a-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b832a-181">JSON Representation</span></span>
<span data-ttu-id="b832a-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b832a-182">Here is a JSON representation of the resource.</span></span>
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



