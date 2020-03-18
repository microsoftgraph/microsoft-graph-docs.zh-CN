---
title: 创建 macOSDeviceFeaturesConfiguration
description: 创建新的 macOSDeviceFeaturesConfiguration 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 509487d54dfa2d7f5041214bd79ca1d144a8bc28
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42747023"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="408fc-103">创建 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="408fc-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="408fc-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="408fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="408fc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="408fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="408fc-106">创建新的 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="408fc-106">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="408fc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="408fc-107">Prerequisites</span></span>
<span data-ttu-id="408fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="408fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="408fc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="408fc-110">Permission type</span></span>|<span data-ttu-id="408fc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="408fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="408fc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="408fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="408fc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="408fc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="408fc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="408fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="408fc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="408fc-115">Not supported.</span></span>|
|<span data-ttu-id="408fc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="408fc-116">Application</span></span>|<span data-ttu-id="408fc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="408fc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="408fc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="408fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="408fc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="408fc-119">Request headers</span></span>
|<span data-ttu-id="408fc-120">标头</span><span class="sxs-lookup"><span data-stu-id="408fc-120">Header</span></span>|<span data-ttu-id="408fc-121">值</span><span class="sxs-lookup"><span data-stu-id="408fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="408fc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="408fc-122">Authorization</span></span>|<span data-ttu-id="408fc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="408fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="408fc-124">接受</span><span class="sxs-lookup"><span data-stu-id="408fc-124">Accept</span></span>|<span data-ttu-id="408fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="408fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="408fc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="408fc-126">Request body</span></span>
<span data-ttu-id="408fc-127">在请求正文中，提供 macOSDeviceFeaturesConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="408fc-127">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="408fc-128">下表显示创建 macOSDeviceFeaturesConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="408fc-128">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="408fc-129">属性</span><span class="sxs-lookup"><span data-stu-id="408fc-129">Property</span></span>|<span data-ttu-id="408fc-130">类型</span><span class="sxs-lookup"><span data-stu-id="408fc-130">Type</span></span>|<span data-ttu-id="408fc-131">说明</span><span class="sxs-lookup"><span data-stu-id="408fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="408fc-132">id</span><span class="sxs-lookup"><span data-stu-id="408fc-132">id</span></span>|<span data-ttu-id="408fc-133">字符串</span><span class="sxs-lookup"><span data-stu-id="408fc-133">String</span></span>|<span data-ttu-id="408fc-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="408fc-134">Key of the entity.</span></span> <span data-ttu-id="408fc-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="408fc-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="408fc-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="408fc-136">lastModifiedDateTime</span></span>|<span data-ttu-id="408fc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="408fc-137">DateTimeOffset</span></span>|<span data-ttu-id="408fc-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="408fc-138">DateTime the object was last modified.</span></span> <span data-ttu-id="408fc-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="408fc-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="408fc-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="408fc-140">roleScopeTagIds</span></span>|<span data-ttu-id="408fc-141">String collection</span><span class="sxs-lookup"><span data-stu-id="408fc-141">String collection</span></span>|<span data-ttu-id="408fc-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="408fc-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="408fc-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="408fc-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="408fc-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="408fc-144">supportsScopeTags</span></span>|<span data-ttu-id="408fc-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="408fc-145">Boolean</span></span>|<span data-ttu-id="408fc-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="408fc-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="408fc-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="408fc-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="408fc-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="408fc-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="408fc-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="408fc-149">This property is read-only.</span></span> <span data-ttu-id="408fc-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="408fc-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="408fc-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="408fc-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="408fc-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="408fc-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="408fc-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="408fc-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="408fc-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="408fc-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="408fc-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="408fc-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="408fc-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="408fc-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="408fc-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="408fc-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="408fc-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="408fc-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="408fc-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="408fc-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="408fc-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="408fc-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="408fc-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="408fc-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="408fc-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="408fc-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="408fc-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="408fc-163">createdDateTime</span></span>|<span data-ttu-id="408fc-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="408fc-164">DateTimeOffset</span></span>|<span data-ttu-id="408fc-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="408fc-165">DateTime the object was created.</span></span> <span data-ttu-id="408fc-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="408fc-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="408fc-167">说明</span><span class="sxs-lookup"><span data-stu-id="408fc-167">description</span></span>|<span data-ttu-id="408fc-168">String</span><span class="sxs-lookup"><span data-stu-id="408fc-168">String</span></span>|<span data-ttu-id="408fc-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="408fc-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="408fc-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="408fc-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="408fc-171">displayName</span><span class="sxs-lookup"><span data-stu-id="408fc-171">displayName</span></span>|<span data-ttu-id="408fc-172">String</span><span class="sxs-lookup"><span data-stu-id="408fc-172">String</span></span>|<span data-ttu-id="408fc-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="408fc-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="408fc-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="408fc-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="408fc-175">version</span><span class="sxs-lookup"><span data-stu-id="408fc-175">version</span></span>|<span data-ttu-id="408fc-176">Int32</span><span class="sxs-lookup"><span data-stu-id="408fc-176">Int32</span></span>|<span data-ttu-id="408fc-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="408fc-177">Version of the device configuration.</span></span> <span data-ttu-id="408fc-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="408fc-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="408fc-179">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="408fc-179">airPrintDestinations</span></span>|<span data-ttu-id="408fc-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)集合</span><span class="sxs-lookup"><span data-stu-id="408fc-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="408fc-181">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="408fc-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="408fc-182">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="408fc-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="408fc-183">继承自[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="408fc-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="408fc-184">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="408fc-184">autoLaunchItems</span></span>|<span data-ttu-id="408fc-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="408fc-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="408fc-186">用户登录时要启动的应用程序、文件、文件夹和其他项目的列表。</span><span class="sxs-lookup"><span data-stu-id="408fc-186">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="408fc-187">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="408fc-187">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="408fc-188">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="408fc-188">adminShowHostInfo</span></span>|<span data-ttu-id="408fc-189">布尔值</span><span class="sxs-lookup"><span data-stu-id="408fc-189">Boolean</span></span>|<span data-ttu-id="408fc-190">是否在登录窗口中显示管理员主机信息。</span><span class="sxs-lookup"><span data-stu-id="408fc-190">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="408fc-191">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="408fc-191">loginWindowText</span></span>|<span data-ttu-id="408fc-192">String</span><span class="sxs-lookup"><span data-stu-id="408fc-192">String</span></span>|<span data-ttu-id="408fc-193">要在登录窗口中显示的自定义文本。</span><span class="sxs-lookup"><span data-stu-id="408fc-193">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="408fc-194">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="408fc-194">authorizedUsersListHidden</span></span>|<span data-ttu-id="408fc-195">布尔值</span><span class="sxs-lookup"><span data-stu-id="408fc-195">Boolean</span></span>|<span data-ttu-id="408fc-196">是否在登录窗口中显示 "名称" 和 "密码" 对话框或用户列表。</span><span class="sxs-lookup"><span data-stu-id="408fc-196">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="408fc-197">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="408fc-197">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="408fc-198">布尔值</span><span class="sxs-lookup"><span data-stu-id="408fc-198">Boolean</span></span>|<span data-ttu-id="408fc-199">是否在登录窗口的授权用户列表中仅显示网络和系统用户。</span><span class="sxs-lookup"><span data-stu-id="408fc-199">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="408fc-200">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="408fc-200">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="408fc-201">布尔值</span><span class="sxs-lookup"><span data-stu-id="408fc-201">Boolean</span></span>|<span data-ttu-id="408fc-202">是否在登录窗口上的授权用户列表中隐藏移动用户。</span><span class="sxs-lookup"><span data-stu-id="408fc-202">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="408fc-203">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="408fc-203">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="408fc-204">布尔值</span><span class="sxs-lookup"><span data-stu-id="408fc-204">Boolean</span></span>|<span data-ttu-id="408fc-205">是否在登录窗口上的授权用户列表中显示网络用户。</span><span class="sxs-lookup"><span data-stu-id="408fc-205">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="408fc-206">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="408fc-206">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="408fc-207">布尔值</span><span class="sxs-lookup"><span data-stu-id="408fc-207">Boolean</span></span>|<span data-ttu-id="408fc-208">是否在登录窗口的授权用户列表中隐藏管理员用户。</span><span class="sxs-lookup"><span data-stu-id="408fc-208">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="408fc-209">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="408fc-209">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="408fc-210">布尔值</span><span class="sxs-lookup"><span data-stu-id="408fc-210">Boolean</span></span>|<span data-ttu-id="408fc-211">是否在登录窗口上的授权用户列表中显示其他用户。</span><span class="sxs-lookup"><span data-stu-id="408fc-211">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="408fc-212">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="408fc-212">shutDownDisabled</span></span>|<span data-ttu-id="408fc-213">布尔值</span><span class="sxs-lookup"><span data-stu-id="408fc-213">Boolean</span></span>|<span data-ttu-id="408fc-214">是否在登录窗口中隐藏 "关机" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="408fc-214">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="408fc-215">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="408fc-215">restartDisabled</span></span>|<span data-ttu-id="408fc-216">布尔值</span><span class="sxs-lookup"><span data-stu-id="408fc-216">Boolean</span></span>|<span data-ttu-id="408fc-217">是否在登录窗口中隐藏 "重新启动" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="408fc-217">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="408fc-218">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="408fc-218">sleepDisabled</span></span>|<span data-ttu-id="408fc-219">布尔值</span><span class="sxs-lookup"><span data-stu-id="408fc-219">Boolean</span></span>|<span data-ttu-id="408fc-220">是否在登录窗口中隐藏 "睡眠" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="408fc-220">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="408fc-221">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="408fc-221">consoleAccessDisabled</span></span>|<span data-ttu-id="408fc-222">布尔值</span><span class="sxs-lookup"><span data-stu-id="408fc-222">Boolean</span></span>|<span data-ttu-id="408fc-223">其他用户是否会忽略使用 ">控制台> 特殊用户名。</span><span class="sxs-lookup"><span data-stu-id="408fc-223">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="408fc-224">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="408fc-224">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="408fc-225">布尔值</span><span class="sxs-lookup"><span data-stu-id="408fc-225">Boolean</span></span>|<span data-ttu-id="408fc-226">用户登录时是否禁用登录窗口上的 "关闭" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="408fc-226">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="408fc-227">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="408fc-227">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="408fc-228">布尔值</span><span class="sxs-lookup"><span data-stu-id="408fc-228">Boolean</span></span>|<span data-ttu-id="408fc-229">用户登录时是否禁用登录窗口上的重启菜单项。</span><span class="sxs-lookup"><span data-stu-id="408fc-229">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="408fc-230">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="408fc-230">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="408fc-231">布尔值</span><span class="sxs-lookup"><span data-stu-id="408fc-231">Boolean</span></span>|<span data-ttu-id="408fc-232">用户登录时登录窗口上的 "断电" 菜单项是否将被禁用。</span><span class="sxs-lookup"><span data-stu-id="408fc-232">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="408fc-233">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="408fc-233">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="408fc-234">布尔值</span><span class="sxs-lookup"><span data-stu-id="408fc-234">Boolean</span></span>|<span data-ttu-id="408fc-235">用户登录时，登录窗口上的注销菜单项是否会被禁用。</span><span class="sxs-lookup"><span data-stu-id="408fc-235">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="408fc-236">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="408fc-236">screenLockDisableImmediate</span></span>|<span data-ttu-id="408fc-237">布尔值</span><span class="sxs-lookup"><span data-stu-id="408fc-237">Boolean</span></span>|<span data-ttu-id="408fc-238">是否禁用即时屏幕锁定功能。</span><span class="sxs-lookup"><span data-stu-id="408fc-238">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="408fc-239">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="408fc-239">associatedDomains</span></span>|<span data-ttu-id="408fc-240">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="408fc-240">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="408fc-241">获取或设置一个列表，该列表将应用程序映射到其关联的域。</span><span class="sxs-lookup"><span data-stu-id="408fc-241">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="408fc-242">该密钥应与应用程序的 ID 匹配，并且值应为 "服务：域" 形式的字符串，其中 domain 是完全限定的主机名（例如 webcredentials:example）。</span><span class="sxs-lookup"><span data-stu-id="408fc-242">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="408fc-243">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="408fc-243">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="408fc-244">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="408fc-244">singleSignOnExtension</span></span>|[<span data-ttu-id="408fc-245">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="408fc-245">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="408fc-246">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="408fc-246">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="408fc-247">弃用：改用 MacOSSingleSignOnExtension。</span><span class="sxs-lookup"><span data-stu-id="408fc-247">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="408fc-248">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="408fc-248">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="408fc-249">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="408fc-249">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="408fc-250">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="408fc-250">Gets or sets a single sign-on extension profile.</span></span>|



