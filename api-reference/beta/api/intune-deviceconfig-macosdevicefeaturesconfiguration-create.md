---
title: 创建 macOSDeviceFeaturesConfiguration
description: 创建新的 macOSDeviceFeaturesConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9d85d2ff96b4da0dea48bce3f8148a7bd93a71fd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147704"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="2f716-103">创建 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f716-103">Create macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="2f716-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f716-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f716-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f716-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f716-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f716-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f716-107">创建新的 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f716-107">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f716-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2f716-108">Prerequisites</span></span>
<span data-ttu-id="2f716-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f716-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f716-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f716-111">Permission type</span></span>|<span data-ttu-id="2f716-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f716-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f716-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f716-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f716-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f716-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f716-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f716-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f716-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f716-116">Not supported.</span></span>|
|<span data-ttu-id="2f716-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f716-117">Application</span></span>|<span data-ttu-id="2f716-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f716-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f716-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f716-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2f716-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f716-120">Request headers</span></span>
|<span data-ttu-id="2f716-121">标头</span><span class="sxs-lookup"><span data-stu-id="2f716-121">Header</span></span>|<span data-ttu-id="2f716-122">值</span><span class="sxs-lookup"><span data-stu-id="2f716-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f716-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f716-123">Authorization</span></span>|<span data-ttu-id="2f716-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2f716-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f716-125">接受</span><span class="sxs-lookup"><span data-stu-id="2f716-125">Accept</span></span>|<span data-ttu-id="2f716-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f716-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f716-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f716-127">Request body</span></span>
<span data-ttu-id="2f716-128">在请求正文中，提供 macOSDeviceFeaturesConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f716-128">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="2f716-129">下表显示创建 macOSDeviceFeaturesConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2f716-129">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="2f716-130">属性</span><span class="sxs-lookup"><span data-stu-id="2f716-130">Property</span></span>|<span data-ttu-id="2f716-131">类型</span><span class="sxs-lookup"><span data-stu-id="2f716-131">Type</span></span>|<span data-ttu-id="2f716-132">说明</span><span class="sxs-lookup"><span data-stu-id="2f716-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f716-133">id</span><span class="sxs-lookup"><span data-stu-id="2f716-133">id</span></span>|<span data-ttu-id="2f716-134">String</span><span class="sxs-lookup"><span data-stu-id="2f716-134">String</span></span>|<span data-ttu-id="2f716-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2f716-135">Key of the entity.</span></span> <span data-ttu-id="2f716-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f716-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f716-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f716-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2f716-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f716-138">DateTimeOffset</span></span>|<span data-ttu-id="2f716-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2f716-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2f716-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f716-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f716-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2f716-141">roleScopeTagIds</span></span>|<span data-ttu-id="2f716-142">String collection</span><span class="sxs-lookup"><span data-stu-id="2f716-142">String collection</span></span>|<span data-ttu-id="2f716-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2f716-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2f716-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f716-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f716-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2f716-145">supportsScopeTags</span></span>|<span data-ttu-id="2f716-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-146">Boolean</span></span>|<span data-ttu-id="2f716-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="2f716-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2f716-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="2f716-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2f716-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="2f716-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2f716-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2f716-150">This property is read-only.</span></span> <span data-ttu-id="2f716-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f716-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f716-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2f716-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2f716-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2f716-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2f716-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="2f716-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2f716-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f716-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f716-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2f716-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2f716-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2f716-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2f716-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2f716-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2f716-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f716-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f716-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2f716-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2f716-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2f716-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2f716-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2f716-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2f716-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f716-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f716-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f716-164">createdDateTime</span></span>|<span data-ttu-id="2f716-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f716-165">DateTimeOffset</span></span>|<span data-ttu-id="2f716-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2f716-166">DateTime the object was created.</span></span> <span data-ttu-id="2f716-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f716-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f716-168">说明</span><span class="sxs-lookup"><span data-stu-id="2f716-168">description</span></span>|<span data-ttu-id="2f716-169">String</span><span class="sxs-lookup"><span data-stu-id="2f716-169">String</span></span>|<span data-ttu-id="2f716-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2f716-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2f716-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f716-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f716-172">displayName</span><span class="sxs-lookup"><span data-stu-id="2f716-172">displayName</span></span>|<span data-ttu-id="2f716-173">String</span><span class="sxs-lookup"><span data-stu-id="2f716-173">String</span></span>|<span data-ttu-id="2f716-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2f716-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2f716-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f716-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f716-176">version</span><span class="sxs-lookup"><span data-stu-id="2f716-176">version</span></span>|<span data-ttu-id="2f716-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2f716-177">Int32</span></span>|<span data-ttu-id="2f716-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2f716-178">Version of the device configuration.</span></span> <span data-ttu-id="2f716-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f716-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f716-180">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="2f716-180">airPrintDestinations</span></span>|<span data-ttu-id="2f716-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f716-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="2f716-182">应始终显示的 AirPrint 打印机数组。</span><span class="sxs-lookup"><span data-stu-id="2f716-182">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="2f716-183">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2f716-183">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="2f716-184">继承自 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="2f716-184">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="2f716-185">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="2f716-185">autoLaunchItems</span></span>|<span data-ttu-id="2f716-186">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f716-186">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="2f716-187">用户登录时要启动的应用程序、文件、文件夹和其他项目的列表。</span><span class="sxs-lookup"><span data-stu-id="2f716-187">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="2f716-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2f716-188">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2f716-189">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="2f716-189">adminShowHostInfo</span></span>|<span data-ttu-id="2f716-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-190">Boolean</span></span>|<span data-ttu-id="2f716-191">是否在登录窗口中显示管理员主机信息。</span><span class="sxs-lookup"><span data-stu-id="2f716-191">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="2f716-192">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="2f716-192">loginWindowText</span></span>|<span data-ttu-id="2f716-193">String</span><span class="sxs-lookup"><span data-stu-id="2f716-193">String</span></span>|<span data-ttu-id="2f716-194">要显示在登录窗口上的自定义文本。</span><span class="sxs-lookup"><span data-stu-id="2f716-194">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="2f716-195">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="2f716-195">authorizedUsersListHidden</span></span>|<span data-ttu-id="2f716-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-196">Boolean</span></span>|<span data-ttu-id="2f716-197">是否在登录窗口中显示名称和密码对话框或用户列表。</span><span class="sxs-lookup"><span data-stu-id="2f716-197">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="2f716-198">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="2f716-198">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="2f716-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-199">Boolean</span></span>|<span data-ttu-id="2f716-200">是否在登录窗口的授权用户列表中只显示网络和系统用户。</span><span class="sxs-lookup"><span data-stu-id="2f716-200">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="2f716-201">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="2f716-201">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="2f716-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-202">Boolean</span></span>|<span data-ttu-id="2f716-203">是否在登录窗口的授权用户列表中隐藏移动用户。</span><span class="sxs-lookup"><span data-stu-id="2f716-203">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="2f716-204">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="2f716-204">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="2f716-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-205">Boolean</span></span>|<span data-ttu-id="2f716-206">是否在登录窗口的授权用户列表中显示网络用户。</span><span class="sxs-lookup"><span data-stu-id="2f716-206">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="2f716-207">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="2f716-207">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="2f716-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-208">Boolean</span></span>|<span data-ttu-id="2f716-209">是否在登录窗口的授权用户列表中隐藏管理员用户。</span><span class="sxs-lookup"><span data-stu-id="2f716-209">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="2f716-210">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="2f716-210">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="2f716-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-211">Boolean</span></span>|<span data-ttu-id="2f716-212">是否在登录窗口的授权用户列表中显示其他用户。</span><span class="sxs-lookup"><span data-stu-id="2f716-212">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="2f716-213">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="2f716-213">shutDownDisabled</span></span>|<span data-ttu-id="2f716-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-214">Boolean</span></span>|<span data-ttu-id="2f716-215">是否在登录窗口中隐藏"关闭"按钮项。</span><span class="sxs-lookup"><span data-stu-id="2f716-215">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="2f716-216">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="2f716-216">restartDisabled</span></span>|<span data-ttu-id="2f716-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-217">Boolean</span></span>|<span data-ttu-id="2f716-218">是否在登录窗口中隐藏"重启"按钮项。</span><span class="sxs-lookup"><span data-stu-id="2f716-218">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="2f716-219">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="2f716-219">sleepDisabled</span></span>|<span data-ttu-id="2f716-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-220">Boolean</span></span>|<span data-ttu-id="2f716-221">是否在登录窗口上隐藏"睡眠"菜单项。</span><span class="sxs-lookup"><span data-stu-id="2f716-221">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="2f716-222">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="2f716-222">consoleAccessDisabled</span></span>|<span data-ttu-id="2f716-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-223">Boolean</span></span>|<span data-ttu-id="2f716-224">其他用户是否将忽略使用'>控制台>特殊用户名。</span><span class="sxs-lookup"><span data-stu-id="2f716-224">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="2f716-225">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="2f716-225">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="2f716-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-226">Boolean</span></span>|<span data-ttu-id="2f716-227">登录时是否禁用登录窗口上的"关闭"菜单项。</span><span class="sxs-lookup"><span data-stu-id="2f716-227">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="2f716-228">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="2f716-228">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="2f716-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-229">Boolean</span></span>|<span data-ttu-id="2f716-230">登录时是否禁用登录窗口上的"重新启动"菜单项。</span><span class="sxs-lookup"><span data-stu-id="2f716-230">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="2f716-231">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="2f716-231">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="2f716-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-232">Boolean</span></span>|<span data-ttu-id="2f716-233">登录窗口上的"电源关闭"菜单项在用户登录时是否将被禁用。</span><span class="sxs-lookup"><span data-stu-id="2f716-233">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="2f716-234">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="2f716-234">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="2f716-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-235">Boolean</span></span>|<span data-ttu-id="2f716-236">登录窗口上的"注销"菜单项在用户登录时是否将被禁用。</span><span class="sxs-lookup"><span data-stu-id="2f716-236">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="2f716-237">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="2f716-237">screenLockDisableImmediate</span></span>|<span data-ttu-id="2f716-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-238">Boolean</span></span>|<span data-ttu-id="2f716-239">是否禁用即时屏幕锁定功能。</span><span class="sxs-lookup"><span data-stu-id="2f716-239">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="2f716-240">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="2f716-240">associatedDomains</span></span>|<span data-ttu-id="2f716-241">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f716-241">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="2f716-242">已弃用：改为使用 appAssociatedDomains。</span><span class="sxs-lookup"><span data-stu-id="2f716-242">DEPRECATED: use appAssociatedDomains instead.</span></span> <span data-ttu-id="2f716-243">获取或设置将应用映射到其关联域的列表。</span><span class="sxs-lookup"><span data-stu-id="2f716-243">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="2f716-244">密钥应匹配应用的 ID，并且值应为"service：domain"形式的字符串，其中 domain 是完全限定的主机名 (例如 webcredentials：example.com) 。</span><span class="sxs-lookup"><span data-stu-id="2f716-244">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="2f716-245">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2f716-245">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2f716-246">appAssociatedDomains</span><span class="sxs-lookup"><span data-stu-id="2f716-246">appAssociatedDomains</span></span>|<span data-ttu-id="2f716-247">[macOSAssociatedDomainsItem](../resources/intune-deviceconfig-macosassociateddomainsitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f716-247">[macOSAssociatedDomainsItem](../resources/intune-deviceconfig-macosassociateddomainsitem.md) collection</span></span>|<span data-ttu-id="2f716-248">获取或设置将应用映射到其关联域的列表。</span><span class="sxs-lookup"><span data-stu-id="2f716-248">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="2f716-249">应用程序标识符必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="2f716-249">Application identifiers must be unique.</span></span> <span data-ttu-id="2f716-250">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2f716-250">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2f716-251">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="2f716-251">singleSignOnExtension</span></span>|[<span data-ttu-id="2f716-252">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="2f716-252">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="2f716-253">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="2f716-253">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="2f716-254">已弃用：改为使用 MacOSSingleSignOnExtension。</span><span class="sxs-lookup"><span data-stu-id="2f716-254">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="2f716-255">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="2f716-255">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="2f716-256">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="2f716-256">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="2f716-257">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="2f716-257">Gets or sets a single sign-on extension profile.</span></span>|
|<span data-ttu-id="2f716-258">contentCachingEnabled</span><span class="sxs-lookup"><span data-stu-id="2f716-258">contentCachingEnabled</span></span>|<span data-ttu-id="2f716-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-259">Boolean</span></span>|<span data-ttu-id="2f716-260">启用内容缓存并防止用户禁用它。</span><span class="sxs-lookup"><span data-stu-id="2f716-260">Enables content caching and prevents it from being disabled by the user.</span></span>|
|<span data-ttu-id="2f716-261">contentCachingType</span><span class="sxs-lookup"><span data-stu-id="2f716-261">contentCachingType</span></span>|[<span data-ttu-id="2f716-262">macOSContentCachingType</span><span class="sxs-lookup"><span data-stu-id="2f716-262">macOSContentCachingType</span></span>](../resources/intune-deviceconfig-macoscontentcachingtype.md)|<span data-ttu-id="2f716-263">确定 Apple 的内容缓存服务允许缓存的内容类型。</span><span class="sxs-lookup"><span data-stu-id="2f716-263">Determines what type of content is allowed to be cached by Apple's content caching service.</span></span> <span data-ttu-id="2f716-264">可取值为：`notConfigured`、`userContentOnly`、`sharedContentOnly`。</span><span class="sxs-lookup"><span data-stu-id="2f716-264">Possible values are: `notConfigured`, `userContentOnly`, `sharedContentOnly`.</span></span>|
|<span data-ttu-id="2f716-265">contentCachingMaxSizeBytes</span><span class="sxs-lookup"><span data-stu-id="2f716-265">contentCachingMaxSizeBytes</span></span>|<span data-ttu-id="2f716-266">Int32</span><span class="sxs-lookup"><span data-stu-id="2f716-266">Int32</span></span>|<span data-ttu-id="2f716-267">将用于内容缓存的最大磁盘空间字节数。</span><span class="sxs-lookup"><span data-stu-id="2f716-267">The maximum number of bytes of disk space that will be used for the content cache.</span></span> <span data-ttu-id="2f716-268">默认值为 0 (表示) 磁盘空间不受限制。</span><span class="sxs-lookup"><span data-stu-id="2f716-268">A value of 0 (default) indicates unlimited disk space.</span></span> |
|<span data-ttu-id="2f716-269">contentCachingDataPath</span><span class="sxs-lookup"><span data-stu-id="2f716-269">contentCachingDataPath</span></span>|<span data-ttu-id="2f716-270">String</span><span class="sxs-lookup"><span data-stu-id="2f716-270">String</span></span>|<span data-ttu-id="2f716-271">用于存储缓存内容的目录的路径。</span><span class="sxs-lookup"><span data-stu-id="2f716-271">The path to the directory used to store cached content.</span></span> <span data-ttu-id="2f716-272">该值必须以 (/Library/Application Support/Apple/AssetCache/Data) 结尾</span><span class="sxs-lookup"><span data-stu-id="2f716-272">The value must be (or end with) /Library/Application Support/Apple/AssetCache/Data</span></span>|
|<span data-ttu-id="2f716-273">contentCachingDisableConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="2f716-273">contentCachingDisableConnectionSharing</span></span>|<span data-ttu-id="2f716-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-274">Boolean</span></span>|<span data-ttu-id="2f716-275">禁用 Internet 连接共享。</span><span class="sxs-lookup"><span data-stu-id="2f716-275">Disables internet connection sharing.</span></span>|
|<span data-ttu-id="2f716-276">contentCachingForceConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="2f716-276">contentCachingForceConnectionSharing</span></span>|<span data-ttu-id="2f716-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-277">Boolean</span></span>|<span data-ttu-id="2f716-278">强制进行 Internet 连接共享。</span><span class="sxs-lookup"><span data-stu-id="2f716-278">Forces internet connection sharing.</span></span> <span data-ttu-id="2f716-279">contentCachingDisableConnectionSharing 会覆盖此设置。</span><span class="sxs-lookup"><span data-stu-id="2f716-279">contentCachingDisableConnectionSharing overrides this setting.</span></span>|
|<span data-ttu-id="2f716-280">contentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="2f716-280">contentCachingClientPolicy</span></span>|[<span data-ttu-id="2f716-281">macOSContentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="2f716-281">macOSContentCachingClientPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingclientpolicy.md)|<span data-ttu-id="2f716-282">确定内容缓存服务器侦听客户端的方法。</span><span class="sxs-lookup"><span data-stu-id="2f716-282">Determines the method in which content caching servers will listen for clients.</span></span> <span data-ttu-id="2f716-283">可取值为：`notConfigured`、`clientsInLocalNetwork`、`clientsWithSamePublicIpAddress`、`clientsInCustomLocalNetworks`、`clientsInCustomLocalNetworksWithFallback`。</span><span class="sxs-lookup"><span data-stu-id="2f716-283">Possible values are: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.</span></span>|
|<span data-ttu-id="2f716-284">contentCachingClientListenRanges</span><span class="sxs-lookup"><span data-stu-id="2f716-284">contentCachingClientListenRanges</span></span>|<span data-ttu-id="2f716-285">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f716-285">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="2f716-286">自定义 IP 范围内容缓存将用于侦听客户端的列表。</span><span class="sxs-lookup"><span data-stu-id="2f716-286">A list of custom IP ranges content caches will use to listen for clients.</span></span> <span data-ttu-id="2f716-287">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2f716-287">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2f716-288">contentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="2f716-288">contentCachingPeerPolicy</span></span>|[<span data-ttu-id="2f716-289">macOSContentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="2f716-289">macOSContentCachingPeerPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingpeerpolicy.md)|<span data-ttu-id="2f716-290">确定内容缓存与其他缓存对等的方法。</span><span class="sxs-lookup"><span data-stu-id="2f716-290">Determines the method in which content caches peer with other caches.</span></span> <span data-ttu-id="2f716-291">可取值为：`notConfigured`、`peersInLocalNetwork`、`peersWithSamePublicIpAddress`、`peersInCustomLocalNetworks`。</span><span class="sxs-lookup"><span data-stu-id="2f716-291">Possible values are: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.</span></span>|
|<span data-ttu-id="2f716-292">contentCachingPeerListenRanges</span><span class="sxs-lookup"><span data-stu-id="2f716-292">contentCachingPeerListenRanges</span></span>|<span data-ttu-id="2f716-293">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f716-293">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="2f716-294">内容缓存将用于侦听对等缓存的自定义 IP 范围列表。</span><span class="sxs-lookup"><span data-stu-id="2f716-294">A list of custom IP ranges content caches will use to listen for peer caches.</span></span> <span data-ttu-id="2f716-295">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2f716-295">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2f716-296">contentCachingPeerFilterRanges</span><span class="sxs-lookup"><span data-stu-id="2f716-296">contentCachingPeerFilterRanges</span></span>|<span data-ttu-id="2f716-297">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f716-297">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="2f716-298">自定义 IP 范围列表内容缓存将用于查询对等缓存中的内容。</span><span class="sxs-lookup"><span data-stu-id="2f716-298">A list of custom IP ranges content caches will use to query for content from peers caches.</span></span> <span data-ttu-id="2f716-299">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2f716-299">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2f716-300">contentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="2f716-300">contentCachingParentSelectionPolicy</span></span>|[<span data-ttu-id="2f716-301">macOSContentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="2f716-301">macOSContentCachingParentSelectionPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingparentselectionpolicy.md)|<span data-ttu-id="2f716-302">确定内容缓存服务器选择父项（如果存在多个父项）的方法。</span><span class="sxs-lookup"><span data-stu-id="2f716-302">Determines the method in which content caching servers will select parents if multiple are present.</span></span> <span data-ttu-id="2f716-303">可取值为：`notConfigured`、`roundRobin`、`firstAvailable`、`urlPathHash`、`random`、`stickyAvailable`。</span><span class="sxs-lookup"><span data-stu-id="2f716-303">Possible values are: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.</span></span>|
|<span data-ttu-id="2f716-304">contentCachingParents</span><span class="sxs-lookup"><span data-stu-id="2f716-304">contentCachingParents</span></span>|<span data-ttu-id="2f716-305">String collection</span><span class="sxs-lookup"><span data-stu-id="2f716-305">String collection</span></span>|<span data-ttu-id="2f716-306">表示父内容缓存的 IP 地址列表。</span><span class="sxs-lookup"><span data-stu-id="2f716-306">A list of IP addresses representing parent content caches.</span></span>|
|<span data-ttu-id="2f716-307">contentCachingLogClientIdentities</span><span class="sxs-lookup"><span data-stu-id="2f716-307">contentCachingLogClientIdentities</span></span>|<span data-ttu-id="2f716-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-308">Boolean</span></span>|<span data-ttu-id="2f716-309">启用请求缓存内容的客户端的 IP 地址和端口的日志记录。</span><span class="sxs-lookup"><span data-stu-id="2f716-309">Enables logging of IP addresses and ports of clients that request cached content.</span></span>|
|<span data-ttu-id="2f716-310">contentCachingPublicRanges</span><span class="sxs-lookup"><span data-stu-id="2f716-310">contentCachingPublicRanges</span></span>|<span data-ttu-id="2f716-311">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f716-311">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="2f716-312">Apple 的内容缓存服务应该用于将客户端与内容缓存相匹配的自定义 IP 范围的列表。</span><span class="sxs-lookup"><span data-stu-id="2f716-312">A list of custom IP ranges that Apple's content caching service should use to match clients to content caches.</span></span> <span data-ttu-id="2f716-313">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2f716-313">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2f716-314">contentCachingBlockDeletion</span><span class="sxs-lookup"><span data-stu-id="2f716-314">contentCachingBlockDeletion</span></span>|<span data-ttu-id="2f716-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-315">Boolean</span></span>|<span data-ttu-id="2f716-316">防止内容缓存清除内容以释放其他应用的磁盘空间。</span><span class="sxs-lookup"><span data-stu-id="2f716-316">Prevents content caches from purging content to free up disk space for other apps.</span></span>|
|<span data-ttu-id="2f716-317">contentCachingShowAlerts</span><span class="sxs-lookup"><span data-stu-id="2f716-317">contentCachingShowAlerts</span></span>|<span data-ttu-id="2f716-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-318">Boolean</span></span>|<span data-ttu-id="2f716-319">将内容缓存警报显示为系统通知。</span><span class="sxs-lookup"><span data-stu-id="2f716-319">Display content caching alerts as system notifications.</span></span>|
|<span data-ttu-id="2f716-320">contentCachingKeepChingke</span><span class="sxs-lookup"><span data-stu-id="2f716-320">contentCachingKeepAwake</span></span>|<span data-ttu-id="2f716-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f716-321">Boolean</span></span>|<span data-ttu-id="2f716-322">如果启用了内容缓存，则防止设备休眠。</span><span class="sxs-lookup"><span data-stu-id="2f716-322">Prevent the device from sleeping if content caching is enabled.</span></span>|
|<span data-ttu-id="2f716-323">contentCachingPort</span><span class="sxs-lookup"><span data-stu-id="2f716-323">contentCachingPort</span></span>|<span data-ttu-id="2f716-324">Int32</span><span class="sxs-lookup"><span data-stu-id="2f716-324">Int32</span></span>|<span data-ttu-id="2f716-325">设置用于内容缓存的端口。</span><span class="sxs-lookup"><span data-stu-id="2f716-325">Sets the port used for content caching.</span></span> <span data-ttu-id="2f716-326">如果值为 0，将选择随机可用的端口。</span><span class="sxs-lookup"><span data-stu-id="2f716-326">If the value is 0, a random available port will be selected.</span></span> <span data-ttu-id="2f716-327">有效值为 0 到 65535</span><span class="sxs-lookup"><span data-stu-id="2f716-327">Valid values 0 to 65535</span></span>|



## <a name="response"></a><span data-ttu-id="2f716-328">响应</span><span class="sxs-lookup"><span data-stu-id="2f716-328">Response</span></span>
<span data-ttu-id="2f716-329">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f716-329">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f716-330">示例</span><span class="sxs-lookup"><span data-stu-id="2f716-330">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f716-331">请求</span><span class="sxs-lookup"><span data-stu-id="2f716-331">Request</span></span>
<span data-ttu-id="2f716-332">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f716-332">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 5662

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
  "appAssociatedDomains": [
    {
      "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem",
      "applicationIdentifier": "Application Identifier value",
      "domains": [
        "Domains value"
      ],
      "directDownloadsEnabled": true
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

### <a name="response"></a><span data-ttu-id="2f716-333">响应</span><span class="sxs-lookup"><span data-stu-id="2f716-333">Response</span></span>
<span data-ttu-id="2f716-p130">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f716-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 5834

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
  "appAssociatedDomains": [
    {
      "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem",
      "applicationIdentifier": "Application Identifier value",
      "domains": [
        "Domains value"
      ],
      "directDownloadsEnabled": true
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




