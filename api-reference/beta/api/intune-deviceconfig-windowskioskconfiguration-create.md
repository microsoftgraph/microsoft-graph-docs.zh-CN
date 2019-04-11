---
title: 创建 windowsKioskConfiguration
description: 创建新的 windowsKioskConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d34e55a4de496eff9d9305c35a4815a2910a2d7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776848"
---
# <a name="create-windowskioskconfiguration"></a><span data-ttu-id="da250-103">创建 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="da250-103">Create windowsKioskConfiguration</span></span>

> <span data-ttu-id="da250-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da250-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da250-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da250-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da250-106">创建新的[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="da250-106">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da250-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="da250-107">Prerequisites</span></span>
<span data-ttu-id="da250-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da250-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da250-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="da250-110">Permission type</span></span>|<span data-ttu-id="da250-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="da250-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da250-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da250-112">Delegated (work or school account)</span></span>|<span data-ttu-id="da250-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da250-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da250-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da250-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da250-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="da250-115">Not supported.</span></span>|
|<span data-ttu-id="da250-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="da250-116">Application</span></span>|<span data-ttu-id="da250-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="da250-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da250-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da250-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="da250-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="da250-119">Request headers</span></span>
|<span data-ttu-id="da250-120">标头</span><span class="sxs-lookup"><span data-stu-id="da250-120">Header</span></span>|<span data-ttu-id="da250-121">值</span><span class="sxs-lookup"><span data-stu-id="da250-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da250-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="da250-122">Authorization</span></span>|<span data-ttu-id="da250-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da250-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da250-124">接受</span><span class="sxs-lookup"><span data-stu-id="da250-124">Accept</span></span>|<span data-ttu-id="da250-125">application/json</span><span class="sxs-lookup"><span data-stu-id="da250-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da250-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="da250-126">Request body</span></span>
<span data-ttu-id="da250-127">在请求正文中, 提供 windowsKioskConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da250-127">In the request body, supply a JSON representation for the windowsKioskConfiguration object.</span></span>

<span data-ttu-id="da250-128">下表显示创建 windowsKioskConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="da250-128">The following table shows the properties that are required when you create the windowsKioskConfiguration.</span></span>

|<span data-ttu-id="da250-129">属性</span><span class="sxs-lookup"><span data-stu-id="da250-129">Property</span></span>|<span data-ttu-id="da250-130">类型</span><span class="sxs-lookup"><span data-stu-id="da250-130">Type</span></span>|<span data-ttu-id="da250-131">说明</span><span class="sxs-lookup"><span data-stu-id="da250-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da250-132">id</span><span class="sxs-lookup"><span data-stu-id="da250-132">id</span></span>|<span data-ttu-id="da250-133">String</span><span class="sxs-lookup"><span data-stu-id="da250-133">String</span></span>|<span data-ttu-id="da250-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="da250-134">Key of the entity.</span></span> <span data-ttu-id="da250-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da250-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da250-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da250-136">lastModifiedDateTime</span></span>|<span data-ttu-id="da250-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da250-137">DateTimeOffset</span></span>|<span data-ttu-id="da250-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="da250-138">DateTime the object was last modified.</span></span> <span data-ttu-id="da250-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da250-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da250-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="da250-140">roleScopeTagIds</span></span>|<span data-ttu-id="da250-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="da250-141">String collection</span></span>|<span data-ttu-id="da250-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="da250-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="da250-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da250-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da250-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="da250-144">supportsScopeTags</span></span>|<span data-ttu-id="da250-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="da250-145">Boolean</span></span>|<span data-ttu-id="da250-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="da250-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="da250-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="da250-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="da250-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="da250-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="da250-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="da250-149">This property is read-only.</span></span> <span data-ttu-id="da250-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da250-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da250-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da250-151">createdDateTime</span></span>|<span data-ttu-id="da250-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da250-152">DateTimeOffset</span></span>|<span data-ttu-id="da250-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="da250-153">DateTime the object was created.</span></span> <span data-ttu-id="da250-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da250-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da250-155">description</span><span class="sxs-lookup"><span data-stu-id="da250-155">description</span></span>|<span data-ttu-id="da250-156">String</span><span class="sxs-lookup"><span data-stu-id="da250-156">String</span></span>|<span data-ttu-id="da250-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="da250-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="da250-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da250-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da250-159">displayName</span><span class="sxs-lookup"><span data-stu-id="da250-159">displayName</span></span>|<span data-ttu-id="da250-160">String</span><span class="sxs-lookup"><span data-stu-id="da250-160">String</span></span>|<span data-ttu-id="da250-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="da250-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="da250-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da250-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da250-163">version</span><span class="sxs-lookup"><span data-stu-id="da250-163">version</span></span>|<span data-ttu-id="da250-164">Int32</span><span class="sxs-lookup"><span data-stu-id="da250-164">Int32</span></span>|<span data-ttu-id="da250-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="da250-165">Version of the device configuration.</span></span> <span data-ttu-id="da250-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da250-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da250-167">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="da250-167">kioskProfiles</span></span>|<span data-ttu-id="da250-168">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="da250-168">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="da250-169">此策略设置允许为展台配置定义展台配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="da250-169">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="da250-170">此集合最多可包含3个元素。</span><span class="sxs-lookup"><span data-stu-id="da250-170">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="da250-171">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="da250-171">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="da250-172">String</span><span class="sxs-lookup"><span data-stu-id="da250-172">String</span></span>|<span data-ttu-id="da250-173">指定浏览器在启动时应导航到的默认 URL。</span><span class="sxs-lookup"><span data-stu-id="da250-173">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="da250-174">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="da250-174">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="da250-175">布尔值</span><span class="sxs-lookup"><span data-stu-id="da250-175">Boolean</span></span>|<span data-ttu-id="da250-176">启用展台浏览器的 "主页" 按钮。</span><span class="sxs-lookup"><span data-stu-id="da250-176">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="da250-177">默认情况下, "主页" 按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="da250-177">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="da250-178">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="da250-178">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="da250-179">布尔值</span><span class="sxs-lookup"><span data-stu-id="da250-179">Boolean</span></span>|<span data-ttu-id="da250-180">启用展台浏览器的导航按钮 (前进/后退)。</span><span class="sxs-lookup"><span data-stu-id="da250-180">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="da250-181">默认情况下, 导航按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="da250-181">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="da250-182">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="da250-182">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="da250-183">布尔值</span><span class="sxs-lookup"><span data-stu-id="da250-183">Boolean</span></span>|<span data-ttu-id="da250-184">启用展台浏览器的结束会话按钮。</span><span class="sxs-lookup"><span data-stu-id="da250-184">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="da250-185">默认情况下, "结束会话" 按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="da250-185">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="da250-186">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="da250-186">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="da250-187">Int32</span><span class="sxs-lookup"><span data-stu-id="da250-187">Int32</span></span>|<span data-ttu-id="da250-188">指定在展台浏览器以全新状态重新启动之前会话处于空闲状态的分钟数。</span><span class="sxs-lookup"><span data-stu-id="da250-188">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="da250-189">有效值为1-1440。</span><span class="sxs-lookup"><span data-stu-id="da250-189">Valid values are 1-1440.</span></span> <span data-ttu-id="da250-190">有效值为1至1440</span><span class="sxs-lookup"><span data-stu-id="da250-190">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="da250-191">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="da250-191">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="da250-192">String 集合</span><span class="sxs-lookup"><span data-stu-id="da250-192">String collection</span></span>|<span data-ttu-id="da250-193">指定展台浏览器不应导航到的 url</span><span class="sxs-lookup"><span data-stu-id="da250-193">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="da250-194">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="da250-194">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="da250-195">String 集合</span><span class="sxs-lookup"><span data-stu-id="da250-195">String collection</span></span>|<span data-ttu-id="da250-196">指定展台浏览器允许其导航到的 url</span><span class="sxs-lookup"><span data-stu-id="da250-196">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="da250-197">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="da250-197">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="da250-198">布尔值</span><span class="sxs-lookup"><span data-stu-id="da250-198">Boolean</span></span>|<span data-ttu-id="da250-199">为 Microsoft Edge 浏览器启用公共浏览展台模式。</span><span class="sxs-lookup"><span data-stu-id="da250-199">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="da250-200">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="da250-200">The Default is false.</span></span>|



## <a name="response"></a><span data-ttu-id="da250-201">响应</span><span class="sxs-lookup"><span data-stu-id="da250-201">Response</span></span>
<span data-ttu-id="da250-202">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="da250-202">If successful, this method returns a `201 Created` response code and a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da250-203">示例</span><span class="sxs-lookup"><span data-stu-id="da250-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="da250-204">请求</span><span class="sxs-lookup"><span data-stu-id="da250-204">Request</span></span>
<span data-ttu-id="da250-205">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da250-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1753

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
  "edgeKioskEnablePublicBrowsing": true
}
```

### <a name="response"></a><span data-ttu-id="da250-206">响应</span><span class="sxs-lookup"><span data-stu-id="da250-206">Response</span></span>
<span data-ttu-id="da250-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da250-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1925

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
  "edgeKioskEnablePublicBrowsing": true
}
```





