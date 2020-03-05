---
title: 更新 macOSDeviceFeaturesConfiguration
description: 更新 macOSDeviceFeaturesConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 511ac80fb823976002daab3fa03aaef471675140
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442374"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="c86b5-103">更新 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="c86b5-103">Update macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="c86b5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c86b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c86b5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c86b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c86b5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c86b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c86b5-107">更新 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c86b5-107">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c86b5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c86b5-108">Prerequisites</span></span>
<span data-ttu-id="c86b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c86b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c86b5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c86b5-111">Permission type</span></span>|<span data-ttu-id="c86b5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c86b5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c86b5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c86b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c86b5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c86b5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c86b5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c86b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c86b5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c86b5-116">Not supported.</span></span>|
|<span data-ttu-id="c86b5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c86b5-117">Application</span></span>|<span data-ttu-id="c86b5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c86b5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c86b5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c86b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c86b5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c86b5-120">Request headers</span></span>
|<span data-ttu-id="c86b5-121">标头</span><span class="sxs-lookup"><span data-stu-id="c86b5-121">Header</span></span>|<span data-ttu-id="c86b5-122">值</span><span class="sxs-lookup"><span data-stu-id="c86b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c86b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c86b5-123">Authorization</span></span>|<span data-ttu-id="c86b5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c86b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c86b5-125">接受</span><span class="sxs-lookup"><span data-stu-id="c86b5-125">Accept</span></span>|<span data-ttu-id="c86b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c86b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c86b5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c86b5-127">Request body</span></span>
<span data-ttu-id="c86b5-128">在请求正文中，提供 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c86b5-128">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="c86b5-129">下表显示创建 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c86b5-129">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="c86b5-130">属性</span><span class="sxs-lookup"><span data-stu-id="c86b5-130">Property</span></span>|<span data-ttu-id="c86b5-131">类型</span><span class="sxs-lookup"><span data-stu-id="c86b5-131">Type</span></span>|<span data-ttu-id="c86b5-132">说明</span><span class="sxs-lookup"><span data-stu-id="c86b5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c86b5-133">id</span><span class="sxs-lookup"><span data-stu-id="c86b5-133">id</span></span>|<span data-ttu-id="c86b5-134">字符串</span><span class="sxs-lookup"><span data-stu-id="c86b5-134">String</span></span>|<span data-ttu-id="c86b5-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c86b5-135">Key of the entity.</span></span> <span data-ttu-id="c86b5-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c86b5-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c86b5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c86b5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c86b5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c86b5-138">DateTimeOffset</span></span>|<span data-ttu-id="c86b5-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c86b5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c86b5-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c86b5-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c86b5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c86b5-141">roleScopeTagIds</span></span>|<span data-ttu-id="c86b5-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="c86b5-142">String collection</span></span>|<span data-ttu-id="c86b5-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c86b5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c86b5-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c86b5-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c86b5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c86b5-145">supportsScopeTags</span></span>|<span data-ttu-id="c86b5-146">布尔</span><span class="sxs-lookup"><span data-stu-id="c86b5-146">Boolean</span></span>|<span data-ttu-id="c86b5-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="c86b5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c86b5-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="c86b5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c86b5-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="c86b5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c86b5-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c86b5-150">This property is read-only.</span></span> <span data-ttu-id="c86b5-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c86b5-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c86b5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c86b5-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c86b5-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c86b5-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c86b5-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c86b5-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c86b5-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c86b5-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c86b5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c86b5-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c86b5-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c86b5-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c86b5-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c86b5-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c86b5-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c86b5-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c86b5-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c86b5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c86b5-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c86b5-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c86b5-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c86b5-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c86b5-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c86b5-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c86b5-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c86b5-164">createdDateTime</span></span>|<span data-ttu-id="c86b5-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c86b5-165">DateTimeOffset</span></span>|<span data-ttu-id="c86b5-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c86b5-166">DateTime the object was created.</span></span> <span data-ttu-id="c86b5-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c86b5-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c86b5-168">说明</span><span class="sxs-lookup"><span data-stu-id="c86b5-168">description</span></span>|<span data-ttu-id="c86b5-169">String</span><span class="sxs-lookup"><span data-stu-id="c86b5-169">String</span></span>|<span data-ttu-id="c86b5-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c86b5-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c86b5-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c86b5-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c86b5-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c86b5-172">displayName</span></span>|<span data-ttu-id="c86b5-173">String</span><span class="sxs-lookup"><span data-stu-id="c86b5-173">String</span></span>|<span data-ttu-id="c86b5-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c86b5-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c86b5-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c86b5-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c86b5-176">version</span><span class="sxs-lookup"><span data-stu-id="c86b5-176">version</span></span>|<span data-ttu-id="c86b5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c86b5-177">Int32</span></span>|<span data-ttu-id="c86b5-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c86b5-178">Version of the device configuration.</span></span> <span data-ttu-id="c86b5-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c86b5-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c86b5-180">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="c86b5-180">airPrintDestinations</span></span>|<span data-ttu-id="c86b5-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)集合</span><span class="sxs-lookup"><span data-stu-id="c86b5-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="c86b5-182">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="c86b5-182">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="c86b5-183">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c86b5-183">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c86b5-184">继承自[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="c86b5-184">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="c86b5-185">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="c86b5-185">autoLaunchItems</span></span>|<span data-ttu-id="c86b5-186">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="c86b5-186">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="c86b5-187">用户登录时要启动的应用程序、文件、文件夹和其他项目的列表。</span><span class="sxs-lookup"><span data-stu-id="c86b5-187">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="c86b5-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c86b5-188">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c86b5-189">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="c86b5-189">adminShowHostInfo</span></span>|<span data-ttu-id="c86b5-190">布尔</span><span class="sxs-lookup"><span data-stu-id="c86b5-190">Boolean</span></span>|<span data-ttu-id="c86b5-191">是否在登录窗口中显示管理员主机信息。</span><span class="sxs-lookup"><span data-stu-id="c86b5-191">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="c86b5-192">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="c86b5-192">loginWindowText</span></span>|<span data-ttu-id="c86b5-193">String</span><span class="sxs-lookup"><span data-stu-id="c86b5-193">String</span></span>|<span data-ttu-id="c86b5-194">要在登录窗口中显示的自定义文本。</span><span class="sxs-lookup"><span data-stu-id="c86b5-194">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="c86b5-195">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="c86b5-195">authorizedUsersListHidden</span></span>|<span data-ttu-id="c86b5-196">布尔</span><span class="sxs-lookup"><span data-stu-id="c86b5-196">Boolean</span></span>|<span data-ttu-id="c86b5-197">是否在登录窗口中显示 "名称" 和 "密码" 对话框或用户列表。</span><span class="sxs-lookup"><span data-stu-id="c86b5-197">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="c86b5-198">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="c86b5-198">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="c86b5-199">布尔</span><span class="sxs-lookup"><span data-stu-id="c86b5-199">Boolean</span></span>|<span data-ttu-id="c86b5-200">是否在登录窗口的授权用户列表中仅显示网络和系统用户。</span><span class="sxs-lookup"><span data-stu-id="c86b5-200">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="c86b5-201">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="c86b5-201">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="c86b5-202">布尔</span><span class="sxs-lookup"><span data-stu-id="c86b5-202">Boolean</span></span>|<span data-ttu-id="c86b5-203">是否在登录窗口上的授权用户列表中隐藏移动用户。</span><span class="sxs-lookup"><span data-stu-id="c86b5-203">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="c86b5-204">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="c86b5-204">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="c86b5-205">布尔</span><span class="sxs-lookup"><span data-stu-id="c86b5-205">Boolean</span></span>|<span data-ttu-id="c86b5-206">是否在登录窗口上的授权用户列表中显示网络用户。</span><span class="sxs-lookup"><span data-stu-id="c86b5-206">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="c86b5-207">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="c86b5-207">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="c86b5-208">布尔</span><span class="sxs-lookup"><span data-stu-id="c86b5-208">Boolean</span></span>|<span data-ttu-id="c86b5-209">是否在登录窗口的授权用户列表中隐藏管理员用户。</span><span class="sxs-lookup"><span data-stu-id="c86b5-209">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="c86b5-210">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="c86b5-210">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="c86b5-211">布尔</span><span class="sxs-lookup"><span data-stu-id="c86b5-211">Boolean</span></span>|<span data-ttu-id="c86b5-212">是否在登录窗口上的授权用户列表中显示其他用户。</span><span class="sxs-lookup"><span data-stu-id="c86b5-212">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="c86b5-213">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="c86b5-213">shutDownDisabled</span></span>|<span data-ttu-id="c86b5-214">布尔</span><span class="sxs-lookup"><span data-stu-id="c86b5-214">Boolean</span></span>|<span data-ttu-id="c86b5-215">是否在登录窗口中隐藏 "关机" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="c86b5-215">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="c86b5-216">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="c86b5-216">restartDisabled</span></span>|<span data-ttu-id="c86b5-217">布尔</span><span class="sxs-lookup"><span data-stu-id="c86b5-217">Boolean</span></span>|<span data-ttu-id="c86b5-218">是否在登录窗口中隐藏 "重新启动" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="c86b5-218">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="c86b5-219">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="c86b5-219">sleepDisabled</span></span>|<span data-ttu-id="c86b5-220">布尔</span><span class="sxs-lookup"><span data-stu-id="c86b5-220">Boolean</span></span>|<span data-ttu-id="c86b5-221">是否在登录窗口中隐藏 "睡眠" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="c86b5-221">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="c86b5-222">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="c86b5-222">consoleAccessDisabled</span></span>|<span data-ttu-id="c86b5-223">布尔</span><span class="sxs-lookup"><span data-stu-id="c86b5-223">Boolean</span></span>|<span data-ttu-id="c86b5-224">其他用户是否会忽略使用 ">控制台> 特殊用户名。</span><span class="sxs-lookup"><span data-stu-id="c86b5-224">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="c86b5-225">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="c86b5-225">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="c86b5-226">布尔</span><span class="sxs-lookup"><span data-stu-id="c86b5-226">Boolean</span></span>|<span data-ttu-id="c86b5-227">用户登录时是否禁用登录窗口上的 "关闭" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="c86b5-227">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="c86b5-228">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="c86b5-228">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="c86b5-229">布尔</span><span class="sxs-lookup"><span data-stu-id="c86b5-229">Boolean</span></span>|<span data-ttu-id="c86b5-230">用户登录时是否禁用登录窗口上的重启菜单项。</span><span class="sxs-lookup"><span data-stu-id="c86b5-230">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="c86b5-231">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="c86b5-231">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="c86b5-232">布尔</span><span class="sxs-lookup"><span data-stu-id="c86b5-232">Boolean</span></span>|<span data-ttu-id="c86b5-233">用户登录时登录窗口上的 "断电" 菜单项是否将被禁用。</span><span class="sxs-lookup"><span data-stu-id="c86b5-233">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="c86b5-234">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="c86b5-234">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="c86b5-235">布尔</span><span class="sxs-lookup"><span data-stu-id="c86b5-235">Boolean</span></span>|<span data-ttu-id="c86b5-236">用户登录时，登录窗口上的注销菜单项是否会被禁用。</span><span class="sxs-lookup"><span data-stu-id="c86b5-236">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="c86b5-237">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="c86b5-237">screenLockDisableImmediate</span></span>|<span data-ttu-id="c86b5-238">布尔</span><span class="sxs-lookup"><span data-stu-id="c86b5-238">Boolean</span></span>|<span data-ttu-id="c86b5-239">是否禁用即时屏幕锁定功能。</span><span class="sxs-lookup"><span data-stu-id="c86b5-239">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="c86b5-240">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="c86b5-240">associatedDomains</span></span>|<span data-ttu-id="c86b5-241">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c86b5-241">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c86b5-242">获取或设置一个列表，该列表将应用程序映射到其关联的域。</span><span class="sxs-lookup"><span data-stu-id="c86b5-242">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="c86b5-243">该密钥应与应用程序的 ID 匹配，并且值应为 "服务：域" 形式的字符串，其中 domain 是完全限定的主机名（例如 webcredentials:example）。</span><span class="sxs-lookup"><span data-stu-id="c86b5-243">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="c86b5-244">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c86b5-244">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c86b5-245">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="c86b5-245">singleSignOnExtension</span></span>|[<span data-ttu-id="c86b5-246">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="c86b5-246">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="c86b5-247">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="c86b5-247">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="c86b5-248">弃用：改用 MacOSSingleSignOnExtension。</span><span class="sxs-lookup"><span data-stu-id="c86b5-248">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="c86b5-249">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="c86b5-249">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="c86b5-250">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="c86b5-250">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="c86b5-251">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="c86b5-251">Gets or sets a single sign-on extension profile.</span></span>|



## <a name="response"></a><span data-ttu-id="c86b5-252">响应</span><span class="sxs-lookup"><span data-stu-id="c86b5-252">Response</span></span>
<span data-ttu-id="c86b5-253">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c86b5-253">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c86b5-254">示例</span><span class="sxs-lookup"><span data-stu-id="c86b5-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="c86b5-255">请求</span><span class="sxs-lookup"><span data-stu-id="c86b5-255">Request</span></span>
<span data-ttu-id="c86b5-256">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c86b5-256">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c86b5-257">响应</span><span class="sxs-lookup"><span data-stu-id="c86b5-257">Response</span></span>
<span data-ttu-id="c86b5-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c86b5-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





