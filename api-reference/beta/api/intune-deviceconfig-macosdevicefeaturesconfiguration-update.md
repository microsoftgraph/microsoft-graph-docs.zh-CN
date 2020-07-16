---
title: 更新 macOSDeviceFeaturesConfiguration
description: 更新 macOSDeviceFeaturesConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8881ea25ffc5e3e5919a6f6b3498b6caaa377475
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792826"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="07e72-103">更新 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="07e72-103">Update macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="07e72-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07e72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07e72-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="07e72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07e72-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07e72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07e72-107">更新 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="07e72-107">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07e72-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="07e72-108">Prerequisites</span></span>
<span data-ttu-id="07e72-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07e72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07e72-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="07e72-111">Permission type</span></span>|<span data-ttu-id="07e72-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="07e72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07e72-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07e72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07e72-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07e72-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="07e72-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07e72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07e72-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="07e72-116">Not supported.</span></span>|
|<span data-ttu-id="07e72-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="07e72-117">Application</span></span>|<span data-ttu-id="07e72-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07e72-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07e72-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07e72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="07e72-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="07e72-120">Request headers</span></span>
|<span data-ttu-id="07e72-121">标头</span><span class="sxs-lookup"><span data-stu-id="07e72-121">Header</span></span>|<span data-ttu-id="07e72-122">值</span><span class="sxs-lookup"><span data-stu-id="07e72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07e72-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="07e72-123">Authorization</span></span>|<span data-ttu-id="07e72-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="07e72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07e72-125">接受</span><span class="sxs-lookup"><span data-stu-id="07e72-125">Accept</span></span>|<span data-ttu-id="07e72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07e72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07e72-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="07e72-127">Request body</span></span>
<span data-ttu-id="07e72-128">在请求正文中，提供 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07e72-128">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="07e72-129">下表显示创建 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="07e72-129">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="07e72-130">属性</span><span class="sxs-lookup"><span data-stu-id="07e72-130">Property</span></span>|<span data-ttu-id="07e72-131">类型</span><span class="sxs-lookup"><span data-stu-id="07e72-131">Type</span></span>|<span data-ttu-id="07e72-132">说明</span><span class="sxs-lookup"><span data-stu-id="07e72-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07e72-133">id</span><span class="sxs-lookup"><span data-stu-id="07e72-133">id</span></span>|<span data-ttu-id="07e72-134">字符串</span><span class="sxs-lookup"><span data-stu-id="07e72-134">String</span></span>|<span data-ttu-id="07e72-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="07e72-135">Key of the entity.</span></span> <span data-ttu-id="07e72-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07e72-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07e72-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07e72-137">lastModifiedDateTime</span></span>|<span data-ttu-id="07e72-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07e72-138">DateTimeOffset</span></span>|<span data-ttu-id="07e72-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="07e72-139">DateTime the object was last modified.</span></span> <span data-ttu-id="07e72-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07e72-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07e72-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="07e72-141">roleScopeTagIds</span></span>|<span data-ttu-id="07e72-142">String collection</span><span class="sxs-lookup"><span data-stu-id="07e72-142">String collection</span></span>|<span data-ttu-id="07e72-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="07e72-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="07e72-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07e72-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07e72-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="07e72-145">supportsScopeTags</span></span>|<span data-ttu-id="07e72-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-146">Boolean</span></span>|<span data-ttu-id="07e72-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="07e72-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="07e72-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="07e72-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="07e72-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="07e72-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="07e72-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="07e72-150">This property is read-only.</span></span> <span data-ttu-id="07e72-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07e72-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07e72-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="07e72-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="07e72-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="07e72-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="07e72-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="07e72-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="07e72-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07e72-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07e72-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="07e72-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="07e72-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="07e72-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="07e72-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="07e72-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="07e72-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07e72-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07e72-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="07e72-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="07e72-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="07e72-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="07e72-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="07e72-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="07e72-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07e72-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07e72-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07e72-164">createdDateTime</span></span>|<span data-ttu-id="07e72-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07e72-165">DateTimeOffset</span></span>|<span data-ttu-id="07e72-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="07e72-166">DateTime the object was created.</span></span> <span data-ttu-id="07e72-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07e72-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07e72-168">说明</span><span class="sxs-lookup"><span data-stu-id="07e72-168">description</span></span>|<span data-ttu-id="07e72-169">String</span><span class="sxs-lookup"><span data-stu-id="07e72-169">String</span></span>|<span data-ttu-id="07e72-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="07e72-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="07e72-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07e72-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07e72-172">displayName</span><span class="sxs-lookup"><span data-stu-id="07e72-172">displayName</span></span>|<span data-ttu-id="07e72-173">String</span><span class="sxs-lookup"><span data-stu-id="07e72-173">String</span></span>|<span data-ttu-id="07e72-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="07e72-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="07e72-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07e72-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07e72-176">version</span><span class="sxs-lookup"><span data-stu-id="07e72-176">version</span></span>|<span data-ttu-id="07e72-177">Int32</span><span class="sxs-lookup"><span data-stu-id="07e72-177">Int32</span></span>|<span data-ttu-id="07e72-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="07e72-178">Version of the device configuration.</span></span> <span data-ttu-id="07e72-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07e72-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07e72-180">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="07e72-180">airPrintDestinations</span></span>|<span data-ttu-id="07e72-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)集合</span><span class="sxs-lookup"><span data-stu-id="07e72-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="07e72-182">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="07e72-182">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="07e72-183">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="07e72-183">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="07e72-184">继承自[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="07e72-184">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="07e72-185">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="07e72-185">autoLaunchItems</span></span>|<span data-ttu-id="07e72-186">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="07e72-186">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="07e72-187">用户登录时要启动的应用程序、文件、文件夹和其他项目的列表。</span><span class="sxs-lookup"><span data-stu-id="07e72-187">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="07e72-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="07e72-188">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="07e72-189">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="07e72-189">adminShowHostInfo</span></span>|<span data-ttu-id="07e72-190">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-190">Boolean</span></span>|<span data-ttu-id="07e72-191">是否在登录窗口中显示管理员主机信息。</span><span class="sxs-lookup"><span data-stu-id="07e72-191">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="07e72-192">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="07e72-192">loginWindowText</span></span>|<span data-ttu-id="07e72-193">String</span><span class="sxs-lookup"><span data-stu-id="07e72-193">String</span></span>|<span data-ttu-id="07e72-194">要在登录窗口中显示的自定义文本。</span><span class="sxs-lookup"><span data-stu-id="07e72-194">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="07e72-195">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="07e72-195">authorizedUsersListHidden</span></span>|<span data-ttu-id="07e72-196">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-196">Boolean</span></span>|<span data-ttu-id="07e72-197">是否在登录窗口中显示 "名称" 和 "密码" 对话框或用户列表。</span><span class="sxs-lookup"><span data-stu-id="07e72-197">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="07e72-198">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="07e72-198">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="07e72-199">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-199">Boolean</span></span>|<span data-ttu-id="07e72-200">是否在登录窗口的授权用户列表中仅显示网络和系统用户。</span><span class="sxs-lookup"><span data-stu-id="07e72-200">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="07e72-201">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="07e72-201">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="07e72-202">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-202">Boolean</span></span>|<span data-ttu-id="07e72-203">是否在登录窗口上的授权用户列表中隐藏移动用户。</span><span class="sxs-lookup"><span data-stu-id="07e72-203">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="07e72-204">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="07e72-204">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="07e72-205">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-205">Boolean</span></span>|<span data-ttu-id="07e72-206">是否在登录窗口上的授权用户列表中显示网络用户。</span><span class="sxs-lookup"><span data-stu-id="07e72-206">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="07e72-207">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="07e72-207">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="07e72-208">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-208">Boolean</span></span>|<span data-ttu-id="07e72-209">是否在登录窗口的授权用户列表中隐藏管理员用户。</span><span class="sxs-lookup"><span data-stu-id="07e72-209">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="07e72-210">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="07e72-210">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="07e72-211">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-211">Boolean</span></span>|<span data-ttu-id="07e72-212">是否在登录窗口上的授权用户列表中显示其他用户。</span><span class="sxs-lookup"><span data-stu-id="07e72-212">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="07e72-213">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="07e72-213">shutDownDisabled</span></span>|<span data-ttu-id="07e72-214">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-214">Boolean</span></span>|<span data-ttu-id="07e72-215">是否在登录窗口中隐藏 "关机" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="07e72-215">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="07e72-216">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="07e72-216">restartDisabled</span></span>|<span data-ttu-id="07e72-217">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-217">Boolean</span></span>|<span data-ttu-id="07e72-218">是否在登录窗口中隐藏 "重新启动" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="07e72-218">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="07e72-219">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="07e72-219">sleepDisabled</span></span>|<span data-ttu-id="07e72-220">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-220">Boolean</span></span>|<span data-ttu-id="07e72-221">是否在登录窗口中隐藏 "睡眠" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="07e72-221">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="07e72-222">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="07e72-222">consoleAccessDisabled</span></span>|<span data-ttu-id="07e72-223">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-223">Boolean</span></span>|<span data-ttu-id="07e72-224">其他用户是否会忽略使用 ">控制台> 特殊用户名。</span><span class="sxs-lookup"><span data-stu-id="07e72-224">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="07e72-225">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="07e72-225">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="07e72-226">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-226">Boolean</span></span>|<span data-ttu-id="07e72-227">用户登录时是否禁用登录窗口上的 "关闭" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="07e72-227">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="07e72-228">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="07e72-228">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="07e72-229">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-229">Boolean</span></span>|<span data-ttu-id="07e72-230">用户登录时是否禁用登录窗口上的重启菜单项。</span><span class="sxs-lookup"><span data-stu-id="07e72-230">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="07e72-231">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="07e72-231">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="07e72-232">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-232">Boolean</span></span>|<span data-ttu-id="07e72-233">用户登录时登录窗口上的 "断电" 菜单项是否将被禁用。</span><span class="sxs-lookup"><span data-stu-id="07e72-233">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="07e72-234">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="07e72-234">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="07e72-235">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-235">Boolean</span></span>|<span data-ttu-id="07e72-236">用户登录时，登录窗口上的注销菜单项是否会被禁用。</span><span class="sxs-lookup"><span data-stu-id="07e72-236">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="07e72-237">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="07e72-237">screenLockDisableImmediate</span></span>|<span data-ttu-id="07e72-238">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-238">Boolean</span></span>|<span data-ttu-id="07e72-239">是否禁用即时屏幕锁定功能。</span><span class="sxs-lookup"><span data-stu-id="07e72-239">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="07e72-240">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="07e72-240">associatedDomains</span></span>|<span data-ttu-id="07e72-241">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="07e72-241">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="07e72-242">获取或设置一个列表，该列表将应用程序映射到其关联的域。</span><span class="sxs-lookup"><span data-stu-id="07e72-242">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="07e72-243">该密钥应与应用程序的 ID 匹配，并且值应为 "服务：域" 形式的字符串，其中 domain 是完全限定的主机名（例如 webcredentials:example）。</span><span class="sxs-lookup"><span data-stu-id="07e72-243">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="07e72-244">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="07e72-244">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="07e72-245">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="07e72-245">singleSignOnExtension</span></span>|[<span data-ttu-id="07e72-246">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="07e72-246">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="07e72-247">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="07e72-247">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="07e72-248">弃用：改用 MacOSSingleSignOnExtension。</span><span class="sxs-lookup"><span data-stu-id="07e72-248">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="07e72-249">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="07e72-249">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="07e72-250">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="07e72-250">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="07e72-251">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="07e72-251">Gets or sets a single sign-on extension profile.</span></span>|
|<span data-ttu-id="07e72-252">contentCachingEnabled</span><span class="sxs-lookup"><span data-stu-id="07e72-252">contentCachingEnabled</span></span>|<span data-ttu-id="07e72-253">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-253">Boolean</span></span>|<span data-ttu-id="07e72-254">启用内容缓存，并防止用户对其禁用。</span><span class="sxs-lookup"><span data-stu-id="07e72-254">Enables content caching and prevents it from being disabled by the user.</span></span>|
|<span data-ttu-id="07e72-255">contentCachingType</span><span class="sxs-lookup"><span data-stu-id="07e72-255">contentCachingType</span></span>|[<span data-ttu-id="07e72-256">macOSContentCachingType</span><span class="sxs-lookup"><span data-stu-id="07e72-256">macOSContentCachingType</span></span>](../resources/intune-deviceconfig-macoscontentcachingtype.md)|<span data-ttu-id="07e72-257">确定允许由 Apple 的内容缓存服务缓存的内容类型。</span><span class="sxs-lookup"><span data-stu-id="07e72-257">Determines what type of content is allowed to be cached by Apple's content caching service.</span></span> <span data-ttu-id="07e72-258">可取值为：`notConfigured`、`userContentOnly`、`sharedContentOnly`。</span><span class="sxs-lookup"><span data-stu-id="07e72-258">Possible values are: `notConfigured`, `userContentOnly`, `sharedContentOnly`.</span></span>|
|<span data-ttu-id="07e72-259">contentCachingMaxSizeBytes</span><span class="sxs-lookup"><span data-stu-id="07e72-259">contentCachingMaxSizeBytes</span></span>|<span data-ttu-id="07e72-260">Int32</span><span class="sxs-lookup"><span data-stu-id="07e72-260">Int32</span></span>|<span data-ttu-id="07e72-261">将用于内容缓存的磁盘空间的最大字节数。</span><span class="sxs-lookup"><span data-stu-id="07e72-261">The maximum number of bytes of disk space that will be used for the content cache.</span></span> <span data-ttu-id="07e72-262">值为0（默认值）表示无限制的磁盘空间。</span><span class="sxs-lookup"><span data-stu-id="07e72-262">A value of 0 (default) indicates unlimited disk space.</span></span> |
|<span data-ttu-id="07e72-263">contentCachingDataPath</span><span class="sxs-lookup"><span data-stu-id="07e72-263">contentCachingDataPath</span></span>|<span data-ttu-id="07e72-264">String</span><span class="sxs-lookup"><span data-stu-id="07e72-264">String</span></span>|<span data-ttu-id="07e72-265">用于存储缓存内容的目录的路径。</span><span class="sxs-lookup"><span data-stu-id="07e72-265">The path to the directory used to store cached content.</span></span> <span data-ttu-id="07e72-266">值必须是（或 end with）/Library/Application 支持/Apple/AssetCache/Data</span><span class="sxs-lookup"><span data-stu-id="07e72-266">The value must be (or end with) /Library/Application Support/Apple/AssetCache/Data</span></span>|
|<span data-ttu-id="07e72-267">contentCachingDisableConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="07e72-267">contentCachingDisableConnectionSharing</span></span>|<span data-ttu-id="07e72-268">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-268">Boolean</span></span>|<span data-ttu-id="07e72-269">禁用 internet 连接共享。</span><span class="sxs-lookup"><span data-stu-id="07e72-269">Disables internet connection sharing.</span></span>|
|<span data-ttu-id="07e72-270">contentCachingForceConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="07e72-270">contentCachingForceConnectionSharing</span></span>|<span data-ttu-id="07e72-271">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-271">Boolean</span></span>|<span data-ttu-id="07e72-272">强制 internet 连接共享。</span><span class="sxs-lookup"><span data-stu-id="07e72-272">Forces internet connection sharing.</span></span> <span data-ttu-id="07e72-273">contentCachingDisableConnectionSharing 将覆盖此设置。</span><span class="sxs-lookup"><span data-stu-id="07e72-273">contentCachingDisableConnectionSharing overrides this setting.</span></span>|
|<span data-ttu-id="07e72-274">contentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="07e72-274">contentCachingClientPolicy</span></span>|[<span data-ttu-id="07e72-275">macOSContentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="07e72-275">macOSContentCachingClientPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingclientpolicy.md)|<span data-ttu-id="07e72-276">确定内容缓存服务器将在其中侦听客户端的方法。</span><span class="sxs-lookup"><span data-stu-id="07e72-276">Determines the method in which content caching servers will listen for clients.</span></span> <span data-ttu-id="07e72-277">可取值为：`notConfigured`、`clientsInLocalNetwork`、`clientsWithSamePublicIpAddress`、`clientsInCustomLocalNetworks`、`clientsInCustomLocalNetworksWithFallback`。</span><span class="sxs-lookup"><span data-stu-id="07e72-277">Possible values are: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.</span></span>|
|<span data-ttu-id="07e72-278">contentCachingClientListenRanges</span><span class="sxs-lookup"><span data-stu-id="07e72-278">contentCachingClientListenRanges</span></span>|<span data-ttu-id="07e72-279">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="07e72-279">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="07e72-280">自定义 IP 范围的列表将用于侦听客户端。</span><span class="sxs-lookup"><span data-stu-id="07e72-280">A list of custom IP ranges content caches will use to listen for clients.</span></span> <span data-ttu-id="07e72-281">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="07e72-281">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="07e72-282">contentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="07e72-282">contentCachingPeerPolicy</span></span>|[<span data-ttu-id="07e72-283">macOSContentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="07e72-283">macOSContentCachingPeerPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingpeerpolicy.md)|<span data-ttu-id="07e72-284">确定内容缓存对等方和其他缓存的方法。</span><span class="sxs-lookup"><span data-stu-id="07e72-284">Determines the method in which content caches peer with other caches.</span></span> <span data-ttu-id="07e72-285">可取值为：`notConfigured`、`peersInLocalNetwork`、`peersWithSamePublicIpAddress`、`peersInCustomLocalNetworks`。</span><span class="sxs-lookup"><span data-stu-id="07e72-285">Possible values are: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.</span></span>|
|<span data-ttu-id="07e72-286">contentCachingPeerListenRanges</span><span class="sxs-lookup"><span data-stu-id="07e72-286">contentCachingPeerListenRanges</span></span>|<span data-ttu-id="07e72-287">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="07e72-287">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="07e72-288">将使用自定义 IP 范围的列表来侦听对等缓存的内容缓存。</span><span class="sxs-lookup"><span data-stu-id="07e72-288">A list of custom IP ranges content caches will use to listen for peer caches.</span></span> <span data-ttu-id="07e72-289">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="07e72-289">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="07e72-290">contentCachingPeerFilterRanges</span><span class="sxs-lookup"><span data-stu-id="07e72-290">contentCachingPeerFilterRanges</span></span>|<span data-ttu-id="07e72-291">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="07e72-291">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="07e72-292">自定义 IP 范围的列表中，内容缓存将用于查询来自对等缓存的内容。</span><span class="sxs-lookup"><span data-stu-id="07e72-292">A list of custom IP ranges content caches will use to query for content from peers caches.</span></span> <span data-ttu-id="07e72-293">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="07e72-293">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="07e72-294">contentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="07e72-294">contentCachingParentSelectionPolicy</span></span>|[<span data-ttu-id="07e72-295">macOSContentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="07e72-295">macOSContentCachingParentSelectionPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingparentselectionpolicy.md)|<span data-ttu-id="07e72-296">确定内容缓存服务器将选择父项（如果有多个）的方法。</span><span class="sxs-lookup"><span data-stu-id="07e72-296">Determines the method in which content caching servers will select parents if multiple are present.</span></span> <span data-ttu-id="07e72-297">可取值为：`notConfigured`、`roundRobin`、`firstAvailable`、`urlPathHash`、`random`、`stickyAvailable`。</span><span class="sxs-lookup"><span data-stu-id="07e72-297">Possible values are: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.</span></span>|
|<span data-ttu-id="07e72-298">contentCachingParents</span><span class="sxs-lookup"><span data-stu-id="07e72-298">contentCachingParents</span></span>|<span data-ttu-id="07e72-299">String collection</span><span class="sxs-lookup"><span data-stu-id="07e72-299">String collection</span></span>|<span data-ttu-id="07e72-300">表示父内容缓存的 IP 地址的列表。</span><span class="sxs-lookup"><span data-stu-id="07e72-300">A list of IP addresses representing parent content caches.</span></span>|
|<span data-ttu-id="07e72-301">contentCachingLogClientIdentities</span><span class="sxs-lookup"><span data-stu-id="07e72-301">contentCachingLogClientIdentities</span></span>|<span data-ttu-id="07e72-302">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-302">Boolean</span></span>|<span data-ttu-id="07e72-303">启用对请求缓存内容的客户端的 IP 地址和端口的日志记录。</span><span class="sxs-lookup"><span data-stu-id="07e72-303">Enables logging of IP addresses and ports of clients that request cached content.</span></span>|
|<span data-ttu-id="07e72-304">contentCachingPublicRanges</span><span class="sxs-lookup"><span data-stu-id="07e72-304">contentCachingPublicRanges</span></span>|<span data-ttu-id="07e72-305">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="07e72-305">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="07e72-306">Apple 的内容缓存服务应用于将客户端与内容缓存匹配的自定义 IP 范围的列表。</span><span class="sxs-lookup"><span data-stu-id="07e72-306">A list of custom IP ranges that Apple's content caching service should use to match clients to content caches.</span></span> <span data-ttu-id="07e72-307">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="07e72-307">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="07e72-308">contentCachingBlockDeletion</span><span class="sxs-lookup"><span data-stu-id="07e72-308">contentCachingBlockDeletion</span></span>|<span data-ttu-id="07e72-309">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-309">Boolean</span></span>|<span data-ttu-id="07e72-310">防止内容缓存清除内容以释放磁盘空间以用于其他应用程序。</span><span class="sxs-lookup"><span data-stu-id="07e72-310">Prevents content caches from purging content to free up disk space for other apps.</span></span>|
|<span data-ttu-id="07e72-311">contentCachingShowAlerts</span><span class="sxs-lookup"><span data-stu-id="07e72-311">contentCachingShowAlerts</span></span>|<span data-ttu-id="07e72-312">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-312">Boolean</span></span>|<span data-ttu-id="07e72-313">将内容缓存警报显示为系统通知。</span><span class="sxs-lookup"><span data-stu-id="07e72-313">Display content caching alerts as system notifications.</span></span>|
|<span data-ttu-id="07e72-314">contentCachingKeepAwake</span><span class="sxs-lookup"><span data-stu-id="07e72-314">contentCachingKeepAwake</span></span>|<span data-ttu-id="07e72-315">布尔值</span><span class="sxs-lookup"><span data-stu-id="07e72-315">Boolean</span></span>|<span data-ttu-id="07e72-316">如果启用了内容缓存，则阻止设备进入睡眠状态。</span><span class="sxs-lookup"><span data-stu-id="07e72-316">Prevent the device from sleeping if content caching is enabled.</span></span>|
|<span data-ttu-id="07e72-317">contentCachingPort</span><span class="sxs-lookup"><span data-stu-id="07e72-317">contentCachingPort</span></span>|<span data-ttu-id="07e72-318">Int32</span><span class="sxs-lookup"><span data-stu-id="07e72-318">Int32</span></span>|<span data-ttu-id="07e72-319">设置用于内容缓存的端口。</span><span class="sxs-lookup"><span data-stu-id="07e72-319">Sets the port used for content caching.</span></span> <span data-ttu-id="07e72-320">如果值为0，则将选择随机可用端口。</span><span class="sxs-lookup"><span data-stu-id="07e72-320">If the value is 0, a random available port will be selected.</span></span> <span data-ttu-id="07e72-321">有效值为0至65535</span><span class="sxs-lookup"><span data-stu-id="07e72-321">Valid values 0 to 65535</span></span>|



## <a name="response"></a><span data-ttu-id="07e72-322">响应</span><span class="sxs-lookup"><span data-stu-id="07e72-322">Response</span></span>
<span data-ttu-id="07e72-323">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07e72-323">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07e72-324">示例</span><span class="sxs-lookup"><span data-stu-id="07e72-324">Example</span></span>

### <a name="request"></a><span data-ttu-id="07e72-325">请求</span><span class="sxs-lookup"><span data-stu-id="07e72-325">Request</span></span>
<span data-ttu-id="07e72-326">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="07e72-326">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 5388

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
    "@odata.type": "microsoft.graph.credentialSingleSignOnExtension",
    "extensionIdentifier": "Extension Identifier value",
    "teamIdentifier": "Team Identifier value",
    "domains": [
      "Domains value"
    ],
    "realm": "Realm value",
    "configurations": [
      {
        "@odata.type": "microsoft.graph.keyStringValuePair",
        "key": "Key value",
        "value": "Value value"
      }
    ]
  },
  "macOSSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  },
  "contentCachingEnabled": true,
  "contentCachingType": "userContentOnly",
  "contentCachingMaxSizeBytes": 10,
  "contentCachingDataPath": "Content Caching Data Path value",
  "contentCachingDisableConnectionSharing": true,
  "contentCachingForceConnectionSharing": true,
  "contentCachingClientPolicy": "clientsInLocalNetwork",
  "contentCachingClientListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingPeerPolicy": "peersInLocalNetwork",
  "contentCachingPeerListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingPeerFilterRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingParentSelectionPolicy": "roundRobin",
  "contentCachingParents": [
    "Content Caching Parents value"
  ],
  "contentCachingLogClientIdentities": true,
  "contentCachingPublicRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingBlockDeletion": true,
  "contentCachingShowAlerts": true,
  "contentCachingKeepAwake": true,
  "contentCachingPort": 2
}
```

### <a name="response"></a><span data-ttu-id="07e72-327">响应</span><span class="sxs-lookup"><span data-stu-id="07e72-327">Response</span></span>
<span data-ttu-id="07e72-p129">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="07e72-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5560

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
    "@odata.type": "microsoft.graph.credentialSingleSignOnExtension",
    "extensionIdentifier": "Extension Identifier value",
    "teamIdentifier": "Team Identifier value",
    "domains": [
      "Domains value"
    ],
    "realm": "Realm value",
    "configurations": [
      {
        "@odata.type": "microsoft.graph.keyStringValuePair",
        "key": "Key value",
        "value": "Value value"
      }
    ]
  },
  "macOSSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  },
  "contentCachingEnabled": true,
  "contentCachingType": "userContentOnly",
  "contentCachingMaxSizeBytes": 10,
  "contentCachingDataPath": "Content Caching Data Path value",
  "contentCachingDisableConnectionSharing": true,
  "contentCachingForceConnectionSharing": true,
  "contentCachingClientPolicy": "clientsInLocalNetwork",
  "contentCachingClientListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingPeerPolicy": "peersInLocalNetwork",
  "contentCachingPeerListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingPeerFilterRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingParentSelectionPolicy": "roundRobin",
  "contentCachingParents": [
    "Content Caching Parents value"
  ],
  "contentCachingLogClientIdentities": true,
  "contentCachingPublicRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingBlockDeletion": true,
  "contentCachingShowAlerts": true,
  "contentCachingKeepAwake": true,
  "contentCachingPort": 2
}
```



