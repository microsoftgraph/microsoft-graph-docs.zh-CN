---
title: macOSDeviceFeaturesConfiguration 资源类型
description: MacOS 设备功能配置的配置文件。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f79736f53fe67372447cab7b1f133818d48098d
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44788841"
---
# <a name="macosdevicefeaturesconfiguration-resource-type"></a><span data-ttu-id="93f99-103">macOSDeviceFeaturesConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="93f99-103">macOSDeviceFeaturesConfiguration resource type</span></span>

<span data-ttu-id="93f99-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93f99-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93f99-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="93f99-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93f99-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="93f99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93f99-107">MacOS 设备功能配置的配置文件。</span><span class="sxs-lookup"><span data-stu-id="93f99-107">MacOS device features configuration profile.</span></span>


<span data-ttu-id="93f99-108">继承自 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-108">Inherits from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>

## <a name="methods"></a><span data-ttu-id="93f99-109">Methods</span><span class="sxs-lookup"><span data-stu-id="93f99-109">Methods</span></span>
|<span data-ttu-id="93f99-110">方法</span><span class="sxs-lookup"><span data-stu-id="93f99-110">Method</span></span>|<span data-ttu-id="93f99-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="93f99-111">Return Type</span></span>|<span data-ttu-id="93f99-112">说明</span><span class="sxs-lookup"><span data-stu-id="93f99-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="93f99-113">列出 macOSDeviceFeaturesConfigurations</span><span class="sxs-lookup"><span data-stu-id="93f99-113">List macOSDeviceFeaturesConfigurations</span></span>](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-list.md)|<span data-ttu-id="93f99-114">[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="93f99-114">[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) collection</span></span>|<span data-ttu-id="93f99-115">列出 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="93f99-115">List properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="93f99-116">获取 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="93f99-116">Get macOSDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-get.md)|[<span data-ttu-id="93f99-117">macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="93f99-117">macOSDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|<span data-ttu-id="93f99-118">读取 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="93f99-118">Read properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>|
|[<span data-ttu-id="93f99-119">创建 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="93f99-119">Create macOSDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-create.md)|[<span data-ttu-id="93f99-120">macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="93f99-120">macOSDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|<span data-ttu-id="93f99-121">创建新的 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="93f99-121">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>|
|[<span data-ttu-id="93f99-122">删除 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="93f99-122">Delete macOSDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-delete.md)|<span data-ttu-id="93f99-123">无</span><span class="sxs-lookup"><span data-stu-id="93f99-123">None</span></span>|<span data-ttu-id="93f99-124">删除 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="93f99-124">Deletes a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>|
|[<span data-ttu-id="93f99-125">更新 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="93f99-125">Update macOSDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-update.md)|[<span data-ttu-id="93f99-126">macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="93f99-126">macOSDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|<span data-ttu-id="93f99-127">更新 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="93f99-127">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="93f99-128">属性</span><span class="sxs-lookup"><span data-stu-id="93f99-128">Properties</span></span>
|<span data-ttu-id="93f99-129">属性</span><span class="sxs-lookup"><span data-stu-id="93f99-129">Property</span></span>|<span data-ttu-id="93f99-130">类型</span><span class="sxs-lookup"><span data-stu-id="93f99-130">Type</span></span>|<span data-ttu-id="93f99-131">说明</span><span class="sxs-lookup"><span data-stu-id="93f99-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93f99-132">id</span><span class="sxs-lookup"><span data-stu-id="93f99-132">id</span></span>|<span data-ttu-id="93f99-133">字符串</span><span class="sxs-lookup"><span data-stu-id="93f99-133">String</span></span>|<span data-ttu-id="93f99-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="93f99-134">Key of the entity.</span></span> <span data-ttu-id="93f99-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93f99-136">lastModifiedDateTime</span></span>|<span data-ttu-id="93f99-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93f99-137">DateTimeOffset</span></span>|<span data-ttu-id="93f99-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="93f99-138">DateTime the object was last modified.</span></span> <span data-ttu-id="93f99-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="93f99-140">roleScopeTagIds</span></span>|<span data-ttu-id="93f99-141">String collection</span><span class="sxs-lookup"><span data-stu-id="93f99-141">String collection</span></span>|<span data-ttu-id="93f99-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="93f99-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="93f99-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="93f99-144">supportsScopeTags</span></span>|<span data-ttu-id="93f99-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-145">Boolean</span></span>|<span data-ttu-id="93f99-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="93f99-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="93f99-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="93f99-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="93f99-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="93f99-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="93f99-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="93f99-149">This property is read-only.</span></span> <span data-ttu-id="93f99-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="93f99-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="93f99-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="93f99-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="93f99-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="93f99-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="93f99-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="93f99-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="93f99-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="93f99-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="93f99-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="93f99-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="93f99-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="93f99-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="93f99-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="93f99-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="93f99-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="93f99-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="93f99-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93f99-163">createdDateTime</span></span>|<span data-ttu-id="93f99-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93f99-164">DateTimeOffset</span></span>|<span data-ttu-id="93f99-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="93f99-165">DateTime the object was created.</span></span> <span data-ttu-id="93f99-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-167">说明</span><span class="sxs-lookup"><span data-stu-id="93f99-167">description</span></span>|<span data-ttu-id="93f99-168">String</span><span class="sxs-lookup"><span data-stu-id="93f99-168">String</span></span>|<span data-ttu-id="93f99-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="93f99-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="93f99-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-171">displayName</span><span class="sxs-lookup"><span data-stu-id="93f99-171">displayName</span></span>|<span data-ttu-id="93f99-172">String</span><span class="sxs-lookup"><span data-stu-id="93f99-172">String</span></span>|<span data-ttu-id="93f99-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="93f99-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="93f99-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-175">version</span><span class="sxs-lookup"><span data-stu-id="93f99-175">version</span></span>|<span data-ttu-id="93f99-176">Int32</span><span class="sxs-lookup"><span data-stu-id="93f99-176">Int32</span></span>|<span data-ttu-id="93f99-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="93f99-177">Version of the device configuration.</span></span> <span data-ttu-id="93f99-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-179">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="93f99-179">airPrintDestinations</span></span>|<span data-ttu-id="93f99-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)集合</span><span class="sxs-lookup"><span data-stu-id="93f99-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="93f99-181">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="93f99-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="93f99-182">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="93f99-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="93f99-183">继承自[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="93f99-184">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="93f99-184">autoLaunchItems</span></span>|<span data-ttu-id="93f99-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="93f99-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="93f99-186">用户登录时要启动的应用程序、文件、文件夹和其他项目的列表。</span><span class="sxs-lookup"><span data-stu-id="93f99-186">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="93f99-187">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="93f99-187">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="93f99-188">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="93f99-188">adminShowHostInfo</span></span>|<span data-ttu-id="93f99-189">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-189">Boolean</span></span>|<span data-ttu-id="93f99-190">是否在登录窗口中显示管理员主机信息。</span><span class="sxs-lookup"><span data-stu-id="93f99-190">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="93f99-191">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="93f99-191">loginWindowText</span></span>|<span data-ttu-id="93f99-192">String</span><span class="sxs-lookup"><span data-stu-id="93f99-192">String</span></span>|<span data-ttu-id="93f99-193">要在登录窗口中显示的自定义文本。</span><span class="sxs-lookup"><span data-stu-id="93f99-193">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="93f99-194">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="93f99-194">authorizedUsersListHidden</span></span>|<span data-ttu-id="93f99-195">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-195">Boolean</span></span>|<span data-ttu-id="93f99-196">是否在登录窗口中显示 "名称" 和 "密码" 对话框或用户列表。</span><span class="sxs-lookup"><span data-stu-id="93f99-196">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="93f99-197">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="93f99-197">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="93f99-198">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-198">Boolean</span></span>|<span data-ttu-id="93f99-199">是否在登录窗口的授权用户列表中仅显示网络和系统用户。</span><span class="sxs-lookup"><span data-stu-id="93f99-199">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="93f99-200">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="93f99-200">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="93f99-201">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-201">Boolean</span></span>|<span data-ttu-id="93f99-202">是否在登录窗口上的授权用户列表中隐藏移动用户。</span><span class="sxs-lookup"><span data-stu-id="93f99-202">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="93f99-203">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="93f99-203">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="93f99-204">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-204">Boolean</span></span>|<span data-ttu-id="93f99-205">是否在登录窗口上的授权用户列表中显示网络用户。</span><span class="sxs-lookup"><span data-stu-id="93f99-205">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="93f99-206">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="93f99-206">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="93f99-207">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-207">Boolean</span></span>|<span data-ttu-id="93f99-208">是否在登录窗口的授权用户列表中隐藏管理员用户。</span><span class="sxs-lookup"><span data-stu-id="93f99-208">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="93f99-209">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="93f99-209">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="93f99-210">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-210">Boolean</span></span>|<span data-ttu-id="93f99-211">是否在登录窗口上的授权用户列表中显示其他用户。</span><span class="sxs-lookup"><span data-stu-id="93f99-211">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="93f99-212">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="93f99-212">shutDownDisabled</span></span>|<span data-ttu-id="93f99-213">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-213">Boolean</span></span>|<span data-ttu-id="93f99-214">是否在登录窗口中隐藏 "关机" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="93f99-214">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="93f99-215">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="93f99-215">restartDisabled</span></span>|<span data-ttu-id="93f99-216">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-216">Boolean</span></span>|<span data-ttu-id="93f99-217">是否在登录窗口中隐藏 "重新启动" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="93f99-217">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="93f99-218">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="93f99-218">sleepDisabled</span></span>|<span data-ttu-id="93f99-219">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-219">Boolean</span></span>|<span data-ttu-id="93f99-220">是否在登录窗口中隐藏 "睡眠" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="93f99-220">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="93f99-221">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="93f99-221">consoleAccessDisabled</span></span>|<span data-ttu-id="93f99-222">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-222">Boolean</span></span>|<span data-ttu-id="93f99-223">其他用户是否会忽略使用 ">控制台> 特殊用户名。</span><span class="sxs-lookup"><span data-stu-id="93f99-223">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="93f99-224">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="93f99-224">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="93f99-225">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-225">Boolean</span></span>|<span data-ttu-id="93f99-226">用户登录时是否禁用登录窗口上的 "关闭" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="93f99-226">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="93f99-227">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="93f99-227">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="93f99-228">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-228">Boolean</span></span>|<span data-ttu-id="93f99-229">用户登录时是否禁用登录窗口上的重启菜单项。</span><span class="sxs-lookup"><span data-stu-id="93f99-229">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="93f99-230">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="93f99-230">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="93f99-231">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-231">Boolean</span></span>|<span data-ttu-id="93f99-232">用户登录时登录窗口上的 "断电" 菜单项是否将被禁用。</span><span class="sxs-lookup"><span data-stu-id="93f99-232">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="93f99-233">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="93f99-233">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="93f99-234">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-234">Boolean</span></span>|<span data-ttu-id="93f99-235">用户登录时，登录窗口上的注销菜单项是否会被禁用。</span><span class="sxs-lookup"><span data-stu-id="93f99-235">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="93f99-236">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="93f99-236">screenLockDisableImmediate</span></span>|<span data-ttu-id="93f99-237">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-237">Boolean</span></span>|<span data-ttu-id="93f99-238">是否禁用即时屏幕锁定功能。</span><span class="sxs-lookup"><span data-stu-id="93f99-238">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="93f99-239">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="93f99-239">associatedDomains</span></span>|<span data-ttu-id="93f99-240">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="93f99-240">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="93f99-241">获取或设置一个列表，该列表将应用程序映射到其关联的域。</span><span class="sxs-lookup"><span data-stu-id="93f99-241">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="93f99-242">该密钥应与应用程序的 ID 匹配，并且值应为 "服务：域" 形式的字符串，其中 domain 是完全限定的主机名（例如 webcredentials:example）。</span><span class="sxs-lookup"><span data-stu-id="93f99-242">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="93f99-243">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="93f99-243">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="93f99-244">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="93f99-244">singleSignOnExtension</span></span>|[<span data-ttu-id="93f99-245">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="93f99-245">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="93f99-246">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="93f99-246">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="93f99-247">弃用：改用 MacOSSingleSignOnExtension。</span><span class="sxs-lookup"><span data-stu-id="93f99-247">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="93f99-248">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="93f99-248">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="93f99-249">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="93f99-249">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="93f99-250">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="93f99-250">Gets or sets a single sign-on extension profile.</span></span>|
|<span data-ttu-id="93f99-251">contentCachingEnabled</span><span class="sxs-lookup"><span data-stu-id="93f99-251">contentCachingEnabled</span></span>|<span data-ttu-id="93f99-252">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-252">Boolean</span></span>|<span data-ttu-id="93f99-253">启用内容缓存，并防止用户对其禁用。</span><span class="sxs-lookup"><span data-stu-id="93f99-253">Enables content caching and prevents it from being disabled by the user.</span></span>|
|<span data-ttu-id="93f99-254">contentCachingType</span><span class="sxs-lookup"><span data-stu-id="93f99-254">contentCachingType</span></span>|[<span data-ttu-id="93f99-255">macOSContentCachingType</span><span class="sxs-lookup"><span data-stu-id="93f99-255">macOSContentCachingType</span></span>](../resources/intune-deviceconfig-macoscontentcachingtype.md)|<span data-ttu-id="93f99-256">确定允许由 Apple 的内容缓存服务缓存的内容类型。</span><span class="sxs-lookup"><span data-stu-id="93f99-256">Determines what type of content is allowed to be cached by Apple's content caching service.</span></span> <span data-ttu-id="93f99-257">可取值为：`notConfigured`、`userContentOnly`、`sharedContentOnly`。</span><span class="sxs-lookup"><span data-stu-id="93f99-257">Possible values are: `notConfigured`, `userContentOnly`, `sharedContentOnly`.</span></span>|
|<span data-ttu-id="93f99-258">contentCachingMaxSizeBytes</span><span class="sxs-lookup"><span data-stu-id="93f99-258">contentCachingMaxSizeBytes</span></span>|<span data-ttu-id="93f99-259">Int32</span><span class="sxs-lookup"><span data-stu-id="93f99-259">Int32</span></span>|<span data-ttu-id="93f99-260">将用于内容缓存的磁盘空间的最大字节数。</span><span class="sxs-lookup"><span data-stu-id="93f99-260">The maximum number of bytes of disk space that will be used for the content cache.</span></span> <span data-ttu-id="93f99-261">值为0（默认值）表示无限制的磁盘空间。</span><span class="sxs-lookup"><span data-stu-id="93f99-261">A value of 0 (default) indicates unlimited disk space.</span></span> |
|<span data-ttu-id="93f99-262">contentCachingDataPath</span><span class="sxs-lookup"><span data-stu-id="93f99-262">contentCachingDataPath</span></span>|<span data-ttu-id="93f99-263">String</span><span class="sxs-lookup"><span data-stu-id="93f99-263">String</span></span>|<span data-ttu-id="93f99-264">用于存储缓存内容的目录的路径。</span><span class="sxs-lookup"><span data-stu-id="93f99-264">The path to the directory used to store cached content.</span></span> <span data-ttu-id="93f99-265">值必须是（或 end with）/Library/Application 支持/Apple/AssetCache/Data</span><span class="sxs-lookup"><span data-stu-id="93f99-265">The value must be (or end with) /Library/Application Support/Apple/AssetCache/Data</span></span>|
|<span data-ttu-id="93f99-266">contentCachingDisableConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="93f99-266">contentCachingDisableConnectionSharing</span></span>|<span data-ttu-id="93f99-267">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-267">Boolean</span></span>|<span data-ttu-id="93f99-268">禁用 internet 连接共享。</span><span class="sxs-lookup"><span data-stu-id="93f99-268">Disables internet connection sharing.</span></span>|
|<span data-ttu-id="93f99-269">contentCachingForceConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="93f99-269">contentCachingForceConnectionSharing</span></span>|<span data-ttu-id="93f99-270">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-270">Boolean</span></span>|<span data-ttu-id="93f99-271">强制 internet 连接共享。</span><span class="sxs-lookup"><span data-stu-id="93f99-271">Forces internet connection sharing.</span></span> <span data-ttu-id="93f99-272">contentCachingDisableConnectionSharing 将覆盖此设置。</span><span class="sxs-lookup"><span data-stu-id="93f99-272">contentCachingDisableConnectionSharing overrides this setting.</span></span>|
|<span data-ttu-id="93f99-273">contentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="93f99-273">contentCachingClientPolicy</span></span>|[<span data-ttu-id="93f99-274">macOSContentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="93f99-274">macOSContentCachingClientPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingclientpolicy.md)|<span data-ttu-id="93f99-275">确定内容缓存服务器将在其中侦听客户端的方法。</span><span class="sxs-lookup"><span data-stu-id="93f99-275">Determines the method in which content caching servers will listen for clients.</span></span> <span data-ttu-id="93f99-276">可取值为：`notConfigured`、`clientsInLocalNetwork`、`clientsWithSamePublicIpAddress`、`clientsInCustomLocalNetworks`、`clientsInCustomLocalNetworksWithFallback`。</span><span class="sxs-lookup"><span data-stu-id="93f99-276">Possible values are: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.</span></span>|
|<span data-ttu-id="93f99-277">contentCachingClientListenRanges</span><span class="sxs-lookup"><span data-stu-id="93f99-277">contentCachingClientListenRanges</span></span>|<span data-ttu-id="93f99-278">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="93f99-278">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="93f99-279">自定义 IP 范围的列表将用于侦听客户端。</span><span class="sxs-lookup"><span data-stu-id="93f99-279">A list of custom IP ranges content caches will use to listen for clients.</span></span> <span data-ttu-id="93f99-280">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="93f99-280">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="93f99-281">contentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="93f99-281">contentCachingPeerPolicy</span></span>|[<span data-ttu-id="93f99-282">macOSContentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="93f99-282">macOSContentCachingPeerPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingpeerpolicy.md)|<span data-ttu-id="93f99-283">确定内容缓存对等方和其他缓存的方法。</span><span class="sxs-lookup"><span data-stu-id="93f99-283">Determines the method in which content caches peer with other caches.</span></span> <span data-ttu-id="93f99-284">可取值为：`notConfigured`、`peersInLocalNetwork`、`peersWithSamePublicIpAddress`、`peersInCustomLocalNetworks`。</span><span class="sxs-lookup"><span data-stu-id="93f99-284">Possible values are: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.</span></span>|
|<span data-ttu-id="93f99-285">contentCachingPeerListenRanges</span><span class="sxs-lookup"><span data-stu-id="93f99-285">contentCachingPeerListenRanges</span></span>|<span data-ttu-id="93f99-286">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="93f99-286">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="93f99-287">将使用自定义 IP 范围的列表来侦听对等缓存的内容缓存。</span><span class="sxs-lookup"><span data-stu-id="93f99-287">A list of custom IP ranges content caches will use to listen for peer caches.</span></span> <span data-ttu-id="93f99-288">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="93f99-288">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="93f99-289">contentCachingPeerFilterRanges</span><span class="sxs-lookup"><span data-stu-id="93f99-289">contentCachingPeerFilterRanges</span></span>|<span data-ttu-id="93f99-290">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="93f99-290">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="93f99-291">自定义 IP 范围的列表中，内容缓存将用于查询来自对等缓存的内容。</span><span class="sxs-lookup"><span data-stu-id="93f99-291">A list of custom IP ranges content caches will use to query for content from peers caches.</span></span> <span data-ttu-id="93f99-292">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="93f99-292">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="93f99-293">contentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="93f99-293">contentCachingParentSelectionPolicy</span></span>|[<span data-ttu-id="93f99-294">macOSContentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="93f99-294">macOSContentCachingParentSelectionPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingparentselectionpolicy.md)|<span data-ttu-id="93f99-295">确定内容缓存服务器将选择父项（如果有多个）的方法。</span><span class="sxs-lookup"><span data-stu-id="93f99-295">Determines the method in which content caching servers will select parents if multiple are present.</span></span> <span data-ttu-id="93f99-296">可取值为：`notConfigured`、`roundRobin`、`firstAvailable`、`urlPathHash`、`random`、`stickyAvailable`。</span><span class="sxs-lookup"><span data-stu-id="93f99-296">Possible values are: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.</span></span>|
|<span data-ttu-id="93f99-297">contentCachingParents</span><span class="sxs-lookup"><span data-stu-id="93f99-297">contentCachingParents</span></span>|<span data-ttu-id="93f99-298">String collection</span><span class="sxs-lookup"><span data-stu-id="93f99-298">String collection</span></span>|<span data-ttu-id="93f99-299">表示父内容缓存的 IP 地址的列表。</span><span class="sxs-lookup"><span data-stu-id="93f99-299">A list of IP addresses representing parent content caches.</span></span>|
|<span data-ttu-id="93f99-300">contentCachingLogClientIdentities</span><span class="sxs-lookup"><span data-stu-id="93f99-300">contentCachingLogClientIdentities</span></span>|<span data-ttu-id="93f99-301">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-301">Boolean</span></span>|<span data-ttu-id="93f99-302">启用对请求缓存内容的客户端的 IP 地址和端口的日志记录。</span><span class="sxs-lookup"><span data-stu-id="93f99-302">Enables logging of IP addresses and ports of clients that request cached content.</span></span>|
|<span data-ttu-id="93f99-303">contentCachingPublicRanges</span><span class="sxs-lookup"><span data-stu-id="93f99-303">contentCachingPublicRanges</span></span>|<span data-ttu-id="93f99-304">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="93f99-304">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="93f99-305">Apple 的内容缓存服务应用于将客户端与内容缓存匹配的自定义 IP 范围的列表。</span><span class="sxs-lookup"><span data-stu-id="93f99-305">A list of custom IP ranges that Apple's content caching service should use to match clients to content caches.</span></span> <span data-ttu-id="93f99-306">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="93f99-306">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="93f99-307">contentCachingBlockDeletion</span><span class="sxs-lookup"><span data-stu-id="93f99-307">contentCachingBlockDeletion</span></span>|<span data-ttu-id="93f99-308">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-308">Boolean</span></span>|<span data-ttu-id="93f99-309">防止内容缓存清除内容以释放磁盘空间以用于其他应用程序。</span><span class="sxs-lookup"><span data-stu-id="93f99-309">Prevents content caches from purging content to free up disk space for other apps.</span></span>|
|<span data-ttu-id="93f99-310">contentCachingShowAlerts</span><span class="sxs-lookup"><span data-stu-id="93f99-310">contentCachingShowAlerts</span></span>|<span data-ttu-id="93f99-311">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-311">Boolean</span></span>|<span data-ttu-id="93f99-312">将内容缓存警报显示为系统通知。</span><span class="sxs-lookup"><span data-stu-id="93f99-312">Display content caching alerts as system notifications.</span></span>|
|<span data-ttu-id="93f99-313">contentCachingKeepAwake</span><span class="sxs-lookup"><span data-stu-id="93f99-313">contentCachingKeepAwake</span></span>|<span data-ttu-id="93f99-314">布尔值</span><span class="sxs-lookup"><span data-stu-id="93f99-314">Boolean</span></span>|<span data-ttu-id="93f99-315">如果启用了内容缓存，则阻止设备进入睡眠状态。</span><span class="sxs-lookup"><span data-stu-id="93f99-315">Prevent the device from sleeping if content caching is enabled.</span></span>|
|<span data-ttu-id="93f99-316">contentCachingPort</span><span class="sxs-lookup"><span data-stu-id="93f99-316">contentCachingPort</span></span>|<span data-ttu-id="93f99-317">Int32</span><span class="sxs-lookup"><span data-stu-id="93f99-317">Int32</span></span>|<span data-ttu-id="93f99-318">设置用于内容缓存的端口。</span><span class="sxs-lookup"><span data-stu-id="93f99-318">Sets the port used for content caching.</span></span> <span data-ttu-id="93f99-319">如果值为0，则将选择随机可用端口。</span><span class="sxs-lookup"><span data-stu-id="93f99-319">If the value is 0, a random available port will be selected.</span></span> <span data-ttu-id="93f99-320">有效值为0至65535</span><span class="sxs-lookup"><span data-stu-id="93f99-320">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="93f99-321">关系</span><span class="sxs-lookup"><span data-stu-id="93f99-321">Relationships</span></span>
|<span data-ttu-id="93f99-322">关系</span><span class="sxs-lookup"><span data-stu-id="93f99-322">Relationship</span></span>|<span data-ttu-id="93f99-323">类型</span><span class="sxs-lookup"><span data-stu-id="93f99-323">Type</span></span>|<span data-ttu-id="93f99-324">说明</span><span class="sxs-lookup"><span data-stu-id="93f99-324">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93f99-325">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="93f99-325">groupAssignments</span></span>|<span data-ttu-id="93f99-326">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="93f99-326">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="93f99-327">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="93f99-327">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="93f99-328">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-328">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-329">assignments</span><span class="sxs-lookup"><span data-stu-id="93f99-329">assignments</span></span>|<span data-ttu-id="93f99-330">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="93f99-330">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="93f99-331">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="93f99-331">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="93f99-332">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-332">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-333">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="93f99-333">deviceStatuses</span></span>|<span data-ttu-id="93f99-334">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="93f99-334">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="93f99-335">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="93f99-335">Device configuration installation status by device.</span></span> <span data-ttu-id="93f99-336">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-336">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-337">userStatuses</span><span class="sxs-lookup"><span data-stu-id="93f99-337">userStatuses</span></span>|<span data-ttu-id="93f99-338">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="93f99-338">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="93f99-339">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="93f99-339">Device configuration installation status by user.</span></span> <span data-ttu-id="93f99-340">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-340">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-341">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="93f99-341">deviceStatusOverview</span></span>|[<span data-ttu-id="93f99-342">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="93f99-342">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="93f99-343">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-343">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-344">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="93f99-344">userStatusOverview</span></span>|[<span data-ttu-id="93f99-345">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="93f99-345">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="93f99-346">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-346">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-347">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="93f99-347">deviceSettingStateSummaries</span></span>|<span data-ttu-id="93f99-348">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="93f99-348">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="93f99-349">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93f99-349">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93f99-350">singleSignOnExtensionPkinitCertificate</span><span class="sxs-lookup"><span data-stu-id="93f99-350">singleSignOnExtensionPkinitCertificate</span></span>|[<span data-ttu-id="93f99-351">macOSCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="93f99-351">macOSCertificateProfileBase</span></span>](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|<span data-ttu-id="93f99-352">用于使用单一登录扩展的身份验证的 PKINIT 证书。</span><span class="sxs-lookup"><span data-stu-id="93f99-352">PKINIT Certificate for the authentication with single sign-on extensions.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93f99-353">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93f99-353">JSON Representation</span></span>
<span data-ttu-id="93f99-354">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93f99-354">Here is a JSON representation of the resource.</span></span>
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



