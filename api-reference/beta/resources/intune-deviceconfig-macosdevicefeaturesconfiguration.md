---
title: macOSDeviceFeaturesConfiguration 资源类型
description: MacOS 设备功能配置的配置文件。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 52b0a83dde3986d17f9ff09b41076edd7e9e9041
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179219"
---
# <a name="macosdevicefeaturesconfiguration-resource-type"></a><span data-ttu-id="0c24b-103">macOSDeviceFeaturesConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c24b-103">macOSDeviceFeaturesConfiguration resource type</span></span>

<span data-ttu-id="0c24b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c24b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c24b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0c24b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c24b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0c24b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c24b-107">MacOS 设备功能配置的配置文件。</span><span class="sxs-lookup"><span data-stu-id="0c24b-107">MacOS device features configuration profile.</span></span>


<span data-ttu-id="0c24b-108">继承自 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-108">Inherits from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0c24b-109">方法</span><span class="sxs-lookup"><span data-stu-id="0c24b-109">Methods</span></span>
|<span data-ttu-id="0c24b-110">方法</span><span class="sxs-lookup"><span data-stu-id="0c24b-110">Method</span></span>|<span data-ttu-id="0c24b-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="0c24b-111">Return Type</span></span>|<span data-ttu-id="0c24b-112">说明</span><span class="sxs-lookup"><span data-stu-id="0c24b-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0c24b-113">列出 macOSDeviceFeaturesConfigurations</span><span class="sxs-lookup"><span data-stu-id="0c24b-113">List macOSDeviceFeaturesConfigurations</span></span>](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-list.md)|<span data-ttu-id="0c24b-114">[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0c24b-114">[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) collection</span></span>|<span data-ttu-id="0c24b-115">列出 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0c24b-115">List properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="0c24b-116">获取 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c24b-116">Get macOSDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-get.md)|[<span data-ttu-id="0c24b-117">macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c24b-117">macOSDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|<span data-ttu-id="0c24b-118">读取 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0c24b-118">Read properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>|
|[<span data-ttu-id="0c24b-119">创建 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c24b-119">Create macOSDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-create.md)|[<span data-ttu-id="0c24b-120">macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c24b-120">macOSDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|<span data-ttu-id="0c24b-121">创建新的 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c24b-121">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>|
|[<span data-ttu-id="0c24b-122">删除 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c24b-122">Delete macOSDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-delete.md)|<span data-ttu-id="0c24b-123">无</span><span class="sxs-lookup"><span data-stu-id="0c24b-123">None</span></span>|<span data-ttu-id="0c24b-124">删除 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="0c24b-124">Deletes a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>|
|[<span data-ttu-id="0c24b-125">更新 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c24b-125">Update macOSDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-update.md)|[<span data-ttu-id="0c24b-126">macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c24b-126">macOSDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|<span data-ttu-id="0c24b-127">更新 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0c24b-127">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0c24b-128">属性</span><span class="sxs-lookup"><span data-stu-id="0c24b-128">Properties</span></span>
|<span data-ttu-id="0c24b-129">属性</span><span class="sxs-lookup"><span data-stu-id="0c24b-129">Property</span></span>|<span data-ttu-id="0c24b-130">类型</span><span class="sxs-lookup"><span data-stu-id="0c24b-130">Type</span></span>|<span data-ttu-id="0c24b-131">说明</span><span class="sxs-lookup"><span data-stu-id="0c24b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c24b-132">id</span><span class="sxs-lookup"><span data-stu-id="0c24b-132">id</span></span>|<span data-ttu-id="0c24b-133">字符串</span><span class="sxs-lookup"><span data-stu-id="0c24b-133">String</span></span>|<span data-ttu-id="0c24b-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0c24b-134">Key of the entity.</span></span> <span data-ttu-id="0c24b-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c24b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0c24b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c24b-137">DateTimeOffset</span></span>|<span data-ttu-id="0c24b-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0c24b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0c24b-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0c24b-140">roleScopeTagIds</span></span>|<span data-ttu-id="0c24b-141">字符串集合</span><span class="sxs-lookup"><span data-stu-id="0c24b-141">String collection</span></span>|<span data-ttu-id="0c24b-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0c24b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0c24b-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0c24b-144">supportsScopeTags</span></span>|<span data-ttu-id="0c24b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c24b-145">Boolean</span></span>|<span data-ttu-id="0c24b-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="0c24b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0c24b-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="0c24b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0c24b-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="0c24b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0c24b-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0c24b-149">This property is read-only.</span></span> <span data-ttu-id="0c24b-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0c24b-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0c24b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0c24b-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0c24b-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="0c24b-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0c24b-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0c24b-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0c24b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0c24b-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0c24b-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0c24b-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0c24b-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0c24b-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0c24b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0c24b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0c24b-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0c24b-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0c24b-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c24b-163">createdDateTime</span></span>|<span data-ttu-id="0c24b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c24b-164">DateTimeOffset</span></span>|<span data-ttu-id="0c24b-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0c24b-165">DateTime the object was created.</span></span> <span data-ttu-id="0c24b-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-167">说明</span><span class="sxs-lookup"><span data-stu-id="0c24b-167">description</span></span>|<span data-ttu-id="0c24b-168">String</span><span class="sxs-lookup"><span data-stu-id="0c24b-168">String</span></span>|<span data-ttu-id="0c24b-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0c24b-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0c24b-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-171">displayName</span><span class="sxs-lookup"><span data-stu-id="0c24b-171">displayName</span></span>|<span data-ttu-id="0c24b-172">String</span><span class="sxs-lookup"><span data-stu-id="0c24b-172">String</span></span>|<span data-ttu-id="0c24b-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0c24b-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0c24b-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-175">version</span><span class="sxs-lookup"><span data-stu-id="0c24b-175">version</span></span>|<span data-ttu-id="0c24b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0c24b-176">Int32</span></span>|<span data-ttu-id="0c24b-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0c24b-177">Version of the device configuration.</span></span> <span data-ttu-id="0c24b-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-179">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="0c24b-179">airPrintDestinations</span></span>|<span data-ttu-id="0c24b-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)集合</span><span class="sxs-lookup"><span data-stu-id="0c24b-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="0c24b-181">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="0c24b-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="0c24b-182">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0c24b-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0c24b-183">继承自[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="0c24b-184">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="0c24b-184">autoLaunchItems</span></span>|<span data-ttu-id="0c24b-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="0c24b-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="0c24b-186">用户登录时要启动的应用程序、文件、文件夹和其他项目的列表。</span><span class="sxs-lookup"><span data-stu-id="0c24b-186">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="0c24b-187">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0c24b-187">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0c24b-188">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="0c24b-188">adminShowHostInfo</span></span>|<span data-ttu-id="0c24b-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c24b-189">Boolean</span></span>|<span data-ttu-id="0c24b-190">是否在登录窗口中显示管理员主机信息。</span><span class="sxs-lookup"><span data-stu-id="0c24b-190">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="0c24b-191">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="0c24b-191">loginWindowText</span></span>|<span data-ttu-id="0c24b-192">字符串</span><span class="sxs-lookup"><span data-stu-id="0c24b-192">String</span></span>|<span data-ttu-id="0c24b-193">要在登录窗口中显示的自定义文本。</span><span class="sxs-lookup"><span data-stu-id="0c24b-193">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="0c24b-194">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="0c24b-194">authorizedUsersListHidden</span></span>|<span data-ttu-id="0c24b-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c24b-195">Boolean</span></span>|<span data-ttu-id="0c24b-196">是否在登录窗口中显示 "名称" 和 "密码" 对话框或用户列表。</span><span class="sxs-lookup"><span data-stu-id="0c24b-196">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="0c24b-197">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="0c24b-197">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="0c24b-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c24b-198">Boolean</span></span>|<span data-ttu-id="0c24b-199">是否在登录窗口的授权用户列表中仅显示网络和系统用户。</span><span class="sxs-lookup"><span data-stu-id="0c24b-199">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="0c24b-200">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="0c24b-200">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="0c24b-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c24b-201">Boolean</span></span>|<span data-ttu-id="0c24b-202">是否在登录窗口上的授权用户列表中隐藏移动用户。</span><span class="sxs-lookup"><span data-stu-id="0c24b-202">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="0c24b-203">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="0c24b-203">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="0c24b-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c24b-204">Boolean</span></span>|<span data-ttu-id="0c24b-205">是否在登录窗口上的授权用户列表中显示网络用户。</span><span class="sxs-lookup"><span data-stu-id="0c24b-205">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="0c24b-206">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="0c24b-206">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="0c24b-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c24b-207">Boolean</span></span>|<span data-ttu-id="0c24b-208">是否在登录窗口的授权用户列表中隐藏管理员用户。</span><span class="sxs-lookup"><span data-stu-id="0c24b-208">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="0c24b-209">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="0c24b-209">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="0c24b-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c24b-210">Boolean</span></span>|<span data-ttu-id="0c24b-211">是否在登录窗口上的授权用户列表中显示其他用户。</span><span class="sxs-lookup"><span data-stu-id="0c24b-211">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="0c24b-212">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="0c24b-212">shutDownDisabled</span></span>|<span data-ttu-id="0c24b-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c24b-213">Boolean</span></span>|<span data-ttu-id="0c24b-214">是否在登录窗口中隐藏 "关机" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="0c24b-214">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="0c24b-215">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="0c24b-215">restartDisabled</span></span>|<span data-ttu-id="0c24b-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c24b-216">Boolean</span></span>|<span data-ttu-id="0c24b-217">是否在登录窗口中隐藏 "重新启动" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="0c24b-217">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="0c24b-218">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="0c24b-218">sleepDisabled</span></span>|<span data-ttu-id="0c24b-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c24b-219">Boolean</span></span>|<span data-ttu-id="0c24b-220">是否在登录窗口中隐藏 "睡眠" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="0c24b-220">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="0c24b-221">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="0c24b-221">consoleAccessDisabled</span></span>|<span data-ttu-id="0c24b-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c24b-222">Boolean</span></span>|<span data-ttu-id="0c24b-223">其他用户是否会忽略使用 ">控制台> 特殊用户名。</span><span class="sxs-lookup"><span data-stu-id="0c24b-223">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="0c24b-224">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="0c24b-224">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="0c24b-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c24b-225">Boolean</span></span>|<span data-ttu-id="0c24b-226">用户登录时是否禁用登录窗口上的 "关闭" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="0c24b-226">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="0c24b-227">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="0c24b-227">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="0c24b-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c24b-228">Boolean</span></span>|<span data-ttu-id="0c24b-229">用户登录时是否禁用登录窗口上的重启菜单项。</span><span class="sxs-lookup"><span data-stu-id="0c24b-229">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="0c24b-230">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="0c24b-230">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="0c24b-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c24b-231">Boolean</span></span>|<span data-ttu-id="0c24b-232">用户登录时登录窗口上的 "断电" 菜单项是否将被禁用。</span><span class="sxs-lookup"><span data-stu-id="0c24b-232">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="0c24b-233">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="0c24b-233">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="0c24b-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c24b-234">Boolean</span></span>|<span data-ttu-id="0c24b-235">用户登录时，登录窗口上的注销菜单项是否会被禁用。</span><span class="sxs-lookup"><span data-stu-id="0c24b-235">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="0c24b-236">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="0c24b-236">screenLockDisableImmediate</span></span>|<span data-ttu-id="0c24b-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c24b-237">Boolean</span></span>|<span data-ttu-id="0c24b-238">是否禁用即时屏幕锁定功能。</span><span class="sxs-lookup"><span data-stu-id="0c24b-238">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="0c24b-239">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="0c24b-239">associatedDomains</span></span>|<span data-ttu-id="0c24b-240">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0c24b-240">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0c24b-241">获取或设置一个列表，该列表将应用程序映射到其关联的域。</span><span class="sxs-lookup"><span data-stu-id="0c24b-241">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="0c24b-242">该密钥应与应用程序的 ID 匹配，并且值应为 "服务：域" 形式的字符串，其中 domain 是完全限定的主机名（例如 webcredentials:example）。</span><span class="sxs-lookup"><span data-stu-id="0c24b-242">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="0c24b-243">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0c24b-243">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0c24b-244">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="0c24b-244">singleSignOnExtension</span></span>|[<span data-ttu-id="0c24b-245">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="0c24b-245">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="0c24b-246">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="0c24b-246">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="0c24b-247">弃用：改用 MacOSSingleSignOnExtension。</span><span class="sxs-lookup"><span data-stu-id="0c24b-247">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="0c24b-248">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="0c24b-248">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="0c24b-249">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="0c24b-249">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="0c24b-250">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="0c24b-250">Gets or sets a single sign-on extension profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c24b-251">关系</span><span class="sxs-lookup"><span data-stu-id="0c24b-251">Relationships</span></span>
|<span data-ttu-id="0c24b-252">关系</span><span class="sxs-lookup"><span data-stu-id="0c24b-252">Relationship</span></span>|<span data-ttu-id="0c24b-253">类型</span><span class="sxs-lookup"><span data-stu-id="0c24b-253">Type</span></span>|<span data-ttu-id="0c24b-254">说明</span><span class="sxs-lookup"><span data-stu-id="0c24b-254">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c24b-255">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="0c24b-255">groupAssignments</span></span>|<span data-ttu-id="0c24b-256">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="0c24b-256">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="0c24b-257">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="0c24b-257">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="0c24b-258">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-258">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-259">assignments</span><span class="sxs-lookup"><span data-stu-id="0c24b-259">assignments</span></span>|<span data-ttu-id="0c24b-260">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0c24b-260">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0c24b-261">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="0c24b-261">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="0c24b-262">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-262">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-263">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="0c24b-263">deviceStatuses</span></span>|<span data-ttu-id="0c24b-264">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0c24b-264">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="0c24b-265">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="0c24b-265">Device configuration installation status by device.</span></span> <span data-ttu-id="0c24b-266">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-266">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-267">userStatuses</span><span class="sxs-lookup"><span data-stu-id="0c24b-267">userStatuses</span></span>|<span data-ttu-id="0c24b-268">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0c24b-268">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="0c24b-269">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="0c24b-269">Device configuration installation status by user.</span></span> <span data-ttu-id="0c24b-270">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-270">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-271">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0c24b-271">deviceStatusOverview</span></span>|[<span data-ttu-id="0c24b-272">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0c24b-272">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="0c24b-273">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-273">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-274">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0c24b-274">userStatusOverview</span></span>|[<span data-ttu-id="0c24b-275">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="0c24b-275">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="0c24b-276">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-276">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-277">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="0c24b-277">deviceSettingStateSummaries</span></span>|<span data-ttu-id="0c24b-278">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0c24b-278">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="0c24b-279">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c24b-279">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c24b-280">singleSignOnExtensionPkinitCertificate</span><span class="sxs-lookup"><span data-stu-id="0c24b-280">singleSignOnExtensionPkinitCertificate</span></span>|[<span data-ttu-id="0c24b-281">macOSCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="0c24b-281">macOSCertificateProfileBase</span></span>](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|<span data-ttu-id="0c24b-282">用于使用单一登录扩展的身份验证的 PKINIT 证书。</span><span class="sxs-lookup"><span data-stu-id="0c24b-282">PKINIT Certificate for the authentication with single sign-on extensions.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c24b-283">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c24b-283">JSON Representation</span></span>
<span data-ttu-id="0c24b-284">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c24b-284">Here is a JSON representation of the resource.</span></span>
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
  }
}
```



