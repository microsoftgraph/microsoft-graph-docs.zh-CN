---
title: 更新 windowsKioskConfiguration
description: 更新 windowsKioskConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b76505bbb51318288f19004f30a2107f6b3c360f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721995"
---
# <a name="update-windowskioskconfiguration"></a><span data-ttu-id="2ddd8-103">更新 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ddd8-103">Update windowsKioskConfiguration</span></span>

> <span data-ttu-id="2ddd8-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ddd8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ddd8-106">更新[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-106">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ddd8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2ddd8-107">Prerequisites</span></span>
<span data-ttu-id="2ddd8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ddd8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ddd8-110">Permission type</span></span>|<span data-ttu-id="2ddd8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2ddd8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ddd8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ddd8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ddd8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ddd8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2ddd8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ddd8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ddd8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-115">Not supported.</span></span>|
|<span data-ttu-id="2ddd8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ddd8-116">Application</span></span>|<span data-ttu-id="2ddd8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ddd8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ddd8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2ddd8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ddd8-119">Request headers</span></span>
|<span data-ttu-id="2ddd8-120">标头</span><span class="sxs-lookup"><span data-stu-id="2ddd8-120">Header</span></span>|<span data-ttu-id="2ddd8-121">值</span><span class="sxs-lookup"><span data-stu-id="2ddd8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ddd8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ddd8-122">Authorization</span></span>|<span data-ttu-id="2ddd8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ddd8-124">接受</span><span class="sxs-lookup"><span data-stu-id="2ddd8-124">Accept</span></span>|<span data-ttu-id="2ddd8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ddd8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ddd8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ddd8-126">Request body</span></span>
<span data-ttu-id="2ddd8-127">在请求正文中, 提供[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-127">In the request body, supply a JSON representation for the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

<span data-ttu-id="2ddd8-128">下表显示创建[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-128">The following table shows the properties that are required when you create the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>

|<span data-ttu-id="2ddd8-129">属性</span><span class="sxs-lookup"><span data-stu-id="2ddd8-129">Property</span></span>|<span data-ttu-id="2ddd8-130">类型</span><span class="sxs-lookup"><span data-stu-id="2ddd8-130">Type</span></span>|<span data-ttu-id="2ddd8-131">说明</span><span class="sxs-lookup"><span data-stu-id="2ddd8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ddd8-132">id</span><span class="sxs-lookup"><span data-stu-id="2ddd8-132">id</span></span>|<span data-ttu-id="2ddd8-133">字符串</span><span class="sxs-lookup"><span data-stu-id="2ddd8-133">String</span></span>|<span data-ttu-id="2ddd8-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-134">Key of the entity.</span></span> <span data-ttu-id="2ddd8-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ddd8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ddd8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ddd8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2ddd8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ddd8-137">DateTimeOffset</span></span>|<span data-ttu-id="2ddd8-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2ddd8-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ddd8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ddd8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2ddd8-140">roleScopeTagIds</span></span>|<span data-ttu-id="2ddd8-141">String collection</span><span class="sxs-lookup"><span data-stu-id="2ddd8-141">String collection</span></span>|<span data-ttu-id="2ddd8-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2ddd8-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ddd8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ddd8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2ddd8-144">supportsScopeTags</span></span>|<span data-ttu-id="2ddd8-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ddd8-145">Boolean</span></span>|<span data-ttu-id="2ddd8-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2ddd8-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2ddd8-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2ddd8-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-149">This property is read-only.</span></span> <span data-ttu-id="2ddd8-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ddd8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ddd8-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2ddd8-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2ddd8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2ddd8-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2ddd8-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2ddd8-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ddd8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ddd8-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2ddd8-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2ddd8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2ddd8-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2ddd8-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2ddd8-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ddd8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ddd8-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2ddd8-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2ddd8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2ddd8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2ddd8-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2ddd8-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ddd8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ddd8-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ddd8-163">createdDateTime</span></span>|<span data-ttu-id="2ddd8-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ddd8-164">DateTimeOffset</span></span>|<span data-ttu-id="2ddd8-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-165">DateTime the object was created.</span></span> <span data-ttu-id="2ddd8-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ddd8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ddd8-167">说明</span><span class="sxs-lookup"><span data-stu-id="2ddd8-167">description</span></span>|<span data-ttu-id="2ddd8-168">String</span><span class="sxs-lookup"><span data-stu-id="2ddd8-168">String</span></span>|<span data-ttu-id="2ddd8-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2ddd8-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ddd8-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ddd8-171">displayName</span><span class="sxs-lookup"><span data-stu-id="2ddd8-171">displayName</span></span>|<span data-ttu-id="2ddd8-172">String</span><span class="sxs-lookup"><span data-stu-id="2ddd8-172">String</span></span>|<span data-ttu-id="2ddd8-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2ddd8-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ddd8-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ddd8-175">version</span><span class="sxs-lookup"><span data-stu-id="2ddd8-175">version</span></span>|<span data-ttu-id="2ddd8-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2ddd8-176">Int32</span></span>|<span data-ttu-id="2ddd8-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-177">Version of the device configuration.</span></span> <span data-ttu-id="2ddd8-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ddd8-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ddd8-179">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="2ddd8-179">kioskProfiles</span></span>|<span data-ttu-id="2ddd8-180">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="2ddd8-180">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="2ddd8-181">此策略设置允许为展台配置定义展台配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-181">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="2ddd8-182">此集合最多可包含3个元素。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-182">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="2ddd8-183">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="2ddd8-183">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="2ddd8-184">String</span><span class="sxs-lookup"><span data-stu-id="2ddd8-184">String</span></span>|<span data-ttu-id="2ddd8-185">指定浏览器在启动时应导航到的默认 URL。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-185">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="2ddd8-186">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="2ddd8-186">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="2ddd8-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ddd8-187">Boolean</span></span>|<span data-ttu-id="2ddd8-188">启用展台浏览器的 "主页" 按钮。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-188">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="2ddd8-189">默认情况下, "主页" 按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-189">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="2ddd8-190">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="2ddd8-190">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="2ddd8-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ddd8-191">Boolean</span></span>|<span data-ttu-id="2ddd8-192">启用展台浏览器的导航按钮 (前进/后退)。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-192">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="2ddd8-193">默认情况下, 导航按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-193">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="2ddd8-194">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="2ddd8-194">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="2ddd8-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ddd8-195">Boolean</span></span>|<span data-ttu-id="2ddd8-196">启用展台浏览器的结束会话按钮。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-196">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="2ddd8-197">默认情况下, "结束会话" 按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-197">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="2ddd8-198">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="2ddd8-198">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="2ddd8-199">Int32</span><span class="sxs-lookup"><span data-stu-id="2ddd8-199">Int32</span></span>|<span data-ttu-id="2ddd8-200">指定在展台浏览器以全新状态重新启动之前会话处于空闲状态的分钟数。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-200">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="2ddd8-201">有效值为1-1440。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-201">Valid values are 1-1440.</span></span> <span data-ttu-id="2ddd8-202">有效值为1至1440</span><span class="sxs-lookup"><span data-stu-id="2ddd8-202">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="2ddd8-203">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="2ddd8-203">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="2ddd8-204">String collection</span><span class="sxs-lookup"><span data-stu-id="2ddd8-204">String collection</span></span>|<span data-ttu-id="2ddd8-205">指定展台浏览器不应导航到的 Url</span><span class="sxs-lookup"><span data-stu-id="2ddd8-205">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="2ddd8-206">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="2ddd8-206">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="2ddd8-207">String collection</span><span class="sxs-lookup"><span data-stu-id="2ddd8-207">String collection</span></span>|<span data-ttu-id="2ddd8-208">指定展台浏览器允许其导航到的 Url</span><span class="sxs-lookup"><span data-stu-id="2ddd8-208">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="2ddd8-209">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="2ddd8-209">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="2ddd8-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ddd8-210">Boolean</span></span>|<span data-ttu-id="2ddd8-211">为 Microsoft Edge 浏览器启用公共浏览展台模式。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-211">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="2ddd8-212">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-212">The Default is false.</span></span>|
|<span data-ttu-id="2ddd8-213">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="2ddd8-213">windowsKioskForceUpdateSchedule</span></span>|[<span data-ttu-id="2ddd8-214">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="2ddd8-214">windowsKioskForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windowskioskforceupdateschedule.md)|<span data-ttu-id="2ddd8-215">强制更新对展台设备的计划。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-215">force update schedule for Kiosk devices.</span></span>|



## <a name="response"></a><span data-ttu-id="2ddd8-216">响应</span><span class="sxs-lookup"><span data-stu-id="2ddd8-216">Response</span></span>
<span data-ttu-id="2ddd8-217">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-217">If successful, this method returns a `200 OK` response code and an updated [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ddd8-218">示例</span><span class="sxs-lookup"><span data-stu-id="2ddd8-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ddd8-219">请求</span><span class="sxs-lookup"><span data-stu-id="2ddd8-219">Request</span></span>
<span data-ttu-id="2ddd8-220">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-220">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2829

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
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
  "kioskProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsKioskProfile",
      "profileId": "Profile Id value",
      "profileName": "Profile Name value",
      "appConfiguration": {
        "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
        "apps": [
          {
            "@odata.type": "microsoft.graph.windowsKioskUWPApp",
            "startLayoutTileSize": "small",
            "name": "Name value",
            "appType": "store",
            "autoLaunch": true,
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
        "allowAccessToDownloadsFolder": true,
        "disallowDesktopApps": true,
        "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
      },
      "userAccountsConfiguration": [
        {
          "@odata.type": "microsoft.graph.windowsKioskVisitor"
        }
      ]
    }
  ],
  "kioskBrowserDefaultUrl": "https://example.com/kioskBrowserDefaultUrl/",
  "kioskBrowserEnableHomeButton": true,
  "kioskBrowserEnableNavigationButtons": true,
  "kioskBrowserEnableEndSessionButton": true,
  "kioskBrowserRestartOnIdleTimeInMinutes": 6,
  "kioskBrowserBlockedURLs": [
    "Kiosk Browser Blocked URLs value"
  ],
  "kioskBrowserBlockedUrlExceptions": [
    "Kiosk Browser Blocked Url Exceptions value"
  ],
  "edgeKioskEnablePublicBrowsing": true,
  "windowsKioskForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "dayofWeek": "monday",
    "dayofMonth": 10,
    "runImmediatelyIfAfterStartDateTime": true
  }
}
```

### <a name="response"></a><span data-ttu-id="2ddd8-221">响应</span><span class="sxs-lookup"><span data-stu-id="2ddd8-221">Response</span></span>
<span data-ttu-id="2ddd8-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2ddd8-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3001

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
  "id": "146a990b-990b-146a-0b99-6a140b996a14",
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
  "kioskProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsKioskProfile",
      "profileId": "Profile Id value",
      "profileName": "Profile Name value",
      "appConfiguration": {
        "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
        "apps": [
          {
            "@odata.type": "microsoft.graph.windowsKioskUWPApp",
            "startLayoutTileSize": "small",
            "name": "Name value",
            "appType": "store",
            "autoLaunch": true,
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
        "allowAccessToDownloadsFolder": true,
        "disallowDesktopApps": true,
        "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
      },
      "userAccountsConfiguration": [
        {
          "@odata.type": "microsoft.graph.windowsKioskVisitor"
        }
      ]
    }
  ],
  "kioskBrowserDefaultUrl": "https://example.com/kioskBrowserDefaultUrl/",
  "kioskBrowserEnableHomeButton": true,
  "kioskBrowserEnableNavigationButtons": true,
  "kioskBrowserEnableEndSessionButton": true,
  "kioskBrowserRestartOnIdleTimeInMinutes": 6,
  "kioskBrowserBlockedURLs": [
    "Kiosk Browser Blocked URLs value"
  ],
  "kioskBrowserBlockedUrlExceptions": [
    "Kiosk Browser Blocked Url Exceptions value"
  ],
  "edgeKioskEnablePublicBrowsing": true,
  "windowsKioskForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "dayofWeek": "monday",
    "dayofMonth": 10,
    "runImmediatelyIfAfterStartDateTime": true
  }
}
```





