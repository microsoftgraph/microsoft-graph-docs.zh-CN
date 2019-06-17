---
title: 更新 macOSDeviceFeaturesConfiguration
description: 更新 macOSDeviceFeaturesConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 780a99d3a298caee1e50d8b85699e9f6a4c2a9af
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34976804"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="6c8b1-103">更新 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c8b1-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="6c8b1-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c8b1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c8b1-106">更新 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-106">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c8b1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6c8b1-107">Prerequisites</span></span>
<span data-ttu-id="6c8b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c8b1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c8b1-110">Permission type</span></span>|<span data-ttu-id="6c8b1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6c8b1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c8b1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c8b1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c8b1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c8b1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c8b1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c8b1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c8b1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-115">Not supported.</span></span>|
|<span data-ttu-id="6c8b1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c8b1-116">Application</span></span>|<span data-ttu-id="6c8b1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c8b1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c8b1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6c8b1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c8b1-119">Request headers</span></span>
|<span data-ttu-id="6c8b1-120">标头</span><span class="sxs-lookup"><span data-stu-id="6c8b1-120">Header</span></span>|<span data-ttu-id="6c8b1-121">值</span><span class="sxs-lookup"><span data-stu-id="6c8b1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c8b1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c8b1-122">Authorization</span></span>|<span data-ttu-id="6c8b1-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c8b1-124">接受</span><span class="sxs-lookup"><span data-stu-id="6c8b1-124">Accept</span></span>|<span data-ttu-id="6c8b1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c8b1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c8b1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c8b1-126">Request body</span></span>
<span data-ttu-id="6c8b1-127">在请求正文中，提供 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-127">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="6c8b1-128">下表显示创建 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-128">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="6c8b1-129">属性</span><span class="sxs-lookup"><span data-stu-id="6c8b1-129">Property</span></span>|<span data-ttu-id="6c8b1-130">类型</span><span class="sxs-lookup"><span data-stu-id="6c8b1-130">Type</span></span>|<span data-ttu-id="6c8b1-131">说明</span><span class="sxs-lookup"><span data-stu-id="6c8b1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c8b1-132">id</span><span class="sxs-lookup"><span data-stu-id="6c8b1-132">id</span></span>|<span data-ttu-id="6c8b1-133">字符串</span><span class="sxs-lookup"><span data-stu-id="6c8b1-133">String</span></span>|<span data-ttu-id="6c8b1-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-134">Key of the entity.</span></span> <span data-ttu-id="6c8b1-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c8b1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c8b1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c8b1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6c8b1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c8b1-137">DateTimeOffset</span></span>|<span data-ttu-id="6c8b1-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6c8b1-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c8b1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c8b1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6c8b1-140">roleScopeTagIds</span></span>|<span data-ttu-id="6c8b1-141">String collection</span><span class="sxs-lookup"><span data-stu-id="6c8b1-141">String collection</span></span>|<span data-ttu-id="6c8b1-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6c8b1-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c8b1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c8b1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6c8b1-144">supportsScopeTags</span></span>|<span data-ttu-id="6c8b1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8b1-145">Boolean</span></span>|<span data-ttu-id="6c8b1-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6c8b1-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6c8b1-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6c8b1-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-149">This property is read-only.</span></span> <span data-ttu-id="6c8b1-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c8b1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c8b1-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6c8b1-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6c8b1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6c8b1-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6c8b1-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6c8b1-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c8b1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c8b1-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6c8b1-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6c8b1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6c8b1-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6c8b1-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6c8b1-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c8b1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c8b1-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6c8b1-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6c8b1-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6c8b1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6c8b1-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6c8b1-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c8b1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c8b1-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c8b1-163">createdDateTime</span></span>|<span data-ttu-id="6c8b1-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c8b1-164">DateTimeOffset</span></span>|<span data-ttu-id="6c8b1-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-165">DateTime the object was created.</span></span> <span data-ttu-id="6c8b1-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c8b1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c8b1-167">说明</span><span class="sxs-lookup"><span data-stu-id="6c8b1-167">description</span></span>|<span data-ttu-id="6c8b1-168">String</span><span class="sxs-lookup"><span data-stu-id="6c8b1-168">String</span></span>|<span data-ttu-id="6c8b1-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6c8b1-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c8b1-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c8b1-171">displayName</span><span class="sxs-lookup"><span data-stu-id="6c8b1-171">displayName</span></span>|<span data-ttu-id="6c8b1-172">String</span><span class="sxs-lookup"><span data-stu-id="6c8b1-172">String</span></span>|<span data-ttu-id="6c8b1-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6c8b1-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c8b1-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c8b1-175">version</span><span class="sxs-lookup"><span data-stu-id="6c8b1-175">version</span></span>|<span data-ttu-id="6c8b1-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6c8b1-176">Int32</span></span>|<span data-ttu-id="6c8b1-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-177">Version of the device configuration.</span></span> <span data-ttu-id="6c8b1-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c8b1-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c8b1-179">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="6c8b1-179">airPrintDestinations</span></span>|<span data-ttu-id="6c8b1-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)集合</span><span class="sxs-lookup"><span data-stu-id="6c8b1-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="6c8b1-181">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="6c8b1-182">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6c8b1-183">继承自[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="6c8b1-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="6c8b1-184">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="6c8b1-184">autoLaunchItems</span></span>|<span data-ttu-id="6c8b1-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="6c8b1-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="6c8b1-186">用户登录时要启动的应用程序、文件、文件夹和其他项目的列表。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-186">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="6c8b1-187">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-187">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6c8b1-188">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="6c8b1-188">adminShowHostInfo</span></span>|<span data-ttu-id="6c8b1-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8b1-189">Boolean</span></span>|<span data-ttu-id="6c8b1-190">是否在登录窗口中显示管理员主机信息。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-190">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="6c8b1-191">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="6c8b1-191">loginWindowText</span></span>|<span data-ttu-id="6c8b1-192">String</span><span class="sxs-lookup"><span data-stu-id="6c8b1-192">String</span></span>|<span data-ttu-id="6c8b1-193">要在登录窗口中显示的自定义文本。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-193">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="6c8b1-194">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="6c8b1-194">authorizedUsersListHidden</span></span>|<span data-ttu-id="6c8b1-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8b1-195">Boolean</span></span>|<span data-ttu-id="6c8b1-196">是否在登录窗口中显示 "名称" 和 "密码" 对话框或用户列表。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-196">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="6c8b1-197">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="6c8b1-197">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="6c8b1-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8b1-198">Boolean</span></span>|<span data-ttu-id="6c8b1-199">是否在登录窗口的授权用户列表中仅显示网络和系统用户。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-199">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="6c8b1-200">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="6c8b1-200">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="6c8b1-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8b1-201">Boolean</span></span>|<span data-ttu-id="6c8b1-202">是否在登录窗口上的授权用户列表中隐藏移动用户。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-202">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="6c8b1-203">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="6c8b1-203">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="6c8b1-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8b1-204">Boolean</span></span>|<span data-ttu-id="6c8b1-205">是否在登录窗口上的授权用户列表中显示网络用户。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-205">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="6c8b1-206">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="6c8b1-206">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="6c8b1-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8b1-207">Boolean</span></span>|<span data-ttu-id="6c8b1-208">是否在登录窗口的授权用户列表中隐藏管理员用户。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-208">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="6c8b1-209">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="6c8b1-209">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="6c8b1-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8b1-210">Boolean</span></span>|<span data-ttu-id="6c8b1-211">是否在登录窗口上的授权用户列表中显示其他用户。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-211">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="6c8b1-212">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="6c8b1-212">shutDownDisabled</span></span>|<span data-ttu-id="6c8b1-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8b1-213">Boolean</span></span>|<span data-ttu-id="6c8b1-214">是否在登录窗口中隐藏 "关机" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-214">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="6c8b1-215">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="6c8b1-215">restartDisabled</span></span>|<span data-ttu-id="6c8b1-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8b1-216">Boolean</span></span>|<span data-ttu-id="6c8b1-217">是否在登录窗口中隐藏 "重新启动" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-217">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="6c8b1-218">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="6c8b1-218">sleepDisabled</span></span>|<span data-ttu-id="6c8b1-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8b1-219">Boolean</span></span>|<span data-ttu-id="6c8b1-220">是否在登录窗口中隐藏 "睡眠" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-220">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="6c8b1-221">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="6c8b1-221">consoleAccessDisabled</span></span>|<span data-ttu-id="6c8b1-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8b1-222">Boolean</span></span>|<span data-ttu-id="6c8b1-223">其他用户是否会忽略使用 ">控制台> 特殊用户名。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-223">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="6c8b1-224">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="6c8b1-224">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="6c8b1-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8b1-225">Boolean</span></span>|<span data-ttu-id="6c8b1-226">用户登录时是否禁用登录窗口上的 "关闭" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-226">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="6c8b1-227">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="6c8b1-227">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="6c8b1-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8b1-228">Boolean</span></span>|<span data-ttu-id="6c8b1-229">用户登录时是否禁用登录窗口上的重启菜单项。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-229">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="6c8b1-230">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="6c8b1-230">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="6c8b1-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8b1-231">Boolean</span></span>|<span data-ttu-id="6c8b1-232">用户登录时登录窗口上的 "断电" 菜单项是否将被禁用。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-232">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="6c8b1-233">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="6c8b1-233">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="6c8b1-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8b1-234">Boolean</span></span>|<span data-ttu-id="6c8b1-235">用户登录时, 登录窗口上的注销菜单项是否会被禁用。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-235">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="6c8b1-236">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="6c8b1-236">screenLockDisableImmediate</span></span>|<span data-ttu-id="6c8b1-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8b1-237">Boolean</span></span>|<span data-ttu-id="6c8b1-238">是否禁用即时屏幕锁定功能。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-238">Whether to disable the immediate screen lock functions.</span></span>|



## <a name="response"></a><span data-ttu-id="6c8b1-239">响应</span><span class="sxs-lookup"><span data-stu-id="6c8b1-239">Response</span></span>
<span data-ttu-id="6c8b1-240">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-240">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c8b1-241">示例</span><span class="sxs-lookup"><span data-stu-id="6c8b1-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c8b1-242">请求</span><span class="sxs-lookup"><span data-stu-id="6c8b1-242">Request</span></span>
<span data-ttu-id="6c8b1-243">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2107

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
  "screenLockDisableImmediate": true
}
```

### <a name="response"></a><span data-ttu-id="6c8b1-244">响应</span><span class="sxs-lookup"><span data-stu-id="6c8b1-244">Response</span></span>
<span data-ttu-id="6c8b1-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6c8b1-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2279

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
  "screenLockDisableImmediate": true
}
```





