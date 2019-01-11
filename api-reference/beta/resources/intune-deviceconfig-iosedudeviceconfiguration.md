---
title: iosEduDeviceConfiguration 资源类型
description: iOS 教育设备配置
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 711c3acf8a462d57b5e5abfa2d453862a1145688
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854045"
---
# <a name="iosedudeviceconfiguration-resource-type"></a><span data-ttu-id="1a7a8-103">iosEduDeviceConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a7a8-103">iosEduDeviceConfiguration resource type</span></span>

> <span data-ttu-id="1a7a8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a7a8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a7a8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a7a8-107">iOS 教育设备配置</span><span class="sxs-lookup"><span data-stu-id="1a7a8-107">iOS Education device configuration</span></span>

<span data-ttu-id="1a7a8-108">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a7a8-108">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1a7a8-109">方法</span><span class="sxs-lookup"><span data-stu-id="1a7a8-109">Methods</span></span>
|<span data-ttu-id="1a7a8-110">方法</span><span class="sxs-lookup"><span data-stu-id="1a7a8-110">Method</span></span>|<span data-ttu-id="1a7a8-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="1a7a8-111">Return Type</span></span>|<span data-ttu-id="1a7a8-112">说明</span><span class="sxs-lookup"><span data-stu-id="1a7a8-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1a7a8-113">列表 iosEduDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="1a7a8-113">List iosEduDeviceConfigurations</span></span>](../api/intune-deviceconfig-iosedudeviceconfiguration-list.md)|<span data-ttu-id="1a7a8-114">[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="1a7a8-114">[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) collection</span></span>|<span data-ttu-id="1a7a8-115">列出属性和[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-115">List properties and relationships of the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="1a7a8-116">获取 iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a7a8-116">Get iosEduDeviceConfiguration</span></span>](../api/intune-deviceconfig-iosedudeviceconfiguration-get.md)|[<span data-ttu-id="1a7a8-117">iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a7a8-117">iosEduDeviceConfiguration</span></span>](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)|<span data-ttu-id="1a7a8-118">读取属性和[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-118">Read properties and relationships of the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="1a7a8-119">创建 iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a7a8-119">Create iosEduDeviceConfiguration</span></span>](../api/intune-deviceconfig-iosedudeviceconfiguration-create.md)|[<span data-ttu-id="1a7a8-120">iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a7a8-120">iosEduDeviceConfiguration</span></span>](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)|<span data-ttu-id="1a7a8-121">创建新的[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-121">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="1a7a8-122">删除 iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a7a8-122">Delete iosEduDeviceConfiguration</span></span>](../api/intune-deviceconfig-iosedudeviceconfiguration-delete.md)|<span data-ttu-id="1a7a8-123">无</span><span class="sxs-lookup"><span data-stu-id="1a7a8-123">None</span></span>|<span data-ttu-id="1a7a8-124">删除[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-124">Deletes a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span></span>|
|[<span data-ttu-id="1a7a8-125">更新 iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a7a8-125">Update iosEduDeviceConfiguration</span></span>](../api/intune-deviceconfig-iosedudeviceconfiguration-update.md)|[<span data-ttu-id="1a7a8-126">iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a7a8-126">iosEduDeviceConfiguration</span></span>](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)|<span data-ttu-id="1a7a8-127">更新[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-127">Update the properties of a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1a7a8-128">属性</span><span class="sxs-lookup"><span data-stu-id="1a7a8-128">Properties</span></span>
|<span data-ttu-id="1a7a8-129">属性</span><span class="sxs-lookup"><span data-stu-id="1a7a8-129">Property</span></span>|<span data-ttu-id="1a7a8-130">类型</span><span class="sxs-lookup"><span data-stu-id="1a7a8-130">Type</span></span>|<span data-ttu-id="1a7a8-131">说明</span><span class="sxs-lookup"><span data-stu-id="1a7a8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a7a8-132">id</span><span class="sxs-lookup"><span data-stu-id="1a7a8-132">id</span></span>|<span data-ttu-id="1a7a8-133">String</span><span class="sxs-lookup"><span data-stu-id="1a7a8-133">String</span></span>|<span data-ttu-id="1a7a8-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-134">Key of the entity.</span></span> <span data-ttu-id="1a7a8-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a7a8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a7a8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a7a8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1a7a8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a7a8-137">DateTimeOffset</span></span>|<span data-ttu-id="1a7a8-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1a7a8-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a7a8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a7a8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1a7a8-140">roleScopeTagIds</span></span>|<span data-ttu-id="1a7a8-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="1a7a8-141">String collection</span></span>|<span data-ttu-id="1a7a8-142">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1a7a8-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a7a8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a7a8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1a7a8-144">supportsScopeTags</span></span>|<span data-ttu-id="1a7a8-145">布尔</span><span class="sxs-lookup"><span data-stu-id="1a7a8-145">Boolean</span></span>|<span data-ttu-id="1a7a8-146">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1a7a8-147">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1a7a8-148">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1a7a8-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-149">This property is read-only.</span></span> <span data-ttu-id="1a7a8-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a7a8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a7a8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a7a8-151">createdDateTime</span></span>|<span data-ttu-id="1a7a8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a7a8-152">DateTimeOffset</span></span>|<span data-ttu-id="1a7a8-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-153">DateTime the object was created.</span></span> <span data-ttu-id="1a7a8-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a7a8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a7a8-155">description</span><span class="sxs-lookup"><span data-stu-id="1a7a8-155">description</span></span>|<span data-ttu-id="1a7a8-156">String</span><span class="sxs-lookup"><span data-stu-id="1a7a8-156">String</span></span>|<span data-ttu-id="1a7a8-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1a7a8-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a7a8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a7a8-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1a7a8-159">displayName</span></span>|<span data-ttu-id="1a7a8-160">String</span><span class="sxs-lookup"><span data-stu-id="1a7a8-160">String</span></span>|<span data-ttu-id="1a7a8-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1a7a8-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a7a8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a7a8-163">version</span><span class="sxs-lookup"><span data-stu-id="1a7a8-163">version</span></span>|<span data-ttu-id="1a7a8-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1a7a8-164">Int32</span></span>|<span data-ttu-id="1a7a8-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-165">Version of the device configuration.</span></span> <span data-ttu-id="1a7a8-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a7a8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a7a8-167">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="1a7a8-167">teacherCertificateSettings</span></span>|[<span data-ttu-id="1a7a8-168">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="1a7a8-168">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="1a7a8-169">教师的受信任的根和 PFX 证书</span><span class="sxs-lookup"><span data-stu-id="1a7a8-169">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="1a7a8-170">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="1a7a8-170">studentCertificateSettings</span></span>|[<span data-ttu-id="1a7a8-171">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="1a7a8-171">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="1a7a8-172">学生的受信任的根和 PFX 证书</span><span class="sxs-lookup"><span data-stu-id="1a7a8-172">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="1a7a8-173">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="1a7a8-173">deviceCertificateSettings</span></span>|[<span data-ttu-id="1a7a8-174">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="1a7a8-174">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="1a7a8-175">受信任的根和 PFX 设备的证书</span><span class="sxs-lookup"><span data-stu-id="1a7a8-175">The Trusted Root and PFX certificates for Device</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a7a8-176">Relationships</span><span class="sxs-lookup"><span data-stu-id="1a7a8-176">Relationships</span></span>
|<span data-ttu-id="1a7a8-177">关系</span><span class="sxs-lookup"><span data-stu-id="1a7a8-177">Relationship</span></span>|<span data-ttu-id="1a7a8-178">类型</span><span class="sxs-lookup"><span data-stu-id="1a7a8-178">Type</span></span>|<span data-ttu-id="1a7a8-179">Description</span><span class="sxs-lookup"><span data-stu-id="1a7a8-179">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a7a8-180">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="1a7a8-180">groupAssignments</span></span>|<span data-ttu-id="1a7a8-181">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="1a7a8-181">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="1a7a8-182">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-182">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="1a7a8-183">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a7a8-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a7a8-184">assignments</span><span class="sxs-lookup"><span data-stu-id="1a7a8-184">assignments</span></span>|<span data-ttu-id="1a7a8-185">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a7a8-185">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="1a7a8-186">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-186">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="1a7a8-187">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a7a8-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a7a8-188">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="1a7a8-188">deviceStatuses</span></span>|<span data-ttu-id="1a7a8-189">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a7a8-189">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="1a7a8-190">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-190">Device configuration installation status by device.</span></span> <span data-ttu-id="1a7a8-191">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a7a8-191">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a7a8-192">userStatuses</span><span class="sxs-lookup"><span data-stu-id="1a7a8-192">userStatuses</span></span>|<span data-ttu-id="1a7a8-193">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a7a8-193">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="1a7a8-194">用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-194">Device configuration installation status by user.</span></span> <span data-ttu-id="1a7a8-195">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a7a8-195">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a7a8-196">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="1a7a8-196">deviceStatusOverview</span></span>|[<span data-ttu-id="1a7a8-197">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1a7a8-197">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="1a7a8-198">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a7a8-198">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a7a8-199">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="1a7a8-199">userStatusOverview</span></span>|[<span data-ttu-id="1a7a8-200">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="1a7a8-200">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="1a7a8-201">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a7a8-201">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a7a8-202">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="1a7a8-202">deviceSettingStateSummaries</span></span>|<span data-ttu-id="1a7a8-203">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a7a8-203">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="1a7a8-204">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a7a8-204">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a7a8-205">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a7a8-205">JSON Representation</span></span>
<span data-ttu-id="1a7a8-206">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a7a8-206">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosEduDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "teacherCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "binary",
    "certFileName": "String",
    "certificationAuthority": "String",
    "certificationAuthorityName": "String",
    "certificateTemplateName": "String",
    "renewalThresholdPercentage": 1024,
    "certificateValidityPeriodValue": 1024,
    "certificateValidityPeriodScale": "String"
  },
  "studentCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "binary",
    "certFileName": "String",
    "certificationAuthority": "String",
    "certificationAuthorityName": "String",
    "certificateTemplateName": "String",
    "renewalThresholdPercentage": 1024,
    "certificateValidityPeriodValue": 1024,
    "certificateValidityPeriodScale": "String"
  },
  "deviceCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "binary",
    "certFileName": "String",
    "certificationAuthority": "String",
    "certificationAuthorityName": "String",
    "certificateTemplateName": "String",
    "renewalThresholdPercentage": 1024,
    "certificateValidityPeriodValue": 1024,
    "certificateValidityPeriodScale": "String"
  }
}
```





