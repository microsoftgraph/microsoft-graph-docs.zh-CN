---
title: iosLobAppProvisioningConfiguration 资源类型
description: 本主题提供由 IOS Lob 应用程序设置配置资源公开的已声明方法、属性和关系的说明。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ab481571cce9bd986b31d12c41705f8fb48558b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151035"
---
# <a name="ioslobappprovisioningconfiguration-resource-type"></a><span data-ttu-id="f9498-103">iosLobAppProvisioningConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9498-103">iosLobAppProvisioningConfiguration resource type</span></span>

> <span data-ttu-id="f9498-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f9498-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9498-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f9498-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9498-106">本主题提供由 IOS Lob 应用程序设置配置资源公开的已声明方法、属性和关系的说明。</span><span class="sxs-lookup"><span data-stu-id="f9498-106">This topic provides descriptions of the declared methods, properties and relationships exposed by the IOS Lob App Provisioning Configuration resource.</span></span>

## <a name="methods"></a><span data-ttu-id="f9498-107">方法</span><span class="sxs-lookup"><span data-stu-id="f9498-107">Methods</span></span>
|<span data-ttu-id="f9498-108">方法</span><span class="sxs-lookup"><span data-stu-id="f9498-108">Method</span></span>|<span data-ttu-id="f9498-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f9498-109">Return Type</span></span>|<span data-ttu-id="f9498-110">说明</span><span class="sxs-lookup"><span data-stu-id="f9498-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f9498-111">列出 iosLobAppProvisioningConfigurations</span><span class="sxs-lookup"><span data-stu-id="f9498-111">List iosLobAppProvisioningConfigurations</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-list.md)|<span data-ttu-id="f9498-112">[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="f9498-112">[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) collection</span></span>|<span data-ttu-id="f9498-113">列出[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f9498-113">List properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="f9498-114">获取 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9498-114">Get iosLobAppProvisioningConfiguration</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-get.md)|[<span data-ttu-id="f9498-115">iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9498-115">iosLobAppProvisioningConfiguration</span></span>](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|<span data-ttu-id="f9498-116">读取[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f9498-116">Read properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>|
|[<span data-ttu-id="f9498-117">创建 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9498-117">Create iosLobAppProvisioningConfiguration</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-create.md)|[<span data-ttu-id="f9498-118">iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9498-118">iosLobAppProvisioningConfiguration</span></span>](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|<span data-ttu-id="f9498-119">创建新的[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f9498-119">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>|
|[<span data-ttu-id="f9498-120">删除 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9498-120">Delete iosLobAppProvisioningConfiguration</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-delete.md)|<span data-ttu-id="f9498-121">无</span><span class="sxs-lookup"><span data-stu-id="f9498-121">None</span></span>|<span data-ttu-id="f9498-122">删除[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="f9498-122">Deletes a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>|
|[<span data-ttu-id="f9498-123">更新 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9498-123">Update iosLobAppProvisioningConfiguration</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-update.md)|[<span data-ttu-id="f9498-124">iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9498-124">iosLobAppProvisioningConfiguration</span></span>](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|<span data-ttu-id="f9498-125">更新[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f9498-125">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>|
|[<span data-ttu-id="f9498-126">assign 操作</span><span class="sxs-lookup"><span data-stu-id="f9498-126">assign action</span></span>](../api/intune-apps-ioslobappprovisioningconfiguration-assign.md)|<span data-ttu-id="f9498-127">无</span><span class="sxs-lookup"><span data-stu-id="f9498-127">None</span></span>|<span data-ttu-id="f9498-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f9498-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f9498-129">属性</span><span class="sxs-lookup"><span data-stu-id="f9498-129">Properties</span></span>
|<span data-ttu-id="f9498-130">属性</span><span class="sxs-lookup"><span data-stu-id="f9498-130">Property</span></span>|<span data-ttu-id="f9498-131">类型</span><span class="sxs-lookup"><span data-stu-id="f9498-131">Type</span></span>|<span data-ttu-id="f9498-132">说明</span><span class="sxs-lookup"><span data-stu-id="f9498-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9498-133">id</span><span class="sxs-lookup"><span data-stu-id="f9498-133">id</span></span>|<span data-ttu-id="f9498-134">字串符号</span><span class="sxs-lookup"><span data-stu-id="f9498-134">String</span></span>|<span data-ttu-id="f9498-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f9498-135">Key of the entity.</span></span>|
|<span data-ttu-id="f9498-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f9498-136">expirationDateTime</span></span>|<span data-ttu-id="f9498-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9498-137">DateTimeOffset</span></span>|<span data-ttu-id="f9498-138">可选的配置文件到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f9498-138">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="f9498-139">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="f9498-139">payloadFileName</span></span>|<span data-ttu-id="f9498-140">String</span><span class="sxs-lookup"><span data-stu-id="f9498-140">String</span></span>|<span data-ttu-id="f9498-141">有效负载文件名 (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="f9498-141">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="f9498-142">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="f9498-142">\*.xml).</span></span>|
|<span data-ttu-id="f9498-143">payload</span><span class="sxs-lookup"><span data-stu-id="f9498-143">payload</span></span>|<span data-ttu-id="f9498-144">Binary</span><span class="sxs-lookup"><span data-stu-id="f9498-144">Binary</span></span>|<span data-ttu-id="f9498-145">有效负载。</span><span class="sxs-lookup"><span data-stu-id="f9498-145">Payload.</span></span> <span data-ttu-id="f9498-146">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="f9498-146">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="f9498-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9498-147">createdDateTime</span></span>|<span data-ttu-id="f9498-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9498-148">DateTimeOffset</span></span>|<span data-ttu-id="f9498-149">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f9498-149">DateTime the object was created.</span></span>|
|<span data-ttu-id="f9498-150">description</span><span class="sxs-lookup"><span data-stu-id="f9498-150">description</span></span>|<span data-ttu-id="f9498-151">字符串</span><span class="sxs-lookup"><span data-stu-id="f9498-151">String</span></span>|<span data-ttu-id="f9498-152">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="f9498-152">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="f9498-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9498-153">lastModifiedDateTime</span></span>|<span data-ttu-id="f9498-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9498-154">DateTimeOffset</span></span>|<span data-ttu-id="f9498-155">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f9498-155">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="f9498-156">displayName</span><span class="sxs-lookup"><span data-stu-id="f9498-156">displayName</span></span>|<span data-ttu-id="f9498-157">String</span><span class="sxs-lookup"><span data-stu-id="f9498-157">String</span></span>|<span data-ttu-id="f9498-158">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="f9498-158">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="f9498-159">version</span><span class="sxs-lookup"><span data-stu-id="f9498-159">version</span></span>|<span data-ttu-id="f9498-160">Int32</span><span class="sxs-lookup"><span data-stu-id="f9498-160">Int32</span></span>|<span data-ttu-id="f9498-161">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f9498-161">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9498-162">关系</span><span class="sxs-lookup"><span data-stu-id="f9498-162">Relationships</span></span>
|<span data-ttu-id="f9498-163">关系</span><span class="sxs-lookup"><span data-stu-id="f9498-163">Relationship</span></span>|<span data-ttu-id="f9498-164">类型</span><span class="sxs-lookup"><span data-stu-id="f9498-164">Type</span></span>|<span data-ttu-id="f9498-165">说明</span><span class="sxs-lookup"><span data-stu-id="f9498-165">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9498-166">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="f9498-166">groupAssignments</span></span>|<span data-ttu-id="f9498-167">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="f9498-167">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="f9498-168">关联的组分配。</span><span class="sxs-lookup"><span data-stu-id="f9498-168">The associated group assignments.</span></span>|
|<span data-ttu-id="f9498-169">assignments</span><span class="sxs-lookup"><span data-stu-id="f9498-169">assignments</span></span>|<span data-ttu-id="f9498-170">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="f9498-170">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f9498-171">IosLobAppProvisioningConfiguration 的关联组分配。</span><span class="sxs-lookup"><span data-stu-id="f9498-171">The associated group assignments for IosLobAppProvisioningConfiguration.</span></span>|
|<span data-ttu-id="f9498-172">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="f9498-172">deviceStatuses</span></span>|<span data-ttu-id="f9498-173">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="f9498-173">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="f9498-174">此移动应用配置的设备安装状态的列表。</span><span class="sxs-lookup"><span data-stu-id="f9498-174">The list of device installation states for this mobile app configuration.</span></span>|
|<span data-ttu-id="f9498-175">userStatuses</span><span class="sxs-lookup"><span data-stu-id="f9498-175">userStatuses</span></span>|<span data-ttu-id="f9498-176">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f9498-176">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="f9498-177">此移动应用配置的用户安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="f9498-177">The list of user installation states for this mobile app configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9498-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9498-178">JSON Representation</span></span>
<span data-ttu-id="f9498-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9498-179">Here is a JSON representation of the resource.</span></span>
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
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```




