---
title: 更新 macOSDeviceFeaturesConfiguration
description: 更新 macOSDeviceFeaturesConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d3d583d894a11edc6d95a95f2b1869b08467689
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804317"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="77676-103">更新 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="77676-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="77676-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="77676-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77676-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77676-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77676-106">更新 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="77676-106">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77676-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="77676-107">Prerequisites</span></span>
<span data-ttu-id="77676-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77676-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77676-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="77676-110">Permission type</span></span>|<span data-ttu-id="77676-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="77676-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77676-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77676-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77676-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77676-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77676-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77676-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77676-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="77676-115">Not supported.</span></span>|
|<span data-ttu-id="77676-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="77676-116">Application</span></span>|<span data-ttu-id="77676-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="77676-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77676-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77676-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="77676-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="77676-119">Request headers</span></span>
|<span data-ttu-id="77676-120">标头</span><span class="sxs-lookup"><span data-stu-id="77676-120">Header</span></span>|<span data-ttu-id="77676-121">值</span><span class="sxs-lookup"><span data-stu-id="77676-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77676-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="77676-122">Authorization</span></span>|<span data-ttu-id="77676-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="77676-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77676-124">接受</span><span class="sxs-lookup"><span data-stu-id="77676-124">Accept</span></span>|<span data-ttu-id="77676-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77676-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77676-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="77676-126">Request body</span></span>
<span data-ttu-id="77676-127">在请求正文中，提供 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77676-127">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="77676-128">下表显示创建 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="77676-128">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="77676-129">属性</span><span class="sxs-lookup"><span data-stu-id="77676-129">Property</span></span>|<span data-ttu-id="77676-130">类型</span><span class="sxs-lookup"><span data-stu-id="77676-130">Type</span></span>|<span data-ttu-id="77676-131">说明</span><span class="sxs-lookup"><span data-stu-id="77676-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77676-132">id</span><span class="sxs-lookup"><span data-stu-id="77676-132">id</span></span>|<span data-ttu-id="77676-133">String</span><span class="sxs-lookup"><span data-stu-id="77676-133">String</span></span>|<span data-ttu-id="77676-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="77676-134">Key of the entity.</span></span> <span data-ttu-id="77676-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77676-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77676-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77676-136">lastModifiedDateTime</span></span>|<span data-ttu-id="77676-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77676-137">DateTimeOffset</span></span>|<span data-ttu-id="77676-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="77676-138">DateTime the object was last modified.</span></span> <span data-ttu-id="77676-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77676-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77676-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="77676-140">roleScopeTagIds</span></span>|<span data-ttu-id="77676-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="77676-141">String collection</span></span>|<span data-ttu-id="77676-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="77676-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="77676-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77676-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77676-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="77676-144">supportsScopeTags</span></span>|<span data-ttu-id="77676-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="77676-145">Boolean</span></span>|<span data-ttu-id="77676-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="77676-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="77676-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="77676-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="77676-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="77676-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="77676-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="77676-149">This property is read-only.</span></span> <span data-ttu-id="77676-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77676-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77676-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77676-151">createdDateTime</span></span>|<span data-ttu-id="77676-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77676-152">DateTimeOffset</span></span>|<span data-ttu-id="77676-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="77676-153">DateTime the object was created.</span></span> <span data-ttu-id="77676-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77676-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77676-155">description</span><span class="sxs-lookup"><span data-stu-id="77676-155">description</span></span>|<span data-ttu-id="77676-156">String</span><span class="sxs-lookup"><span data-stu-id="77676-156">String</span></span>|<span data-ttu-id="77676-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="77676-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="77676-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77676-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77676-159">displayName</span><span class="sxs-lookup"><span data-stu-id="77676-159">displayName</span></span>|<span data-ttu-id="77676-160">String</span><span class="sxs-lookup"><span data-stu-id="77676-160">String</span></span>|<span data-ttu-id="77676-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="77676-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="77676-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77676-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77676-163">version</span><span class="sxs-lookup"><span data-stu-id="77676-163">version</span></span>|<span data-ttu-id="77676-164">Int32</span><span class="sxs-lookup"><span data-stu-id="77676-164">Int32</span></span>|<span data-ttu-id="77676-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="77676-165">Version of the device configuration.</span></span> <span data-ttu-id="77676-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77676-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77676-167">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="77676-167">airPrintDestinations</span></span>|<span data-ttu-id="77676-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)集合</span><span class="sxs-lookup"><span data-stu-id="77676-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="77676-169">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="77676-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="77676-170">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="77676-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="77676-171">继承自[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="77676-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="77676-172">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="77676-172">autoLaunchItems</span></span>|<span data-ttu-id="77676-173">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="77676-173">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="77676-174">用户登录时要启动的应用程序、文件、文件夹和其他项目的列表。</span><span class="sxs-lookup"><span data-stu-id="77676-174">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="77676-175">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="77676-175">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="77676-176">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="77676-176">adminShowHostInfo</span></span>|<span data-ttu-id="77676-177">布尔值</span><span class="sxs-lookup"><span data-stu-id="77676-177">Boolean</span></span>|<span data-ttu-id="77676-178">是否在登录窗口中显示管理员主机信息。</span><span class="sxs-lookup"><span data-stu-id="77676-178">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="77676-179">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="77676-179">loginWindowText</span></span>|<span data-ttu-id="77676-180">String</span><span class="sxs-lookup"><span data-stu-id="77676-180">String</span></span>|<span data-ttu-id="77676-181">要在登录窗口中显示的自定义文本。</span><span class="sxs-lookup"><span data-stu-id="77676-181">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="77676-182">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="77676-182">authorizedUsersListHidden</span></span>|<span data-ttu-id="77676-183">布尔值</span><span class="sxs-lookup"><span data-stu-id="77676-183">Boolean</span></span>|<span data-ttu-id="77676-184">是否在登录窗口中显示 "名称" 和 "密码" 对话框或用户列表。</span><span class="sxs-lookup"><span data-stu-id="77676-184">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="77676-185">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="77676-185">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="77676-186">布尔值</span><span class="sxs-lookup"><span data-stu-id="77676-186">Boolean</span></span>|<span data-ttu-id="77676-187">是否在登录窗口的授权用户列表中仅显示网络和系统用户。</span><span class="sxs-lookup"><span data-stu-id="77676-187">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="77676-188">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="77676-188">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="77676-189">布尔值</span><span class="sxs-lookup"><span data-stu-id="77676-189">Boolean</span></span>|<span data-ttu-id="77676-190">是否在登录窗口上的授权用户列表中隐藏移动用户。</span><span class="sxs-lookup"><span data-stu-id="77676-190">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="77676-191">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="77676-191">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="77676-192">布尔值</span><span class="sxs-lookup"><span data-stu-id="77676-192">Boolean</span></span>|<span data-ttu-id="77676-193">是否在登录窗口上的授权用户列表中显示网络用户。</span><span class="sxs-lookup"><span data-stu-id="77676-193">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="77676-194">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="77676-194">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="77676-195">布尔值</span><span class="sxs-lookup"><span data-stu-id="77676-195">Boolean</span></span>|<span data-ttu-id="77676-196">是否在登录窗口的授权用户列表中隐藏管理员用户。</span><span class="sxs-lookup"><span data-stu-id="77676-196">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="77676-197">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="77676-197">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="77676-198">布尔值</span><span class="sxs-lookup"><span data-stu-id="77676-198">Boolean</span></span>|<span data-ttu-id="77676-199">是否在登录窗口上的授权用户列表中显示其他用户。</span><span class="sxs-lookup"><span data-stu-id="77676-199">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="77676-200">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="77676-200">shutDownDisabled</span></span>|<span data-ttu-id="77676-201">布尔值</span><span class="sxs-lookup"><span data-stu-id="77676-201">Boolean</span></span>|<span data-ttu-id="77676-202">是否在登录窗口中隐藏 "关机" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="77676-202">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="77676-203">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="77676-203">restartDisabled</span></span>|<span data-ttu-id="77676-204">布尔值</span><span class="sxs-lookup"><span data-stu-id="77676-204">Boolean</span></span>|<span data-ttu-id="77676-205">是否在登录窗口中隐藏 "重新启动" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="77676-205">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="77676-206">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="77676-206">sleepDisabled</span></span>|<span data-ttu-id="77676-207">布尔值</span><span class="sxs-lookup"><span data-stu-id="77676-207">Boolean</span></span>|<span data-ttu-id="77676-208">是否在登录窗口中隐藏 "睡眠" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="77676-208">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="77676-209">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="77676-209">consoleAccessDisabled</span></span>|<span data-ttu-id="77676-210">布尔值</span><span class="sxs-lookup"><span data-stu-id="77676-210">Boolean</span></span>|<span data-ttu-id="77676-211">其他用户是否会忽略使用 ">console>" 的专用用户名。</span><span class="sxs-lookup"><span data-stu-id="77676-211">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="77676-212">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="77676-212">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="77676-213">布尔值</span><span class="sxs-lookup"><span data-stu-id="77676-213">Boolean</span></span>|<span data-ttu-id="77676-214">用户登录时是否禁用登录窗口上的 "关闭" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="77676-214">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="77676-215">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="77676-215">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="77676-216">布尔值</span><span class="sxs-lookup"><span data-stu-id="77676-216">Boolean</span></span>|<span data-ttu-id="77676-217">用户登录时是否禁用登录窗口上的重启菜单项。</span><span class="sxs-lookup"><span data-stu-id="77676-217">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="77676-218">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="77676-218">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="77676-219">布尔值</span><span class="sxs-lookup"><span data-stu-id="77676-219">Boolean</span></span>|<span data-ttu-id="77676-220">用户登录时登录窗口上的 "断电" 菜单项是否将被禁用。</span><span class="sxs-lookup"><span data-stu-id="77676-220">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="77676-221">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="77676-221">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="77676-222">布尔值</span><span class="sxs-lookup"><span data-stu-id="77676-222">Boolean</span></span>|<span data-ttu-id="77676-223">用户登录时, 登录窗口上的注销菜单项是否会被禁用。</span><span class="sxs-lookup"><span data-stu-id="77676-223">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="77676-224">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="77676-224">screenLockDisableImmediate</span></span>|<span data-ttu-id="77676-225">布尔值</span><span class="sxs-lookup"><span data-stu-id="77676-225">Boolean</span></span>|<span data-ttu-id="77676-226">是否禁用即时屏幕锁定功能。</span><span class="sxs-lookup"><span data-stu-id="77676-226">Whether to disable the immediate screen lock functions.</span></span>|



## <a name="response"></a><span data-ttu-id="77676-227">响应</span><span class="sxs-lookup"><span data-stu-id="77676-227">Response</span></span>
<span data-ttu-id="77676-228">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="77676-228">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77676-229">示例</span><span class="sxs-lookup"><span data-stu-id="77676-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="77676-230">请求</span><span class="sxs-lookup"><span data-stu-id="77676-230">Request</span></span>
<span data-ttu-id="77676-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="77676-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1334

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "screenLockDisableImmediate": true
}
```

### <a name="response"></a><span data-ttu-id="77676-232">响应</span><span class="sxs-lookup"><span data-stu-id="77676-232">Response</span></span>
<span data-ttu-id="77676-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77676-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1506

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "screenLockDisableImmediate": true
}
```





