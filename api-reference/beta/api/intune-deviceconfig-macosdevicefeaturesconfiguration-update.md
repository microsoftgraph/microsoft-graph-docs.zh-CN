---
title: 更新 macOSDeviceFeaturesConfiguration
description: 更新 macOSDeviceFeaturesConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a615bef0cd18ce7ef28ba71adcbe8935736846b5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43438097"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="9d622-103">更新 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="9d622-103">Update macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="9d622-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d622-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d622-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9d622-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d622-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9d622-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d622-107">更新 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9d622-107">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d622-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9d622-108">Prerequisites</span></span>
<span data-ttu-id="9d622-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d622-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d622-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d622-111">Permission type</span></span>|<span data-ttu-id="9d622-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9d622-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d622-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d622-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d622-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d622-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9d622-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d622-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d622-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d622-116">Not supported.</span></span>|
|<span data-ttu-id="9d622-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d622-117">Application</span></span>|<span data-ttu-id="9d622-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d622-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d622-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d622-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9d622-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d622-120">Request headers</span></span>
|<span data-ttu-id="9d622-121">标头</span><span class="sxs-lookup"><span data-stu-id="9d622-121">Header</span></span>|<span data-ttu-id="9d622-122">值</span><span class="sxs-lookup"><span data-stu-id="9d622-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d622-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d622-123">Authorization</span></span>|<span data-ttu-id="9d622-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9d622-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d622-125">接受</span><span class="sxs-lookup"><span data-stu-id="9d622-125">Accept</span></span>|<span data-ttu-id="9d622-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d622-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d622-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d622-127">Request body</span></span>
<span data-ttu-id="9d622-128">在请求正文中，提供 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d622-128">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="9d622-129">下表显示创建 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9d622-129">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="9d622-130">属性</span><span class="sxs-lookup"><span data-stu-id="9d622-130">Property</span></span>|<span data-ttu-id="9d622-131">类型</span><span class="sxs-lookup"><span data-stu-id="9d622-131">Type</span></span>|<span data-ttu-id="9d622-132">说明</span><span class="sxs-lookup"><span data-stu-id="9d622-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d622-133">id</span><span class="sxs-lookup"><span data-stu-id="9d622-133">id</span></span>|<span data-ttu-id="9d622-134">字符串</span><span class="sxs-lookup"><span data-stu-id="9d622-134">String</span></span>|<span data-ttu-id="9d622-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9d622-135">Key of the entity.</span></span> <span data-ttu-id="9d622-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d622-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d622-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d622-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9d622-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d622-138">DateTimeOffset</span></span>|<span data-ttu-id="9d622-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9d622-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9d622-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d622-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d622-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9d622-141">roleScopeTagIds</span></span>|<span data-ttu-id="9d622-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="9d622-142">String collection</span></span>|<span data-ttu-id="9d622-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9d622-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9d622-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d622-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d622-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9d622-145">supportsScopeTags</span></span>|<span data-ttu-id="9d622-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d622-146">Boolean</span></span>|<span data-ttu-id="9d622-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="9d622-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9d622-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="9d622-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9d622-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="9d622-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9d622-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9d622-150">This property is read-only.</span></span> <span data-ttu-id="9d622-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d622-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d622-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9d622-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9d622-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9d622-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9d622-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9d622-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9d622-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d622-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d622-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9d622-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9d622-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9d622-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9d622-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9d622-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9d622-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d622-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d622-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9d622-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9d622-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9d622-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9d622-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9d622-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9d622-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d622-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d622-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d622-164">createdDateTime</span></span>|<span data-ttu-id="9d622-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d622-165">DateTimeOffset</span></span>|<span data-ttu-id="9d622-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9d622-166">DateTime the object was created.</span></span> <span data-ttu-id="9d622-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d622-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d622-168">description</span><span class="sxs-lookup"><span data-stu-id="9d622-168">description</span></span>|<span data-ttu-id="9d622-169">String</span><span class="sxs-lookup"><span data-stu-id="9d622-169">String</span></span>|<span data-ttu-id="9d622-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9d622-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9d622-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d622-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d622-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9d622-172">displayName</span></span>|<span data-ttu-id="9d622-173">String</span><span class="sxs-lookup"><span data-stu-id="9d622-173">String</span></span>|<span data-ttu-id="9d622-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9d622-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9d622-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d622-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d622-176">version</span><span class="sxs-lookup"><span data-stu-id="9d622-176">version</span></span>|<span data-ttu-id="9d622-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9d622-177">Int32</span></span>|<span data-ttu-id="9d622-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9d622-178">Version of the device configuration.</span></span> <span data-ttu-id="9d622-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d622-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d622-180">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="9d622-180">airPrintDestinations</span></span>|<span data-ttu-id="9d622-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d622-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="9d622-182">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="9d622-182">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="9d622-183">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="9d622-183">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="9d622-184">继承自[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="9d622-184">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="9d622-185">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="9d622-185">autoLaunchItems</span></span>|<span data-ttu-id="9d622-186">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d622-186">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="9d622-187">用户登录时要启动的应用程序、文件、文件夹和其他项目的列表。</span><span class="sxs-lookup"><span data-stu-id="9d622-187">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="9d622-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="9d622-188">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9d622-189">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="9d622-189">adminShowHostInfo</span></span>|<span data-ttu-id="9d622-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d622-190">Boolean</span></span>|<span data-ttu-id="9d622-191">是否在登录窗口中显示管理员主机信息。</span><span class="sxs-lookup"><span data-stu-id="9d622-191">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="9d622-192">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="9d622-192">loginWindowText</span></span>|<span data-ttu-id="9d622-193">String</span><span class="sxs-lookup"><span data-stu-id="9d622-193">String</span></span>|<span data-ttu-id="9d622-194">要在登录窗口中显示的自定义文本。</span><span class="sxs-lookup"><span data-stu-id="9d622-194">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="9d622-195">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="9d622-195">authorizedUsersListHidden</span></span>|<span data-ttu-id="9d622-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d622-196">Boolean</span></span>|<span data-ttu-id="9d622-197">是否在登录窗口中显示 "名称" 和 "密码" 对话框或用户列表。</span><span class="sxs-lookup"><span data-stu-id="9d622-197">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="9d622-198">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="9d622-198">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="9d622-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d622-199">Boolean</span></span>|<span data-ttu-id="9d622-200">是否在登录窗口的授权用户列表中仅显示网络和系统用户。</span><span class="sxs-lookup"><span data-stu-id="9d622-200">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="9d622-201">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="9d622-201">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="9d622-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d622-202">Boolean</span></span>|<span data-ttu-id="9d622-203">是否在登录窗口上的授权用户列表中隐藏移动用户。</span><span class="sxs-lookup"><span data-stu-id="9d622-203">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="9d622-204">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="9d622-204">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="9d622-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d622-205">Boolean</span></span>|<span data-ttu-id="9d622-206">是否在登录窗口上的授权用户列表中显示网络用户。</span><span class="sxs-lookup"><span data-stu-id="9d622-206">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="9d622-207">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="9d622-207">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="9d622-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d622-208">Boolean</span></span>|<span data-ttu-id="9d622-209">是否在登录窗口的授权用户列表中隐藏管理员用户。</span><span class="sxs-lookup"><span data-stu-id="9d622-209">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="9d622-210">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="9d622-210">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="9d622-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d622-211">Boolean</span></span>|<span data-ttu-id="9d622-212">是否在登录窗口上的授权用户列表中显示其他用户。</span><span class="sxs-lookup"><span data-stu-id="9d622-212">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="9d622-213">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="9d622-213">shutDownDisabled</span></span>|<span data-ttu-id="9d622-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d622-214">Boolean</span></span>|<span data-ttu-id="9d622-215">是否在登录窗口中隐藏 "关机" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="9d622-215">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="9d622-216">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="9d622-216">restartDisabled</span></span>|<span data-ttu-id="9d622-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d622-217">Boolean</span></span>|<span data-ttu-id="9d622-218">是否在登录窗口中隐藏 "重新启动" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="9d622-218">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="9d622-219">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="9d622-219">sleepDisabled</span></span>|<span data-ttu-id="9d622-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d622-220">Boolean</span></span>|<span data-ttu-id="9d622-221">是否在登录窗口中隐藏 "睡眠" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="9d622-221">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="9d622-222">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="9d622-222">consoleAccessDisabled</span></span>|<span data-ttu-id="9d622-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d622-223">Boolean</span></span>|<span data-ttu-id="9d622-224">其他用户是否会忽略使用 ">控制台> 特殊用户名。</span><span class="sxs-lookup"><span data-stu-id="9d622-224">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="9d622-225">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="9d622-225">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="9d622-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d622-226">Boolean</span></span>|<span data-ttu-id="9d622-227">用户登录时是否禁用登录窗口上的 "关闭" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="9d622-227">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="9d622-228">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="9d622-228">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="9d622-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d622-229">Boolean</span></span>|<span data-ttu-id="9d622-230">用户登录时是否禁用登录窗口上的重启菜单项。</span><span class="sxs-lookup"><span data-stu-id="9d622-230">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="9d622-231">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="9d622-231">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="9d622-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d622-232">Boolean</span></span>|<span data-ttu-id="9d622-233">用户登录时登录窗口上的 "断电" 菜单项是否将被禁用。</span><span class="sxs-lookup"><span data-stu-id="9d622-233">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="9d622-234">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="9d622-234">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="9d622-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d622-235">Boolean</span></span>|<span data-ttu-id="9d622-236">用户登录时，登录窗口上的注销菜单项是否会被禁用。</span><span class="sxs-lookup"><span data-stu-id="9d622-236">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="9d622-237">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="9d622-237">screenLockDisableImmediate</span></span>|<span data-ttu-id="9d622-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d622-238">Boolean</span></span>|<span data-ttu-id="9d622-239">是否禁用即时屏幕锁定功能。</span><span class="sxs-lookup"><span data-stu-id="9d622-239">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="9d622-240">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="9d622-240">associatedDomains</span></span>|<span data-ttu-id="9d622-241">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9d622-241">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="9d622-242">获取或设置一个列表，该列表将应用程序映射到其关联的域。</span><span class="sxs-lookup"><span data-stu-id="9d622-242">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="9d622-243">该密钥应与应用程序的 ID 匹配，并且值应为 "服务：域" 形式的字符串，其中 domain 是完全限定的主机名（例如 webcredentials:example）。</span><span class="sxs-lookup"><span data-stu-id="9d622-243">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="9d622-244">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="9d622-244">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9d622-245">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="9d622-245">singleSignOnExtension</span></span>|[<span data-ttu-id="9d622-246">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="9d622-246">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="9d622-247">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="9d622-247">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="9d622-248">弃用：改用 MacOSSingleSignOnExtension。</span><span class="sxs-lookup"><span data-stu-id="9d622-248">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="9d622-249">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="9d622-249">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="9d622-250">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="9d622-250">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="9d622-251">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="9d622-251">Gets or sets a single sign-on extension profile.</span></span>|



## <a name="response"></a><span data-ttu-id="9d622-252">响应</span><span class="sxs-lookup"><span data-stu-id="9d622-252">Response</span></span>
<span data-ttu-id="9d622-253">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9d622-253">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d622-254">示例</span><span class="sxs-lookup"><span data-stu-id="9d622-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d622-255">请求</span><span class="sxs-lookup"><span data-stu-id="9d622-255">Request</span></span>
<span data-ttu-id="9d622-256">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9d622-256">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="9d622-257">响应</span><span class="sxs-lookup"><span data-stu-id="9d622-257">Response</span></span>
<span data-ttu-id="9d622-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9d622-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



