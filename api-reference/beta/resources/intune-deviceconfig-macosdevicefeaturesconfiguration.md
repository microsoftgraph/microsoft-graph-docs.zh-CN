---
title: macOSDeviceFeaturesConfiguration 资源类型
description: MacOS 设备功能配置的配置文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3f2e3fc28f68aaec04e75d8e6d082077d821976
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268641"
---
# <a name="macosdevicefeaturesconfiguration-resource-type"></a><span data-ttu-id="1ce49-103">macOSDeviceFeaturesConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="1ce49-103">macOSDeviceFeaturesConfiguration resource type</span></span>

<span data-ttu-id="1ce49-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ce49-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ce49-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1ce49-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ce49-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1ce49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ce49-107">MacOS 设备功能配置的配置文件。</span><span class="sxs-lookup"><span data-stu-id="1ce49-107">MacOS device features configuration profile.</span></span>


<span data-ttu-id="1ce49-108">继承自 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-108">Inherits from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1ce49-109">方法</span><span class="sxs-lookup"><span data-stu-id="1ce49-109">Methods</span></span>
|<span data-ttu-id="1ce49-110">方法</span><span class="sxs-lookup"><span data-stu-id="1ce49-110">Method</span></span>|<span data-ttu-id="1ce49-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="1ce49-111">Return Type</span></span>|<span data-ttu-id="1ce49-112">说明</span><span class="sxs-lookup"><span data-stu-id="1ce49-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1ce49-113">列出 macOSDeviceFeaturesConfigurations</span><span class="sxs-lookup"><span data-stu-id="1ce49-113">List macOSDeviceFeaturesConfigurations</span></span>](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-list.md)|<span data-ttu-id="1ce49-114">[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ce49-114">[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) collection</span></span>|<span data-ttu-id="1ce49-115">列出 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1ce49-115">List properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="1ce49-116">获取 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ce49-116">Get macOSDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-get.md)|[<span data-ttu-id="1ce49-117">macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ce49-117">macOSDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|<span data-ttu-id="1ce49-118">读取 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1ce49-118">Read properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>|
|[<span data-ttu-id="1ce49-119">创建 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ce49-119">Create macOSDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-create.md)|[<span data-ttu-id="1ce49-120">macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ce49-120">macOSDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|<span data-ttu-id="1ce49-121">创建新的 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1ce49-121">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>|
|[<span data-ttu-id="1ce49-122">删除 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ce49-122">Delete macOSDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-delete.md)|<span data-ttu-id="1ce49-123">无</span><span class="sxs-lookup"><span data-stu-id="1ce49-123">None</span></span>|<span data-ttu-id="1ce49-124">删除 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="1ce49-124">Deletes a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>|
|[<span data-ttu-id="1ce49-125">更新 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ce49-125">Update macOSDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-update.md)|[<span data-ttu-id="1ce49-126">macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ce49-126">macOSDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|<span data-ttu-id="1ce49-127">更新 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1ce49-127">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1ce49-128">属性</span><span class="sxs-lookup"><span data-stu-id="1ce49-128">Properties</span></span>
|<span data-ttu-id="1ce49-129">属性</span><span class="sxs-lookup"><span data-stu-id="1ce49-129">Property</span></span>|<span data-ttu-id="1ce49-130">类型</span><span class="sxs-lookup"><span data-stu-id="1ce49-130">Type</span></span>|<span data-ttu-id="1ce49-131">说明</span><span class="sxs-lookup"><span data-stu-id="1ce49-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ce49-132">id</span><span class="sxs-lookup"><span data-stu-id="1ce49-132">id</span></span>|<span data-ttu-id="1ce49-133">字符串</span><span class="sxs-lookup"><span data-stu-id="1ce49-133">String</span></span>|<span data-ttu-id="1ce49-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1ce49-134">Key of the entity.</span></span> <span data-ttu-id="1ce49-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ce49-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1ce49-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ce49-137">DateTimeOffset</span></span>|<span data-ttu-id="1ce49-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1ce49-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1ce49-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1ce49-140">roleScopeTagIds</span></span>|<span data-ttu-id="1ce49-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="1ce49-141">String collection</span></span>|<span data-ttu-id="1ce49-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1ce49-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1ce49-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1ce49-144">supportsScopeTags</span></span>|<span data-ttu-id="1ce49-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-145">Boolean</span></span>|<span data-ttu-id="1ce49-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="1ce49-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1ce49-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="1ce49-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1ce49-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="1ce49-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1ce49-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1ce49-149">This property is read-only.</span></span> <span data-ttu-id="1ce49-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1ce49-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1ce49-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1ce49-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1ce49-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="1ce49-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1ce49-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1ce49-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1ce49-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1ce49-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1ce49-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1ce49-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1ce49-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1ce49-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1ce49-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1ce49-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1ce49-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1ce49-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1ce49-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ce49-163">createdDateTime</span></span>|<span data-ttu-id="1ce49-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ce49-164">DateTimeOffset</span></span>|<span data-ttu-id="1ce49-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1ce49-165">DateTime the object was created.</span></span> <span data-ttu-id="1ce49-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-167">description</span><span class="sxs-lookup"><span data-stu-id="1ce49-167">description</span></span>|<span data-ttu-id="1ce49-168">字符串</span><span class="sxs-lookup"><span data-stu-id="1ce49-168">String</span></span>|<span data-ttu-id="1ce49-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1ce49-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1ce49-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-171">displayName</span><span class="sxs-lookup"><span data-stu-id="1ce49-171">displayName</span></span>|<span data-ttu-id="1ce49-172">字符串</span><span class="sxs-lookup"><span data-stu-id="1ce49-172">String</span></span>|<span data-ttu-id="1ce49-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1ce49-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1ce49-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-175">version</span><span class="sxs-lookup"><span data-stu-id="1ce49-175">version</span></span>|<span data-ttu-id="1ce49-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1ce49-176">Int32</span></span>|<span data-ttu-id="1ce49-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1ce49-177">Version of the device configuration.</span></span> <span data-ttu-id="1ce49-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-179">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="1ce49-179">airPrintDestinations</span></span>|<span data-ttu-id="1ce49-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ce49-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="1ce49-181">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="1ce49-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="1ce49-182">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1ce49-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="1ce49-183">继承自 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="1ce49-184">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="1ce49-184">autoLaunchItems</span></span>|<span data-ttu-id="1ce49-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ce49-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="1ce49-186">用户登录时要启动的应用程序、文件、文件夹和其他项目的列表。</span><span class="sxs-lookup"><span data-stu-id="1ce49-186">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="1ce49-187">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1ce49-187">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1ce49-188">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="1ce49-188">adminShowHostInfo</span></span>|<span data-ttu-id="1ce49-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-189">Boolean</span></span>|<span data-ttu-id="1ce49-190">是否在登录窗口中显示管理员主机信息。</span><span class="sxs-lookup"><span data-stu-id="1ce49-190">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="1ce49-191">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="1ce49-191">loginWindowText</span></span>|<span data-ttu-id="1ce49-192">字符串</span><span class="sxs-lookup"><span data-stu-id="1ce49-192">String</span></span>|<span data-ttu-id="1ce49-193">要在登录窗口中显示的自定义文本。</span><span class="sxs-lookup"><span data-stu-id="1ce49-193">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="1ce49-194">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="1ce49-194">authorizedUsersListHidden</span></span>|<span data-ttu-id="1ce49-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-195">Boolean</span></span>|<span data-ttu-id="1ce49-196">是否在登录窗口中显示 "名称" 和 "密码" 对话框或用户列表。</span><span class="sxs-lookup"><span data-stu-id="1ce49-196">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="1ce49-197">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="1ce49-197">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="1ce49-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-198">Boolean</span></span>|<span data-ttu-id="1ce49-199">是否在登录窗口的授权用户列表中仅显示网络和系统用户。</span><span class="sxs-lookup"><span data-stu-id="1ce49-199">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="1ce49-200">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="1ce49-200">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="1ce49-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-201">Boolean</span></span>|<span data-ttu-id="1ce49-202">是否在登录窗口上的授权用户列表中隐藏移动用户。</span><span class="sxs-lookup"><span data-stu-id="1ce49-202">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="1ce49-203">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="1ce49-203">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="1ce49-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-204">Boolean</span></span>|<span data-ttu-id="1ce49-205">是否在登录窗口上的授权用户列表中显示网络用户。</span><span class="sxs-lookup"><span data-stu-id="1ce49-205">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="1ce49-206">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="1ce49-206">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="1ce49-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-207">Boolean</span></span>|<span data-ttu-id="1ce49-208">是否在登录窗口的授权用户列表中隐藏管理员用户。</span><span class="sxs-lookup"><span data-stu-id="1ce49-208">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="1ce49-209">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="1ce49-209">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="1ce49-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-210">Boolean</span></span>|<span data-ttu-id="1ce49-211">是否在登录窗口上的授权用户列表中显示其他用户。</span><span class="sxs-lookup"><span data-stu-id="1ce49-211">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="1ce49-212">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="1ce49-212">shutDownDisabled</span></span>|<span data-ttu-id="1ce49-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-213">Boolean</span></span>|<span data-ttu-id="1ce49-214">是否在登录窗口中隐藏 "关机" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="1ce49-214">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="1ce49-215">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="1ce49-215">restartDisabled</span></span>|<span data-ttu-id="1ce49-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-216">Boolean</span></span>|<span data-ttu-id="1ce49-217">是否在登录窗口中隐藏 "重新启动" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="1ce49-217">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="1ce49-218">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="1ce49-218">sleepDisabled</span></span>|<span data-ttu-id="1ce49-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-219">Boolean</span></span>|<span data-ttu-id="1ce49-220">是否在登录窗口中隐藏 "睡眠" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="1ce49-220">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="1ce49-221">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="1ce49-221">consoleAccessDisabled</span></span>|<span data-ttu-id="1ce49-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-222">Boolean</span></span>|<span data-ttu-id="1ce49-223">其他用户是否会忽略使用 ">控制台> 特殊用户名。</span><span class="sxs-lookup"><span data-stu-id="1ce49-223">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="1ce49-224">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="1ce49-224">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="1ce49-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-225">Boolean</span></span>|<span data-ttu-id="1ce49-226">用户登录时是否禁用登录窗口上的 "关闭" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="1ce49-226">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="1ce49-227">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="1ce49-227">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="1ce49-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-228">Boolean</span></span>|<span data-ttu-id="1ce49-229">用户登录时是否禁用登录窗口上的重启菜单项。</span><span class="sxs-lookup"><span data-stu-id="1ce49-229">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="1ce49-230">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="1ce49-230">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="1ce49-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-231">Boolean</span></span>|<span data-ttu-id="1ce49-232">用户登录时登录窗口上的 "断电" 菜单项是否将被禁用。</span><span class="sxs-lookup"><span data-stu-id="1ce49-232">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="1ce49-233">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="1ce49-233">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="1ce49-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-234">Boolean</span></span>|<span data-ttu-id="1ce49-235">用户登录时，登录窗口上的注销菜单项是否会被禁用。</span><span class="sxs-lookup"><span data-stu-id="1ce49-235">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="1ce49-236">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="1ce49-236">screenLockDisableImmediate</span></span>|<span data-ttu-id="1ce49-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-237">Boolean</span></span>|<span data-ttu-id="1ce49-238">是否禁用即时屏幕锁定功能。</span><span class="sxs-lookup"><span data-stu-id="1ce49-238">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="1ce49-239">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="1ce49-239">associatedDomains</span></span>|<span data-ttu-id="1ce49-240">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ce49-240">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="1ce49-241">弃用：改用 appAssociatedDomains。</span><span class="sxs-lookup"><span data-stu-id="1ce49-241">DEPRECATED: use appAssociatedDomains instead.</span></span> <span data-ttu-id="1ce49-242">获取或设置一个列表，该列表将应用程序映射到其关联的域。</span><span class="sxs-lookup"><span data-stu-id="1ce49-242">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="1ce49-243">键应与应用程序的 ID 匹配，并且值应为 "服务：域" 形式的字符串，其中 domain 是完全限定的主机名 (例如，webcredentials:example) 。</span><span class="sxs-lookup"><span data-stu-id="1ce49-243">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="1ce49-244">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1ce49-244">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1ce49-245">appAssociatedDomains</span><span class="sxs-lookup"><span data-stu-id="1ce49-245">appAssociatedDomains</span></span>|<span data-ttu-id="1ce49-246">[macOSAssociatedDomainsItem](../resources/intune-deviceconfig-macosassociateddomainsitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ce49-246">[macOSAssociatedDomainsItem](../resources/intune-deviceconfig-macosassociateddomainsitem.md) collection</span></span>|<span data-ttu-id="1ce49-247">获取或设置一个列表，该列表将应用程序映射到其关联的域。</span><span class="sxs-lookup"><span data-stu-id="1ce49-247">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="1ce49-248">应用程序标识符必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="1ce49-248">Application identifiers must be unique.</span></span> <span data-ttu-id="1ce49-249">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1ce49-249">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1ce49-250">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="1ce49-250">singleSignOnExtension</span></span>|[<span data-ttu-id="1ce49-251">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="1ce49-251">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="1ce49-252">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="1ce49-252">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="1ce49-253">弃用：改用 MacOSSingleSignOnExtension。</span><span class="sxs-lookup"><span data-stu-id="1ce49-253">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="1ce49-254">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="1ce49-254">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="1ce49-255">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="1ce49-255">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="1ce49-256">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="1ce49-256">Gets or sets a single sign-on extension profile.</span></span>|
|<span data-ttu-id="1ce49-257">contentCachingEnabled</span><span class="sxs-lookup"><span data-stu-id="1ce49-257">contentCachingEnabled</span></span>|<span data-ttu-id="1ce49-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-258">Boolean</span></span>|<span data-ttu-id="1ce49-259">启用内容缓存，并防止用户对其禁用。</span><span class="sxs-lookup"><span data-stu-id="1ce49-259">Enables content caching and prevents it from being disabled by the user.</span></span>|
|<span data-ttu-id="1ce49-260">contentCachingType</span><span class="sxs-lookup"><span data-stu-id="1ce49-260">contentCachingType</span></span>|[<span data-ttu-id="1ce49-261">macOSContentCachingType</span><span class="sxs-lookup"><span data-stu-id="1ce49-261">macOSContentCachingType</span></span>](../resources/intune-deviceconfig-macoscontentcachingtype.md)|<span data-ttu-id="1ce49-262">确定允许由 Apple 的内容缓存服务缓存的内容类型。</span><span class="sxs-lookup"><span data-stu-id="1ce49-262">Determines what type of content is allowed to be cached by Apple's content caching service.</span></span> <span data-ttu-id="1ce49-263">可取值为：`notConfigured`、`userContentOnly`、`sharedContentOnly`。</span><span class="sxs-lookup"><span data-stu-id="1ce49-263">Possible values are: `notConfigured`, `userContentOnly`, `sharedContentOnly`.</span></span>|
|<span data-ttu-id="1ce49-264">contentCachingMaxSizeBytes</span><span class="sxs-lookup"><span data-stu-id="1ce49-264">contentCachingMaxSizeBytes</span></span>|<span data-ttu-id="1ce49-265">Int32</span><span class="sxs-lookup"><span data-stu-id="1ce49-265">Int32</span></span>|<span data-ttu-id="1ce49-266">将用于内容缓存的磁盘空间的最大字节数。</span><span class="sxs-lookup"><span data-stu-id="1ce49-266">The maximum number of bytes of disk space that will be used for the content cache.</span></span> <span data-ttu-id="1ce49-267">值 0 (默认值) 指示不受限制的磁盘空间。</span><span class="sxs-lookup"><span data-stu-id="1ce49-267">A value of 0 (default) indicates unlimited disk space.</span></span> |
|<span data-ttu-id="1ce49-268">contentCachingDataPath</span><span class="sxs-lookup"><span data-stu-id="1ce49-268">contentCachingDataPath</span></span>|<span data-ttu-id="1ce49-269">字符串</span><span class="sxs-lookup"><span data-stu-id="1ce49-269">String</span></span>|<span data-ttu-id="1ce49-270">用于存储缓存内容的目录的路径。</span><span class="sxs-lookup"><span data-stu-id="1ce49-270">The path to the directory used to store cached content.</span></span> <span data-ttu-id="1ce49-271">该值必须是 (或 end with) /Library/Application 支持/Apple/AssetCache/Data</span><span class="sxs-lookup"><span data-stu-id="1ce49-271">The value must be (or end with) /Library/Application Support/Apple/AssetCache/Data</span></span>|
|<span data-ttu-id="1ce49-272">contentCachingDisableConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="1ce49-272">contentCachingDisableConnectionSharing</span></span>|<span data-ttu-id="1ce49-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-273">Boolean</span></span>|<span data-ttu-id="1ce49-274">禁用 internet 连接共享。</span><span class="sxs-lookup"><span data-stu-id="1ce49-274">Disables internet connection sharing.</span></span>|
|<span data-ttu-id="1ce49-275">contentCachingForceConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="1ce49-275">contentCachingForceConnectionSharing</span></span>|<span data-ttu-id="1ce49-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-276">Boolean</span></span>|<span data-ttu-id="1ce49-277">强制 internet 连接共享。</span><span class="sxs-lookup"><span data-stu-id="1ce49-277">Forces internet connection sharing.</span></span> <span data-ttu-id="1ce49-278">contentCachingDisableConnectionSharing 将覆盖此设置。</span><span class="sxs-lookup"><span data-stu-id="1ce49-278">contentCachingDisableConnectionSharing overrides this setting.</span></span>|
|<span data-ttu-id="1ce49-279">contentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="1ce49-279">contentCachingClientPolicy</span></span>|[<span data-ttu-id="1ce49-280">macOSContentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="1ce49-280">macOSContentCachingClientPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingclientpolicy.md)|<span data-ttu-id="1ce49-281">确定内容缓存服务器将在其中侦听客户端的方法。</span><span class="sxs-lookup"><span data-stu-id="1ce49-281">Determines the method in which content caching servers will listen for clients.</span></span> <span data-ttu-id="1ce49-282">可取值为：`notConfigured`、`clientsInLocalNetwork`、`clientsWithSamePublicIpAddress`、`clientsInCustomLocalNetworks`、`clientsInCustomLocalNetworksWithFallback`。</span><span class="sxs-lookup"><span data-stu-id="1ce49-282">Possible values are: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.</span></span>|
|<span data-ttu-id="1ce49-283">contentCachingClientListenRanges</span><span class="sxs-lookup"><span data-stu-id="1ce49-283">contentCachingClientListenRanges</span></span>|<span data-ttu-id="1ce49-284">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ce49-284">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="1ce49-285">自定义 IP 范围的列表将用于侦听客户端。</span><span class="sxs-lookup"><span data-stu-id="1ce49-285">A list of custom IP ranges content caches will use to listen for clients.</span></span> <span data-ttu-id="1ce49-286">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1ce49-286">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1ce49-287">contentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="1ce49-287">contentCachingPeerPolicy</span></span>|[<span data-ttu-id="1ce49-288">macOSContentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="1ce49-288">macOSContentCachingPeerPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingpeerpolicy.md)|<span data-ttu-id="1ce49-289">确定内容缓存对等方和其他缓存的方法。</span><span class="sxs-lookup"><span data-stu-id="1ce49-289">Determines the method in which content caches peer with other caches.</span></span> <span data-ttu-id="1ce49-290">可取值为：`notConfigured`、`peersInLocalNetwork`、`peersWithSamePublicIpAddress`、`peersInCustomLocalNetworks`。</span><span class="sxs-lookup"><span data-stu-id="1ce49-290">Possible values are: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.</span></span>|
|<span data-ttu-id="1ce49-291">contentCachingPeerListenRanges</span><span class="sxs-lookup"><span data-stu-id="1ce49-291">contentCachingPeerListenRanges</span></span>|<span data-ttu-id="1ce49-292">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ce49-292">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="1ce49-293">将使用自定义 IP 范围的列表来侦听对等缓存的内容缓存。</span><span class="sxs-lookup"><span data-stu-id="1ce49-293">A list of custom IP ranges content caches will use to listen for peer caches.</span></span> <span data-ttu-id="1ce49-294">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1ce49-294">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1ce49-295">contentCachingPeerFilterRanges</span><span class="sxs-lookup"><span data-stu-id="1ce49-295">contentCachingPeerFilterRanges</span></span>|<span data-ttu-id="1ce49-296">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ce49-296">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="1ce49-297">自定义 IP 范围的列表中，内容缓存将用于查询来自对等缓存的内容。</span><span class="sxs-lookup"><span data-stu-id="1ce49-297">A list of custom IP ranges content caches will use to query for content from peers caches.</span></span> <span data-ttu-id="1ce49-298">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1ce49-298">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1ce49-299">contentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="1ce49-299">contentCachingParentSelectionPolicy</span></span>|[<span data-ttu-id="1ce49-300">macOSContentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="1ce49-300">macOSContentCachingParentSelectionPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingparentselectionpolicy.md)|<span data-ttu-id="1ce49-301">确定内容缓存服务器将选择父项（如果有多个）的方法。</span><span class="sxs-lookup"><span data-stu-id="1ce49-301">Determines the method in which content caching servers will select parents if multiple are present.</span></span> <span data-ttu-id="1ce49-302">可取值为：`notConfigured`、`roundRobin`、`firstAvailable`、`urlPathHash`、`random`、`stickyAvailable`。</span><span class="sxs-lookup"><span data-stu-id="1ce49-302">Possible values are: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.</span></span>|
|<span data-ttu-id="1ce49-303">contentCachingParents</span><span class="sxs-lookup"><span data-stu-id="1ce49-303">contentCachingParents</span></span>|<span data-ttu-id="1ce49-304">String 集合</span><span class="sxs-lookup"><span data-stu-id="1ce49-304">String collection</span></span>|<span data-ttu-id="1ce49-305">表示父内容缓存的 IP 地址的列表。</span><span class="sxs-lookup"><span data-stu-id="1ce49-305">A list of IP addresses representing parent content caches.</span></span>|
|<span data-ttu-id="1ce49-306">contentCachingLogClientIdentities</span><span class="sxs-lookup"><span data-stu-id="1ce49-306">contentCachingLogClientIdentities</span></span>|<span data-ttu-id="1ce49-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-307">Boolean</span></span>|<span data-ttu-id="1ce49-308">启用对请求缓存内容的客户端的 IP 地址和端口的日志记录。</span><span class="sxs-lookup"><span data-stu-id="1ce49-308">Enables logging of IP addresses and ports of clients that request cached content.</span></span>|
|<span data-ttu-id="1ce49-309">contentCachingPublicRanges</span><span class="sxs-lookup"><span data-stu-id="1ce49-309">contentCachingPublicRanges</span></span>|<span data-ttu-id="1ce49-310">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ce49-310">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="1ce49-311">Apple 的内容缓存服务应用于将客户端与内容缓存匹配的自定义 IP 范围的列表。</span><span class="sxs-lookup"><span data-stu-id="1ce49-311">A list of custom IP ranges that Apple's content caching service should use to match clients to content caches.</span></span> <span data-ttu-id="1ce49-312">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1ce49-312">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1ce49-313">contentCachingBlockDeletion</span><span class="sxs-lookup"><span data-stu-id="1ce49-313">contentCachingBlockDeletion</span></span>|<span data-ttu-id="1ce49-314">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-314">Boolean</span></span>|<span data-ttu-id="1ce49-315">防止内容缓存清除内容以释放磁盘空间以用于其他应用程序。</span><span class="sxs-lookup"><span data-stu-id="1ce49-315">Prevents content caches from purging content to free up disk space for other apps.</span></span>|
|<span data-ttu-id="1ce49-316">contentCachingShowAlerts</span><span class="sxs-lookup"><span data-stu-id="1ce49-316">contentCachingShowAlerts</span></span>|<span data-ttu-id="1ce49-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-317">Boolean</span></span>|<span data-ttu-id="1ce49-318">将内容缓存警报显示为系统通知。</span><span class="sxs-lookup"><span data-stu-id="1ce49-318">Display content caching alerts as system notifications.</span></span>|
|<span data-ttu-id="1ce49-319">contentCachingKeepAwake</span><span class="sxs-lookup"><span data-stu-id="1ce49-319">contentCachingKeepAwake</span></span>|<span data-ttu-id="1ce49-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce49-320">Boolean</span></span>|<span data-ttu-id="1ce49-321">如果启用了内容缓存，则阻止设备进入睡眠状态。</span><span class="sxs-lookup"><span data-stu-id="1ce49-321">Prevent the device from sleeping if content caching is enabled.</span></span>|
|<span data-ttu-id="1ce49-322">contentCachingPort</span><span class="sxs-lookup"><span data-stu-id="1ce49-322">contentCachingPort</span></span>|<span data-ttu-id="1ce49-323">Int32</span><span class="sxs-lookup"><span data-stu-id="1ce49-323">Int32</span></span>|<span data-ttu-id="1ce49-324">设置用于内容缓存的端口。</span><span class="sxs-lookup"><span data-stu-id="1ce49-324">Sets the port used for content caching.</span></span> <span data-ttu-id="1ce49-325">如果值为0，则将选择随机可用端口。</span><span class="sxs-lookup"><span data-stu-id="1ce49-325">If the value is 0, a random available port will be selected.</span></span> <span data-ttu-id="1ce49-326">有效值为0至65535</span><span class="sxs-lookup"><span data-stu-id="1ce49-326">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ce49-327">关系</span><span class="sxs-lookup"><span data-stu-id="1ce49-327">Relationships</span></span>
|<span data-ttu-id="1ce49-328">关系</span><span class="sxs-lookup"><span data-stu-id="1ce49-328">Relationship</span></span>|<span data-ttu-id="1ce49-329">类型</span><span class="sxs-lookup"><span data-stu-id="1ce49-329">Type</span></span>|<span data-ttu-id="1ce49-330">说明</span><span class="sxs-lookup"><span data-stu-id="1ce49-330">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ce49-331">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="1ce49-331">groupAssignments</span></span>|<span data-ttu-id="1ce49-332">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ce49-332">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="1ce49-333">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="1ce49-333">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="1ce49-334">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-334">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-335">assignments</span><span class="sxs-lookup"><span data-stu-id="1ce49-335">assignments</span></span>|<span data-ttu-id="1ce49-336">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ce49-336">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="1ce49-337">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="1ce49-337">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="1ce49-338">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-338">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-339">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="1ce49-339">deviceStatuses</span></span>|<span data-ttu-id="1ce49-340">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ce49-340">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="1ce49-341">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="1ce49-341">Device configuration installation status by device.</span></span> <span data-ttu-id="1ce49-342">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-342">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-343">userStatuses</span><span class="sxs-lookup"><span data-stu-id="1ce49-343">userStatuses</span></span>|<span data-ttu-id="1ce49-344">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ce49-344">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="1ce49-345">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="1ce49-345">Device configuration installation status by user.</span></span> <span data-ttu-id="1ce49-346">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-346">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-347">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="1ce49-347">deviceStatusOverview</span></span>|[<span data-ttu-id="1ce49-348">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1ce49-348">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="1ce49-349">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-349">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-350">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="1ce49-350">userStatusOverview</span></span>|[<span data-ttu-id="1ce49-351">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="1ce49-351">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="1ce49-352">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-352">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-353">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="1ce49-353">deviceSettingStateSummaries</span></span>|<span data-ttu-id="1ce49-354">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ce49-354">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="1ce49-355">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ce49-355">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ce49-356">singleSignOnExtensionPkinitCertificate</span><span class="sxs-lookup"><span data-stu-id="1ce49-356">singleSignOnExtensionPkinitCertificate</span></span>|[<span data-ttu-id="1ce49-357">macOSCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="1ce49-357">macOSCertificateProfileBase</span></span>](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|<span data-ttu-id="1ce49-358">用于使用单一登录扩展的身份验证的 PKINIT 证书。</span><span class="sxs-lookup"><span data-stu-id="1ce49-358">PKINIT Certificate for the authentication with single sign-on extensions.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1ce49-359">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ce49-359">JSON Representation</span></span>
<span data-ttu-id="1ce49-360">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ce49-360">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSDeviceFeaturesConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "String",
      "resourcePath": "String",
      "port": 1024,
      "forceTls": true
    }
  ],
  "autoLaunchItems": [
    {
      "@odata.type": "microsoft.graph.macOSLaunchItem",
      "path": "String",
      "hide": true
    }
  ],
  "adminShowHostInfo": true,
  "loginWindowText": "String",
  "authorizedUsersListHidden": true,
  "authorizedUsersListHideLocalUsers": true,
  "authorizedUsersListHideMobileAccounts": true,
  "authorizedUsersListIncludeNetworkUsers": true,
  "authorizedUsersListHideAdminUsers": true,
  "authorizedUsersListShowOtherManagedUsers": true,
  "shutDownDisabled": true,
  "restartDisabled": true,
  "sleepDisabled": true,
  "consoleAccessDisabled": true,
  "shutDownDisabledWhileLoggedIn": true,
  "restartDisabledWhileLoggedIn": true,
  "powerOffDisabledWhileLoggedIn": true,
  "logOutDisabledWhileLoggedIn": true,
  "screenLockDisableImmediate": true,
  "associatedDomains": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "appAssociatedDomains": [
    {
      "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem",
      "applicationIdentifier": "String",
      "domains": [
        "String"
      ],
      "directDownloadsEnabled": true
    }
  ],
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.credentialSingleSignOnExtension",
    "extensionIdentifier": "String",
    "teamIdentifier": "String",
    "domains": [
      "String"
    ],
    "realm": "String",
    "configurations": [
      {
        "@odata.type": "microsoft.graph.keyStringValuePair",
        "key": "String",
        "value": "String"
      }
    ]
  },
  "macOSSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension",
    "realm": "String",
    "domains": [
      "String"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "String",
    "credentialBundleIdAccessControlList": [
      "String"
    ],
    "domainRealms": [
      "String"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 1024,
    "passwordExpirationNotificationDays": 1024,
    "userPrincipalName": "String",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 1024,
    "passwordMinimumLength": 1024,
    "passwordMinimumAgeDays": 1024,
    "passwordRequirementsDescription": "String",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "String",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "String"
  },
  "contentCachingEnabled": true,
  "contentCachingType": "String",
  "contentCachingMaxSizeBytes": 1024,
  "contentCachingDataPath": "String",
  "contentCachingDisableConnectionSharing": true,
  "contentCachingForceConnectionSharing": true,
  "contentCachingClientPolicy": "String",
  "contentCachingClientListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "contentCachingPeerPolicy": "String",
  "contentCachingPeerListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "contentCachingPeerFilterRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "contentCachingParentSelectionPolicy": "String",
  "contentCachingParents": [
    "String"
  ],
  "contentCachingLogClientIdentities": true,
  "contentCachingPublicRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "contentCachingBlockDeletion": true,
  "contentCachingShowAlerts": true,
  "contentCachingKeepAwake": true,
  "contentCachingPort": 1024
}
```




