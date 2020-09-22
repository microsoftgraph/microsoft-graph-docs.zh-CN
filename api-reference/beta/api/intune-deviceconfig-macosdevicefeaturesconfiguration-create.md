---
title: 创建 macOSDeviceFeaturesConfiguration
description: 创建新的 macOSDeviceFeaturesConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9033d76816d402b190ff9dbffd49d9ef3d4834e5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017945"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="17f47-103">创建 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="17f47-103">Create macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="17f47-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17f47-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17f47-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="17f47-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17f47-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="17f47-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17f47-107">创建新的 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="17f47-107">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17f47-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="17f47-108">Prerequisites</span></span>
<span data-ttu-id="17f47-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17f47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17f47-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="17f47-111">Permission type</span></span>|<span data-ttu-id="17f47-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="17f47-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17f47-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17f47-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17f47-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17f47-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17f47-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17f47-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17f47-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="17f47-116">Not supported.</span></span>|
|<span data-ttu-id="17f47-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="17f47-117">Application</span></span>|<span data-ttu-id="17f47-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17f47-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17f47-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17f47-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="17f47-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="17f47-120">Request headers</span></span>
|<span data-ttu-id="17f47-121">标头</span><span class="sxs-lookup"><span data-stu-id="17f47-121">Header</span></span>|<span data-ttu-id="17f47-122">值</span><span class="sxs-lookup"><span data-stu-id="17f47-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17f47-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="17f47-123">Authorization</span></span>|<span data-ttu-id="17f47-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="17f47-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17f47-125">接受</span><span class="sxs-lookup"><span data-stu-id="17f47-125">Accept</span></span>|<span data-ttu-id="17f47-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17f47-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17f47-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="17f47-127">Request body</span></span>
<span data-ttu-id="17f47-128">在请求正文中，提供 macOSDeviceFeaturesConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17f47-128">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="17f47-129">下表显示创建 macOSDeviceFeaturesConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="17f47-129">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="17f47-130">属性</span><span class="sxs-lookup"><span data-stu-id="17f47-130">Property</span></span>|<span data-ttu-id="17f47-131">类型</span><span class="sxs-lookup"><span data-stu-id="17f47-131">Type</span></span>|<span data-ttu-id="17f47-132">说明</span><span class="sxs-lookup"><span data-stu-id="17f47-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17f47-133">id</span><span class="sxs-lookup"><span data-stu-id="17f47-133">id</span></span>|<span data-ttu-id="17f47-134">String</span><span class="sxs-lookup"><span data-stu-id="17f47-134">String</span></span>|<span data-ttu-id="17f47-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="17f47-135">Key of the entity.</span></span> <span data-ttu-id="17f47-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17f47-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17f47-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17f47-137">lastModifiedDateTime</span></span>|<span data-ttu-id="17f47-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17f47-138">DateTimeOffset</span></span>|<span data-ttu-id="17f47-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="17f47-139">DateTime the object was last modified.</span></span> <span data-ttu-id="17f47-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17f47-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17f47-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="17f47-141">roleScopeTagIds</span></span>|<span data-ttu-id="17f47-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="17f47-142">String collection</span></span>|<span data-ttu-id="17f47-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="17f47-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="17f47-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17f47-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17f47-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="17f47-145">supportsScopeTags</span></span>|<span data-ttu-id="17f47-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-146">Boolean</span></span>|<span data-ttu-id="17f47-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="17f47-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="17f47-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="17f47-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="17f47-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="17f47-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="17f47-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="17f47-150">This property is read-only.</span></span> <span data-ttu-id="17f47-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17f47-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17f47-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="17f47-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="17f47-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="17f47-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="17f47-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="17f47-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="17f47-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17f47-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17f47-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="17f47-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="17f47-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="17f47-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="17f47-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="17f47-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="17f47-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17f47-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17f47-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="17f47-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="17f47-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="17f47-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="17f47-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="17f47-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="17f47-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17f47-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17f47-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17f47-164">createdDateTime</span></span>|<span data-ttu-id="17f47-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17f47-165">DateTimeOffset</span></span>|<span data-ttu-id="17f47-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="17f47-166">DateTime the object was created.</span></span> <span data-ttu-id="17f47-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17f47-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17f47-168">description</span><span class="sxs-lookup"><span data-stu-id="17f47-168">description</span></span>|<span data-ttu-id="17f47-169">String</span><span class="sxs-lookup"><span data-stu-id="17f47-169">String</span></span>|<span data-ttu-id="17f47-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="17f47-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="17f47-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17f47-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17f47-172">displayName</span><span class="sxs-lookup"><span data-stu-id="17f47-172">displayName</span></span>|<span data-ttu-id="17f47-173">String</span><span class="sxs-lookup"><span data-stu-id="17f47-173">String</span></span>|<span data-ttu-id="17f47-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="17f47-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="17f47-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17f47-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17f47-176">version</span><span class="sxs-lookup"><span data-stu-id="17f47-176">version</span></span>|<span data-ttu-id="17f47-177">Int32</span><span class="sxs-lookup"><span data-stu-id="17f47-177">Int32</span></span>|<span data-ttu-id="17f47-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="17f47-178">Version of the device configuration.</span></span> <span data-ttu-id="17f47-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17f47-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17f47-180">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="17f47-180">airPrintDestinations</span></span>|<span data-ttu-id="17f47-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17f47-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="17f47-182">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="17f47-182">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="17f47-183">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="17f47-183">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="17f47-184">继承自 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="17f47-184">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="17f47-185">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="17f47-185">autoLaunchItems</span></span>|<span data-ttu-id="17f47-186">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17f47-186">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="17f47-187">用户登录时要启动的应用程序、文件、文件夹和其他项目的列表。</span><span class="sxs-lookup"><span data-stu-id="17f47-187">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="17f47-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="17f47-188">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="17f47-189">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="17f47-189">adminShowHostInfo</span></span>|<span data-ttu-id="17f47-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-190">Boolean</span></span>|<span data-ttu-id="17f47-191">是否在登录窗口中显示管理员主机信息。</span><span class="sxs-lookup"><span data-stu-id="17f47-191">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="17f47-192">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="17f47-192">loginWindowText</span></span>|<span data-ttu-id="17f47-193">String</span><span class="sxs-lookup"><span data-stu-id="17f47-193">String</span></span>|<span data-ttu-id="17f47-194">要在登录窗口中显示的自定义文本。</span><span class="sxs-lookup"><span data-stu-id="17f47-194">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="17f47-195">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="17f47-195">authorizedUsersListHidden</span></span>|<span data-ttu-id="17f47-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-196">Boolean</span></span>|<span data-ttu-id="17f47-197">是否在登录窗口中显示 "名称" 和 "密码" 对话框或用户列表。</span><span class="sxs-lookup"><span data-stu-id="17f47-197">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="17f47-198">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="17f47-198">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="17f47-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-199">Boolean</span></span>|<span data-ttu-id="17f47-200">是否在登录窗口的授权用户列表中仅显示网络和系统用户。</span><span class="sxs-lookup"><span data-stu-id="17f47-200">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="17f47-201">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="17f47-201">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="17f47-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-202">Boolean</span></span>|<span data-ttu-id="17f47-203">是否在登录窗口上的授权用户列表中隐藏移动用户。</span><span class="sxs-lookup"><span data-stu-id="17f47-203">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="17f47-204">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="17f47-204">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="17f47-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-205">Boolean</span></span>|<span data-ttu-id="17f47-206">是否在登录窗口上的授权用户列表中显示网络用户。</span><span class="sxs-lookup"><span data-stu-id="17f47-206">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="17f47-207">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="17f47-207">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="17f47-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-208">Boolean</span></span>|<span data-ttu-id="17f47-209">是否在登录窗口的授权用户列表中隐藏管理员用户。</span><span class="sxs-lookup"><span data-stu-id="17f47-209">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="17f47-210">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="17f47-210">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="17f47-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-211">Boolean</span></span>|<span data-ttu-id="17f47-212">是否在登录窗口上的授权用户列表中显示其他用户。</span><span class="sxs-lookup"><span data-stu-id="17f47-212">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="17f47-213">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="17f47-213">shutDownDisabled</span></span>|<span data-ttu-id="17f47-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-214">Boolean</span></span>|<span data-ttu-id="17f47-215">是否在登录窗口中隐藏 "关机" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="17f47-215">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="17f47-216">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="17f47-216">restartDisabled</span></span>|<span data-ttu-id="17f47-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-217">Boolean</span></span>|<span data-ttu-id="17f47-218">是否在登录窗口中隐藏 "重新启动" 按钮项。</span><span class="sxs-lookup"><span data-stu-id="17f47-218">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="17f47-219">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="17f47-219">sleepDisabled</span></span>|<span data-ttu-id="17f47-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-220">Boolean</span></span>|<span data-ttu-id="17f47-221">是否在登录窗口中隐藏 "睡眠" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="17f47-221">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="17f47-222">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="17f47-222">consoleAccessDisabled</span></span>|<span data-ttu-id="17f47-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-223">Boolean</span></span>|<span data-ttu-id="17f47-224">其他用户是否会忽略使用 ">控制台> 特殊用户名。</span><span class="sxs-lookup"><span data-stu-id="17f47-224">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="17f47-225">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="17f47-225">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="17f47-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-226">Boolean</span></span>|<span data-ttu-id="17f47-227">用户登录时是否禁用登录窗口上的 "关闭" 菜单项。</span><span class="sxs-lookup"><span data-stu-id="17f47-227">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="17f47-228">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="17f47-228">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="17f47-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-229">Boolean</span></span>|<span data-ttu-id="17f47-230">用户登录时是否禁用登录窗口上的重启菜单项。</span><span class="sxs-lookup"><span data-stu-id="17f47-230">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="17f47-231">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="17f47-231">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="17f47-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-232">Boolean</span></span>|<span data-ttu-id="17f47-233">用户登录时登录窗口上的 "断电" 菜单项是否将被禁用。</span><span class="sxs-lookup"><span data-stu-id="17f47-233">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="17f47-234">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="17f47-234">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="17f47-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-235">Boolean</span></span>|<span data-ttu-id="17f47-236">用户登录时，登录窗口上的注销菜单项是否会被禁用。</span><span class="sxs-lookup"><span data-stu-id="17f47-236">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="17f47-237">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="17f47-237">screenLockDisableImmediate</span></span>|<span data-ttu-id="17f47-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-238">Boolean</span></span>|<span data-ttu-id="17f47-239">是否禁用即时屏幕锁定功能。</span><span class="sxs-lookup"><span data-stu-id="17f47-239">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="17f47-240">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="17f47-240">associatedDomains</span></span>|<span data-ttu-id="17f47-241">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17f47-241">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="17f47-242">获取或设置一个列表，该列表将应用程序映射到其关联的域。</span><span class="sxs-lookup"><span data-stu-id="17f47-242">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="17f47-243">键应与应用程序的 ID 匹配，并且值应为 "服务：域" 形式的字符串，其中 domain 是完全限定的主机名 (例如，webcredentials:example) 。</span><span class="sxs-lookup"><span data-stu-id="17f47-243">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="17f47-244">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="17f47-244">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="17f47-245">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="17f47-245">singleSignOnExtension</span></span>|[<span data-ttu-id="17f47-246">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="17f47-246">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="17f47-247">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="17f47-247">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="17f47-248">弃用：改用 MacOSSingleSignOnExtension。</span><span class="sxs-lookup"><span data-stu-id="17f47-248">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="17f47-249">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="17f47-249">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="17f47-250">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="17f47-250">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="17f47-251">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="17f47-251">Gets or sets a single sign-on extension profile.</span></span>|
|<span data-ttu-id="17f47-252">contentCachingEnabled</span><span class="sxs-lookup"><span data-stu-id="17f47-252">contentCachingEnabled</span></span>|<span data-ttu-id="17f47-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-253">Boolean</span></span>|<span data-ttu-id="17f47-254">启用内容缓存，并防止用户对其禁用。</span><span class="sxs-lookup"><span data-stu-id="17f47-254">Enables content caching and prevents it from being disabled by the user.</span></span>|
|<span data-ttu-id="17f47-255">contentCachingType</span><span class="sxs-lookup"><span data-stu-id="17f47-255">contentCachingType</span></span>|[<span data-ttu-id="17f47-256">macOSContentCachingType</span><span class="sxs-lookup"><span data-stu-id="17f47-256">macOSContentCachingType</span></span>](../resources/intune-deviceconfig-macoscontentcachingtype.md)|<span data-ttu-id="17f47-257">确定允许由 Apple 的内容缓存服务缓存的内容类型。</span><span class="sxs-lookup"><span data-stu-id="17f47-257">Determines what type of content is allowed to be cached by Apple's content caching service.</span></span> <span data-ttu-id="17f47-258">可取值为：`notConfigured`、`userContentOnly`、`sharedContentOnly`。</span><span class="sxs-lookup"><span data-stu-id="17f47-258">Possible values are: `notConfigured`, `userContentOnly`, `sharedContentOnly`.</span></span>|
|<span data-ttu-id="17f47-259">contentCachingMaxSizeBytes</span><span class="sxs-lookup"><span data-stu-id="17f47-259">contentCachingMaxSizeBytes</span></span>|<span data-ttu-id="17f47-260">Int32</span><span class="sxs-lookup"><span data-stu-id="17f47-260">Int32</span></span>|<span data-ttu-id="17f47-261">将用于内容缓存的磁盘空间的最大字节数。</span><span class="sxs-lookup"><span data-stu-id="17f47-261">The maximum number of bytes of disk space that will be used for the content cache.</span></span> <span data-ttu-id="17f47-262">值 0 (默认值) 指示不受限制的磁盘空间。</span><span class="sxs-lookup"><span data-stu-id="17f47-262">A value of 0 (default) indicates unlimited disk space.</span></span> |
|<span data-ttu-id="17f47-263">contentCachingDataPath</span><span class="sxs-lookup"><span data-stu-id="17f47-263">contentCachingDataPath</span></span>|<span data-ttu-id="17f47-264">String</span><span class="sxs-lookup"><span data-stu-id="17f47-264">String</span></span>|<span data-ttu-id="17f47-265">用于存储缓存内容的目录的路径。</span><span class="sxs-lookup"><span data-stu-id="17f47-265">The path to the directory used to store cached content.</span></span> <span data-ttu-id="17f47-266">该值必须是 (或 end with) /Library/Application 支持/Apple/AssetCache/Data</span><span class="sxs-lookup"><span data-stu-id="17f47-266">The value must be (or end with) /Library/Application Support/Apple/AssetCache/Data</span></span>|
|<span data-ttu-id="17f47-267">contentCachingDisableConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="17f47-267">contentCachingDisableConnectionSharing</span></span>|<span data-ttu-id="17f47-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-268">Boolean</span></span>|<span data-ttu-id="17f47-269">禁用 internet 连接共享。</span><span class="sxs-lookup"><span data-stu-id="17f47-269">Disables internet connection sharing.</span></span>|
|<span data-ttu-id="17f47-270">contentCachingForceConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="17f47-270">contentCachingForceConnectionSharing</span></span>|<span data-ttu-id="17f47-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-271">Boolean</span></span>|<span data-ttu-id="17f47-272">强制 internet 连接共享。</span><span class="sxs-lookup"><span data-stu-id="17f47-272">Forces internet connection sharing.</span></span> <span data-ttu-id="17f47-273">contentCachingDisableConnectionSharing 将覆盖此设置。</span><span class="sxs-lookup"><span data-stu-id="17f47-273">contentCachingDisableConnectionSharing overrides this setting.</span></span>|
|<span data-ttu-id="17f47-274">contentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="17f47-274">contentCachingClientPolicy</span></span>|[<span data-ttu-id="17f47-275">macOSContentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="17f47-275">macOSContentCachingClientPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingclientpolicy.md)|<span data-ttu-id="17f47-276">确定内容缓存服务器将在其中侦听客户端的方法。</span><span class="sxs-lookup"><span data-stu-id="17f47-276">Determines the method in which content caching servers will listen for clients.</span></span> <span data-ttu-id="17f47-277">可取值为：`notConfigured`、`clientsInLocalNetwork`、`clientsWithSamePublicIpAddress`、`clientsInCustomLocalNetworks`、`clientsInCustomLocalNetworksWithFallback`。</span><span class="sxs-lookup"><span data-stu-id="17f47-277">Possible values are: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.</span></span>|
|<span data-ttu-id="17f47-278">contentCachingClientListenRanges</span><span class="sxs-lookup"><span data-stu-id="17f47-278">contentCachingClientListenRanges</span></span>|<span data-ttu-id="17f47-279">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17f47-279">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="17f47-280">自定义 IP 范围的列表将用于侦听客户端。</span><span class="sxs-lookup"><span data-stu-id="17f47-280">A list of custom IP ranges content caches will use to listen for clients.</span></span> <span data-ttu-id="17f47-281">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="17f47-281">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="17f47-282">contentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="17f47-282">contentCachingPeerPolicy</span></span>|[<span data-ttu-id="17f47-283">macOSContentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="17f47-283">macOSContentCachingPeerPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingpeerpolicy.md)|<span data-ttu-id="17f47-284">确定内容缓存对等方和其他缓存的方法。</span><span class="sxs-lookup"><span data-stu-id="17f47-284">Determines the method in which content caches peer with other caches.</span></span> <span data-ttu-id="17f47-285">可取值为：`notConfigured`、`peersInLocalNetwork`、`peersWithSamePublicIpAddress`、`peersInCustomLocalNetworks`。</span><span class="sxs-lookup"><span data-stu-id="17f47-285">Possible values are: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.</span></span>|
|<span data-ttu-id="17f47-286">contentCachingPeerListenRanges</span><span class="sxs-lookup"><span data-stu-id="17f47-286">contentCachingPeerListenRanges</span></span>|<span data-ttu-id="17f47-287">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17f47-287">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="17f47-288">将使用自定义 IP 范围的列表来侦听对等缓存的内容缓存。</span><span class="sxs-lookup"><span data-stu-id="17f47-288">A list of custom IP ranges content caches will use to listen for peer caches.</span></span> <span data-ttu-id="17f47-289">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="17f47-289">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="17f47-290">contentCachingPeerFilterRanges</span><span class="sxs-lookup"><span data-stu-id="17f47-290">contentCachingPeerFilterRanges</span></span>|<span data-ttu-id="17f47-291">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17f47-291">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="17f47-292">自定义 IP 范围的列表中，内容缓存将用于查询来自对等缓存的内容。</span><span class="sxs-lookup"><span data-stu-id="17f47-292">A list of custom IP ranges content caches will use to query for content from peers caches.</span></span> <span data-ttu-id="17f47-293">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="17f47-293">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="17f47-294">contentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="17f47-294">contentCachingParentSelectionPolicy</span></span>|[<span data-ttu-id="17f47-295">macOSContentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="17f47-295">macOSContentCachingParentSelectionPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingparentselectionpolicy.md)|<span data-ttu-id="17f47-296">确定内容缓存服务器将选择父项（如果有多个）的方法。</span><span class="sxs-lookup"><span data-stu-id="17f47-296">Determines the method in which content caching servers will select parents if multiple are present.</span></span> <span data-ttu-id="17f47-297">可取值为：`notConfigured`、`roundRobin`、`firstAvailable`、`urlPathHash`、`random`、`stickyAvailable`。</span><span class="sxs-lookup"><span data-stu-id="17f47-297">Possible values are: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.</span></span>|
|<span data-ttu-id="17f47-298">contentCachingParents</span><span class="sxs-lookup"><span data-stu-id="17f47-298">contentCachingParents</span></span>|<span data-ttu-id="17f47-299">String 集合</span><span class="sxs-lookup"><span data-stu-id="17f47-299">String collection</span></span>|<span data-ttu-id="17f47-300">表示父内容缓存的 IP 地址的列表。</span><span class="sxs-lookup"><span data-stu-id="17f47-300">A list of IP addresses representing parent content caches.</span></span>|
|<span data-ttu-id="17f47-301">contentCachingLogClientIdentities</span><span class="sxs-lookup"><span data-stu-id="17f47-301">contentCachingLogClientIdentities</span></span>|<span data-ttu-id="17f47-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-302">Boolean</span></span>|<span data-ttu-id="17f47-303">启用对请求缓存内容的客户端的 IP 地址和端口的日志记录。</span><span class="sxs-lookup"><span data-stu-id="17f47-303">Enables logging of IP addresses and ports of clients that request cached content.</span></span>|
|<span data-ttu-id="17f47-304">contentCachingPublicRanges</span><span class="sxs-lookup"><span data-stu-id="17f47-304">contentCachingPublicRanges</span></span>|<span data-ttu-id="17f47-305">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17f47-305">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="17f47-306">Apple 的内容缓存服务应用于将客户端与内容缓存匹配的自定义 IP 范围的列表。</span><span class="sxs-lookup"><span data-stu-id="17f47-306">A list of custom IP ranges that Apple's content caching service should use to match clients to content caches.</span></span> <span data-ttu-id="17f47-307">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="17f47-307">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="17f47-308">contentCachingBlockDeletion</span><span class="sxs-lookup"><span data-stu-id="17f47-308">contentCachingBlockDeletion</span></span>|<span data-ttu-id="17f47-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-309">Boolean</span></span>|<span data-ttu-id="17f47-310">防止内容缓存清除内容以释放磁盘空间以用于其他应用程序。</span><span class="sxs-lookup"><span data-stu-id="17f47-310">Prevents content caches from purging content to free up disk space for other apps.</span></span>|
|<span data-ttu-id="17f47-311">contentCachingShowAlerts</span><span class="sxs-lookup"><span data-stu-id="17f47-311">contentCachingShowAlerts</span></span>|<span data-ttu-id="17f47-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-312">Boolean</span></span>|<span data-ttu-id="17f47-313">将内容缓存警报显示为系统通知。</span><span class="sxs-lookup"><span data-stu-id="17f47-313">Display content caching alerts as system notifications.</span></span>|
|<span data-ttu-id="17f47-314">contentCachingKeepAwake</span><span class="sxs-lookup"><span data-stu-id="17f47-314">contentCachingKeepAwake</span></span>|<span data-ttu-id="17f47-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="17f47-315">Boolean</span></span>|<span data-ttu-id="17f47-316">如果启用了内容缓存，则阻止设备进入睡眠状态。</span><span class="sxs-lookup"><span data-stu-id="17f47-316">Prevent the device from sleeping if content caching is enabled.</span></span>|
|<span data-ttu-id="17f47-317">contentCachingPort</span><span class="sxs-lookup"><span data-stu-id="17f47-317">contentCachingPort</span></span>|<span data-ttu-id="17f47-318">Int32</span><span class="sxs-lookup"><span data-stu-id="17f47-318">Int32</span></span>|<span data-ttu-id="17f47-319">设置用于内容缓存的端口。</span><span class="sxs-lookup"><span data-stu-id="17f47-319">Sets the port used for content caching.</span></span> <span data-ttu-id="17f47-320">如果值为0，则将选择随机可用端口。</span><span class="sxs-lookup"><span data-stu-id="17f47-320">If the value is 0, a random available port will be selected.</span></span> <span data-ttu-id="17f47-321">有效值为0至65535</span><span class="sxs-lookup"><span data-stu-id="17f47-321">Valid values 0 to 65535</span></span>|



## <a name="response"></a><span data-ttu-id="17f47-322">响应</span><span class="sxs-lookup"><span data-stu-id="17f47-322">Response</span></span>
<span data-ttu-id="17f47-323">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="17f47-323">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17f47-324">示例</span><span class="sxs-lookup"><span data-stu-id="17f47-324">Example</span></span>

### <a name="request"></a><span data-ttu-id="17f47-325">请求</span><span class="sxs-lookup"><span data-stu-id="17f47-325">Request</span></span>
<span data-ttu-id="17f47-326">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="17f47-326">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="17f47-327">响应</span><span class="sxs-lookup"><span data-stu-id="17f47-327">Response</span></span>
<span data-ttu-id="17f47-p129">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="17f47-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