## <a name="response"></a><span data-ttu-id="408fc-251">响应</span><span class="sxs-lookup"><span data-stu-id="408fc-251">Response</span></span>
<span data-ttu-id="408fc-252">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="408fc-252">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="408fc-253">示例</span><span class="sxs-lookup"><span data-stu-id="408fc-253">Example</span></span>

### <a name="request"></a><span data-ttu-id="408fc-254">请求</span><span class="sxs-lookup"><span data-stu-id="408fc-254">Request</span></span>
<span data-ttu-id="408fc-255">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="408fc-255">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2468

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "autoLaunchItems": [
    {
      "@odata.type": "microsoft.graph.macOSLaunchItem",
      "path": "Path value",
      "hide": true
    }
  ],
  "adminShowHostInfo": true,
  "loginWindowText": "Login Window Text value",
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
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.singleSignOnExtension"
  },
  "macOSSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.macOSSingleSignOnExtension"
  }
}
```

### <a name="response"></a><span data-ttu-id="408fc-256">响应</span><span class="sxs-lookup"><span data-stu-id="408fc-256">Response</span></span>
<span data-ttu-id="408fc-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="408fc-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2640

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "autoLaunchItems": [
    {
      "@odata.type": "microsoft.graph.macOSLaunchItem",
      "path": "Path value",
      "hide": true
    }
  ],
  "adminShowHostInfo": true,
  "loginWindowText": "Login Window Text value",
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
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.singleSignOnExtension"
  },
  "macOSSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.macOSSingleSignOnExtension"
  }
}
```




