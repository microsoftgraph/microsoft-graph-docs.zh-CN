---
title: 创建 windowsKioskConfiguration
description: 创建新的 windowsKioskConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ea00cec81315b8b260db4b571c593df0718c3161
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42475759"
---
# <a name="create-windowskioskconfiguration"></a><span data-ttu-id="1b7af-103">创建 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="1b7af-103">Create windowsKioskConfiguration</span></span>

<span data-ttu-id="1b7af-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1b7af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b7af-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1b7af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b7af-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1b7af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b7af-107">创建新的[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1b7af-107">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b7af-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1b7af-108">Prerequisites</span></span>
<span data-ttu-id="1b7af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b7af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b7af-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b7af-111">Permission type</span></span>|<span data-ttu-id="1b7af-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1b7af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b7af-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b7af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b7af-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b7af-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b7af-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b7af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b7af-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b7af-116">Not supported.</span></span>|
|<span data-ttu-id="1b7af-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b7af-117">Application</span></span>|<span data-ttu-id="1b7af-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b7af-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b7af-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b7af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1b7af-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b7af-120">Request headers</span></span>
|<span data-ttu-id="1b7af-121">标头</span><span class="sxs-lookup"><span data-stu-id="1b7af-121">Header</span></span>|<span data-ttu-id="1b7af-122">值</span><span class="sxs-lookup"><span data-stu-id="1b7af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b7af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b7af-123">Authorization</span></span>|<span data-ttu-id="1b7af-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1b7af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b7af-125">接受</span><span class="sxs-lookup"><span data-stu-id="1b7af-125">Accept</span></span>|<span data-ttu-id="1b7af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b7af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b7af-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b7af-127">Request body</span></span>
<span data-ttu-id="1b7af-128">在请求正文中，提供 windowsKioskConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b7af-128">In the request body, supply a JSON representation for the windowsKioskConfiguration object.</span></span>

<span data-ttu-id="1b7af-129">下表显示创建 windowsKioskConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1b7af-129">The following table shows the properties that are required when you create the windowsKioskConfiguration.</span></span>

|<span data-ttu-id="1b7af-130">属性</span><span class="sxs-lookup"><span data-stu-id="1b7af-130">Property</span></span>|<span data-ttu-id="1b7af-131">类型</span><span class="sxs-lookup"><span data-stu-id="1b7af-131">Type</span></span>|<span data-ttu-id="1b7af-132">说明</span><span class="sxs-lookup"><span data-stu-id="1b7af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b7af-133">id</span><span class="sxs-lookup"><span data-stu-id="1b7af-133">id</span></span>|<span data-ttu-id="1b7af-134">字符串</span><span class="sxs-lookup"><span data-stu-id="1b7af-134">String</span></span>|<span data-ttu-id="1b7af-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1b7af-135">Key of the entity.</span></span> <span data-ttu-id="1b7af-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b7af-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b7af-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b7af-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1b7af-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b7af-138">DateTimeOffset</span></span>|<span data-ttu-id="1b7af-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1b7af-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1b7af-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b7af-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b7af-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1b7af-141">roleScopeTagIds</span></span>|<span data-ttu-id="1b7af-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="1b7af-142">String collection</span></span>|<span data-ttu-id="1b7af-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1b7af-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1b7af-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b7af-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b7af-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1b7af-145">supportsScopeTags</span></span>|<span data-ttu-id="1b7af-146">布尔</span><span class="sxs-lookup"><span data-stu-id="1b7af-146">Boolean</span></span>|<span data-ttu-id="1b7af-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="1b7af-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1b7af-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="1b7af-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1b7af-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="1b7af-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1b7af-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1b7af-150">This property is read-only.</span></span> <span data-ttu-id="1b7af-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b7af-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b7af-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1b7af-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1b7af-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1b7af-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1b7af-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="1b7af-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1b7af-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b7af-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b7af-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1b7af-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1b7af-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1b7af-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1b7af-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1b7af-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1b7af-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b7af-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b7af-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1b7af-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1b7af-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1b7af-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1b7af-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1b7af-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1b7af-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b7af-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b7af-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b7af-164">createdDateTime</span></span>|<span data-ttu-id="1b7af-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b7af-165">DateTimeOffset</span></span>|<span data-ttu-id="1b7af-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1b7af-166">DateTime the object was created.</span></span> <span data-ttu-id="1b7af-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b7af-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b7af-168">说明</span><span class="sxs-lookup"><span data-stu-id="1b7af-168">description</span></span>|<span data-ttu-id="1b7af-169">String</span><span class="sxs-lookup"><span data-stu-id="1b7af-169">String</span></span>|<span data-ttu-id="1b7af-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1b7af-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1b7af-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b7af-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b7af-172">displayName</span><span class="sxs-lookup"><span data-stu-id="1b7af-172">displayName</span></span>|<span data-ttu-id="1b7af-173">String</span><span class="sxs-lookup"><span data-stu-id="1b7af-173">String</span></span>|<span data-ttu-id="1b7af-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1b7af-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1b7af-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b7af-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b7af-176">version</span><span class="sxs-lookup"><span data-stu-id="1b7af-176">version</span></span>|<span data-ttu-id="1b7af-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1b7af-177">Int32</span></span>|<span data-ttu-id="1b7af-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1b7af-178">Version of the device configuration.</span></span> <span data-ttu-id="1b7af-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b7af-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b7af-180">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="1b7af-180">kioskProfiles</span></span>|<span data-ttu-id="1b7af-181">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="1b7af-181">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="1b7af-182">此策略设置允许为展台配置定义展台配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="1b7af-182">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="1b7af-183">此集合最多可包含3个元素。</span><span class="sxs-lookup"><span data-stu-id="1b7af-183">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="1b7af-184">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="1b7af-184">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="1b7af-185">String</span><span class="sxs-lookup"><span data-stu-id="1b7af-185">String</span></span>|<span data-ttu-id="1b7af-186">指定浏览器在启动时应导航到的默认 URL。</span><span class="sxs-lookup"><span data-stu-id="1b7af-186">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="1b7af-187">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="1b7af-187">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="1b7af-188">布尔</span><span class="sxs-lookup"><span data-stu-id="1b7af-188">Boolean</span></span>|<span data-ttu-id="1b7af-189">启用展台浏览器的 "主页" 按钮。</span><span class="sxs-lookup"><span data-stu-id="1b7af-189">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="1b7af-190">默认情况下，"主页" 按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="1b7af-190">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="1b7af-191">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="1b7af-191">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="1b7af-192">布尔</span><span class="sxs-lookup"><span data-stu-id="1b7af-192">Boolean</span></span>|<span data-ttu-id="1b7af-193">启用展台浏览器的导航按钮（前进/后退）。</span><span class="sxs-lookup"><span data-stu-id="1b7af-193">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="1b7af-194">默认情况下，导航按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="1b7af-194">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="1b7af-195">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="1b7af-195">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="1b7af-196">布尔</span><span class="sxs-lookup"><span data-stu-id="1b7af-196">Boolean</span></span>|<span data-ttu-id="1b7af-197">启用展台浏览器的结束会话按钮。</span><span class="sxs-lookup"><span data-stu-id="1b7af-197">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="1b7af-198">默认情况下，"结束会话" 按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="1b7af-198">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="1b7af-199">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="1b7af-199">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="1b7af-200">Int32</span><span class="sxs-lookup"><span data-stu-id="1b7af-200">Int32</span></span>|<span data-ttu-id="1b7af-201">指定在展台浏览器以全新状态重新启动之前会话处于空闲状态的分钟数。</span><span class="sxs-lookup"><span data-stu-id="1b7af-201">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="1b7af-202">有效值为1-1440。</span><span class="sxs-lookup"><span data-stu-id="1b7af-202">Valid values are 1-1440.</span></span> <span data-ttu-id="1b7af-203">有效值为1至1440</span><span class="sxs-lookup"><span data-stu-id="1b7af-203">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="1b7af-204">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="1b7af-204">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="1b7af-205">String 集合</span><span class="sxs-lookup"><span data-stu-id="1b7af-205">String collection</span></span>|<span data-ttu-id="1b7af-206">指定展台浏览器不应导航到的 Url</span><span class="sxs-lookup"><span data-stu-id="1b7af-206">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="1b7af-207">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="1b7af-207">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="1b7af-208">String 集合</span><span class="sxs-lookup"><span data-stu-id="1b7af-208">String collection</span></span>|<span data-ttu-id="1b7af-209">指定展台浏览器允许其导航到的 Url</span><span class="sxs-lookup"><span data-stu-id="1b7af-209">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="1b7af-210">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="1b7af-210">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="1b7af-211">布尔</span><span class="sxs-lookup"><span data-stu-id="1b7af-211">Boolean</span></span>|<span data-ttu-id="1b7af-212">为 Microsoft Edge 浏览器启用公共浏览展台模式。</span><span class="sxs-lookup"><span data-stu-id="1b7af-212">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="1b7af-213">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="1b7af-213">The Default is false.</span></span>|
|<span data-ttu-id="1b7af-214">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="1b7af-214">windowsKioskForceUpdateSchedule</span></span>|[<span data-ttu-id="1b7af-215">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="1b7af-215">windowsKioskForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windowskioskforceupdateschedule.md)|<span data-ttu-id="1b7af-216">强制更新对展台设备的计划。</span><span class="sxs-lookup"><span data-stu-id="1b7af-216">force update schedule for Kiosk devices.</span></span>|



## <a name="response"></a><span data-ttu-id="1b7af-217">响应</span><span class="sxs-lookup"><span data-stu-id="1b7af-217">Response</span></span>
<span data-ttu-id="1b7af-218">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1b7af-218">If successful, this method returns a `201 Created` response code and a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b7af-219">示例</span><span class="sxs-lookup"><span data-stu-id="1b7af-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b7af-220">请求</span><span class="sxs-lookup"><span data-stu-id="1b7af-220">Request</span></span>
<span data-ttu-id="1b7af-221">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1b7af-221">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="1b7af-222">响应</span><span class="sxs-lookup"><span data-stu-id="1b7af-222">Response</span></span>
<span data-ttu-id="1b7af-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1b7af-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





