---
title: 创建 windowsKioskConfiguration
description: 创建新的 windowsKioskConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dd32b23626c027cfc4a9cdac60b5a5a4a6c37973
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160744"
---
# <a name="create-windowskioskconfiguration"></a><span data-ttu-id="4eeac-103">创建 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="4eeac-103">Create windowsKioskConfiguration</span></span>

> <span data-ttu-id="4eeac-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4eeac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4eeac-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4eeac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4eeac-106">创建新的[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4eeac-106">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4eeac-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4eeac-107">Prerequisites</span></span>
<span data-ttu-id="4eeac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4eeac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4eeac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4eeac-110">Permission type</span></span>|<span data-ttu-id="4eeac-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4eeac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4eeac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4eeac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4eeac-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eeac-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4eeac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4eeac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4eeac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4eeac-115">Not supported.</span></span>|
|<span data-ttu-id="4eeac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4eeac-116">Application</span></span>|<span data-ttu-id="4eeac-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4eeac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4eeac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4eeac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4eeac-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4eeac-119">Request headers</span></span>
|<span data-ttu-id="4eeac-120">标头</span><span class="sxs-lookup"><span data-stu-id="4eeac-120">Header</span></span>|<span data-ttu-id="4eeac-121">值</span><span class="sxs-lookup"><span data-stu-id="4eeac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4eeac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4eeac-122">Authorization</span></span>|<span data-ttu-id="4eeac-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4eeac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4eeac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4eeac-124">Accept</span></span>|<span data-ttu-id="4eeac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4eeac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4eeac-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4eeac-126">Request body</span></span>
<span data-ttu-id="4eeac-127">在请求正文中, 提供 windowsKioskConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4eeac-127">In the request body, supply a JSON representation for the windowsKioskConfiguration object.</span></span>

<span data-ttu-id="4eeac-128">下表显示创建 windowsKioskConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4eeac-128">The following table shows the properties that are required when you create the windowsKioskConfiguration.</span></span>

|<span data-ttu-id="4eeac-129">属性</span><span class="sxs-lookup"><span data-stu-id="4eeac-129">Property</span></span>|<span data-ttu-id="4eeac-130">类型</span><span class="sxs-lookup"><span data-stu-id="4eeac-130">Type</span></span>|<span data-ttu-id="4eeac-131">说明</span><span class="sxs-lookup"><span data-stu-id="4eeac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eeac-132">id</span><span class="sxs-lookup"><span data-stu-id="4eeac-132">id</span></span>|<span data-ttu-id="4eeac-133">String</span><span class="sxs-lookup"><span data-stu-id="4eeac-133">String</span></span>|<span data-ttu-id="4eeac-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4eeac-134">Key of the entity.</span></span> <span data-ttu-id="4eeac-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4eeac-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eeac-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4eeac-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4eeac-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eeac-137">DateTimeOffset</span></span>|<span data-ttu-id="4eeac-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4eeac-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4eeac-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4eeac-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eeac-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4eeac-140">roleScopeTagIds</span></span>|<span data-ttu-id="4eeac-141">String collection</span><span class="sxs-lookup"><span data-stu-id="4eeac-141">String collection</span></span>|<span data-ttu-id="4eeac-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4eeac-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4eeac-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4eeac-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eeac-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4eeac-144">supportsScopeTags</span></span>|<span data-ttu-id="4eeac-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4eeac-145">Boolean</span></span>|<span data-ttu-id="4eeac-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="4eeac-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4eeac-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="4eeac-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4eeac-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="4eeac-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4eeac-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4eeac-149">This property is read-only.</span></span> <span data-ttu-id="4eeac-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4eeac-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eeac-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4eeac-151">createdDateTime</span></span>|<span data-ttu-id="4eeac-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eeac-152">DateTimeOffset</span></span>|<span data-ttu-id="4eeac-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4eeac-153">DateTime the object was created.</span></span> <span data-ttu-id="4eeac-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4eeac-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eeac-155">description</span><span class="sxs-lookup"><span data-stu-id="4eeac-155">description</span></span>|<span data-ttu-id="4eeac-156">String</span><span class="sxs-lookup"><span data-stu-id="4eeac-156">String</span></span>|<span data-ttu-id="4eeac-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4eeac-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4eeac-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4eeac-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eeac-159">displayName</span><span class="sxs-lookup"><span data-stu-id="4eeac-159">displayName</span></span>|<span data-ttu-id="4eeac-160">String</span><span class="sxs-lookup"><span data-stu-id="4eeac-160">String</span></span>|<span data-ttu-id="4eeac-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4eeac-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4eeac-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4eeac-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eeac-163">version</span><span class="sxs-lookup"><span data-stu-id="4eeac-163">version</span></span>|<span data-ttu-id="4eeac-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4eeac-164">Int32</span></span>|<span data-ttu-id="4eeac-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4eeac-165">Version of the device configuration.</span></span> <span data-ttu-id="4eeac-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4eeac-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eeac-167">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="4eeac-167">kioskProfiles</span></span>|<span data-ttu-id="4eeac-168">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="4eeac-168">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="4eeac-169">此策略设置允许为展台配置定义展台配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="4eeac-169">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="4eeac-170">此集合最多可包含3个元素。</span><span class="sxs-lookup"><span data-stu-id="4eeac-170">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="4eeac-171">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="4eeac-171">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="4eeac-172">String</span><span class="sxs-lookup"><span data-stu-id="4eeac-172">String</span></span>|<span data-ttu-id="4eeac-173">指定浏览器在启动时应导航到的默认 URL。</span><span class="sxs-lookup"><span data-stu-id="4eeac-173">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="4eeac-174">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="4eeac-174">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="4eeac-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="4eeac-175">Boolean</span></span>|<span data-ttu-id="4eeac-176">启用展台浏览器的 "主页" 按钮。</span><span class="sxs-lookup"><span data-stu-id="4eeac-176">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="4eeac-177">默认情况下, "主页" 按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="4eeac-177">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="4eeac-178">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="4eeac-178">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="4eeac-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="4eeac-179">Boolean</span></span>|<span data-ttu-id="4eeac-180">启用展台浏览器的导航按钮 (前进/后退)。</span><span class="sxs-lookup"><span data-stu-id="4eeac-180">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="4eeac-181">默认情况下, 导航按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="4eeac-181">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="4eeac-182">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="4eeac-182">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="4eeac-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="4eeac-183">Boolean</span></span>|<span data-ttu-id="4eeac-184">启用展台浏览器的结束会话按钮。</span><span class="sxs-lookup"><span data-stu-id="4eeac-184">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="4eeac-185">默认情况下, "结束会话" 按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="4eeac-185">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="4eeac-186">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="4eeac-186">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="4eeac-187">Int32</span><span class="sxs-lookup"><span data-stu-id="4eeac-187">Int32</span></span>|<span data-ttu-id="4eeac-188">指定在展台浏览器以全新状态重新启动之前会话处于空闲状态的分钟数。</span><span class="sxs-lookup"><span data-stu-id="4eeac-188">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="4eeac-189">有效值为1-1440。</span><span class="sxs-lookup"><span data-stu-id="4eeac-189">Valid values are 1-1440.</span></span> <span data-ttu-id="4eeac-190">有效值为1至1440</span><span class="sxs-lookup"><span data-stu-id="4eeac-190">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="4eeac-191">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="4eeac-191">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="4eeac-192">String collection</span><span class="sxs-lookup"><span data-stu-id="4eeac-192">String collection</span></span>|<span data-ttu-id="4eeac-193">指定展台浏览器不应导航到的 url</span><span class="sxs-lookup"><span data-stu-id="4eeac-193">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="4eeac-194">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="4eeac-194">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="4eeac-195">String collection</span><span class="sxs-lookup"><span data-stu-id="4eeac-195">String collection</span></span>|<span data-ttu-id="4eeac-196">指定展台浏览器允许其导航到的 url</span><span class="sxs-lookup"><span data-stu-id="4eeac-196">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="4eeac-197">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="4eeac-197">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="4eeac-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="4eeac-198">Boolean</span></span>|<span data-ttu-id="4eeac-199">为 Microsoft Edge 浏览器启用公共浏览展台模式。</span><span class="sxs-lookup"><span data-stu-id="4eeac-199">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="4eeac-200">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="4eeac-200">The Default is false.</span></span>|
|<span data-ttu-id="4eeac-201">edgeKioskResetAfterIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="4eeac-201">edgeKioskResetAfterIdleTimeInMinutes</span></span>|<span data-ttu-id="4eeac-202">Int32</span><span class="sxs-lookup"><span data-stu-id="4eeac-202">Int32</span></span>|<span data-ttu-id="4eeac-203">指定在 Microsoft Edge 展台重置前的上次用户活动的时间 (以分钟为单位)。</span><span class="sxs-lookup"><span data-stu-id="4eeac-203">Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets.</span></span>  <span data-ttu-id="4eeac-204">有效值为0-1440。</span><span class="sxs-lookup"><span data-stu-id="4eeac-204">Valid values are 0-1440.</span></span> <span data-ttu-id="4eeac-205">默认值为 5。</span><span class="sxs-lookup"><span data-stu-id="4eeac-205">The default is 5.</span></span> <span data-ttu-id="4eeac-206">0表示不重置。</span><span class="sxs-lookup"><span data-stu-id="4eeac-206">0 indicates no reset.</span></span> <span data-ttu-id="4eeac-207">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="4eeac-207">Valid values 0 to 1440</span></span>|



## <a name="response"></a><span data-ttu-id="4eeac-208">响应</span><span class="sxs-lookup"><span data-stu-id="4eeac-208">Response</span></span>
<span data-ttu-id="4eeac-209">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4eeac-209">If successful, this method returns a `201 Created` response code and a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4eeac-210">示例</span><span class="sxs-lookup"><span data-stu-id="4eeac-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="4eeac-211">请求</span><span class="sxs-lookup"><span data-stu-id="4eeac-211">Request</span></span>
<span data-ttu-id="4eeac-212">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4eeac-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1719

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
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
  "edgeKioskResetAfterIdleTimeInMinutes": 4
}
```

### <a name="response"></a><span data-ttu-id="4eeac-213">响应</span><span class="sxs-lookup"><span data-stu-id="4eeac-213">Response</span></span>
<span data-ttu-id="4eeac-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4eeac-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1891

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
  "id": "146a990b-990b-146a-0b99-6a140b996a14",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
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
  "edgeKioskResetAfterIdleTimeInMinutes": 4
}
```




