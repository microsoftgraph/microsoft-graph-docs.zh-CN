---
title: 更新 windowsKioskConfiguration
description: 更新 windowsKioskConfiguration 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 767acd4136226e2687977cf09d2c08f6c413fcb8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414884"
---
# <a name="update-windowskioskconfiguration"></a><span data-ttu-id="a2388-103">更新 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="a2388-103">Update windowsKioskConfiguration</span></span>

> <span data-ttu-id="a2388-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a2388-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a2388-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a2388-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2388-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2388-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2388-107">更新[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a2388-107">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2388-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a2388-108">Prerequisites</span></span>
<span data-ttu-id="a2388-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a2388-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a2388-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2388-111">Permission type</span></span>|<span data-ttu-id="a2388-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a2388-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2388-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2388-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2388-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2388-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2388-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2388-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2388-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2388-116">Not supported.</span></span>|
|<span data-ttu-id="a2388-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2388-117">Application</span></span>|<span data-ttu-id="a2388-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2388-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2388-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2388-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a2388-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2388-120">Request headers</span></span>
|<span data-ttu-id="a2388-121">标头</span><span class="sxs-lookup"><span data-stu-id="a2388-121">Header</span></span>|<span data-ttu-id="a2388-122">值</span><span class="sxs-lookup"><span data-stu-id="a2388-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2388-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2388-123">Authorization</span></span>|<span data-ttu-id="a2388-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a2388-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2388-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2388-125">Accept</span></span>|<span data-ttu-id="a2388-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2388-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2388-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2388-127">Request body</span></span>
<span data-ttu-id="a2388-128">在请求正文中，提供[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2388-128">In the request body, supply a JSON representation for the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

<span data-ttu-id="a2388-129">下表显示时创建[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a2388-129">The following table shows the properties that are required when you create the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>

|<span data-ttu-id="a2388-130">属性</span><span class="sxs-lookup"><span data-stu-id="a2388-130">Property</span></span>|<span data-ttu-id="a2388-131">类型</span><span class="sxs-lookup"><span data-stu-id="a2388-131">Type</span></span>|<span data-ttu-id="a2388-132">说明</span><span class="sxs-lookup"><span data-stu-id="a2388-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2388-133">id</span><span class="sxs-lookup"><span data-stu-id="a2388-133">id</span></span>|<span data-ttu-id="a2388-134">String</span><span class="sxs-lookup"><span data-stu-id="a2388-134">String</span></span>|<span data-ttu-id="a2388-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a2388-135">Key of the entity.</span></span> <span data-ttu-id="a2388-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2388-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2388-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2388-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a2388-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2388-138">DateTimeOffset</span></span>|<span data-ttu-id="a2388-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a2388-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a2388-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2388-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2388-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a2388-141">roleScopeTagIds</span></span>|<span data-ttu-id="a2388-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="a2388-142">String collection</span></span>|<span data-ttu-id="a2388-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="a2388-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a2388-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2388-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2388-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a2388-145">supportsScopeTags</span></span>|<span data-ttu-id="a2388-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2388-146">Boolean</span></span>|<span data-ttu-id="a2388-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="a2388-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a2388-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="a2388-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a2388-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="a2388-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a2388-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a2388-150">This property is read-only.</span></span> <span data-ttu-id="a2388-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2388-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2388-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2388-152">createdDateTime</span></span>|<span data-ttu-id="a2388-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2388-153">DateTimeOffset</span></span>|<span data-ttu-id="a2388-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a2388-154">DateTime the object was created.</span></span> <span data-ttu-id="a2388-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2388-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2388-156">description</span><span class="sxs-lookup"><span data-stu-id="a2388-156">description</span></span>|<span data-ttu-id="a2388-157">String</span><span class="sxs-lookup"><span data-stu-id="a2388-157">String</span></span>|<span data-ttu-id="a2388-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a2388-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a2388-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2388-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2388-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a2388-160">displayName</span></span>|<span data-ttu-id="a2388-161">String</span><span class="sxs-lookup"><span data-stu-id="a2388-161">String</span></span>|<span data-ttu-id="a2388-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a2388-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a2388-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2388-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2388-164">version</span><span class="sxs-lookup"><span data-stu-id="a2388-164">version</span></span>|<span data-ttu-id="a2388-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a2388-165">Int32</span></span>|<span data-ttu-id="a2388-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a2388-166">Version of the device configuration.</span></span> <span data-ttu-id="a2388-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2388-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2388-168">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="a2388-168">kioskProfiles</span></span>|<span data-ttu-id="a2388-169">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="a2388-169">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="a2388-170">此策略设置允许定义网亭配置网亭配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="a2388-170">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="a2388-171">此集合可以包含 3 个元素的最大值。</span><span class="sxs-lookup"><span data-stu-id="a2388-171">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="a2388-172">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="a2388-172">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="a2388-173">String</span><span class="sxs-lookup"><span data-stu-id="a2388-173">String</span></span>|<span data-ttu-id="a2388-174">在启动上指定浏览器应导航到的默认 URL。</span><span class="sxs-lookup"><span data-stu-id="a2388-174">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="a2388-175">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="a2388-175">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="a2388-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2388-176">Boolean</span></span>|<span data-ttu-id="a2388-177">启用网亭浏览器的主页按钮。</span><span class="sxs-lookup"><span data-stu-id="a2388-177">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="a2388-178">默认情况下禁用主页按钮。</span><span class="sxs-lookup"><span data-stu-id="a2388-178">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="a2388-179">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="a2388-179">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="a2388-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2388-180">Boolean</span></span>|<span data-ttu-id="a2388-181">启用网亭浏览器的导航 buttons(forward/back)。</span><span class="sxs-lookup"><span data-stu-id="a2388-181">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="a2388-182">默认情况下，禁用导航按钮。</span><span class="sxs-lookup"><span data-stu-id="a2388-182">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="a2388-183">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="a2388-183">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="a2388-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2388-184">Boolean</span></span>|<span data-ttu-id="a2388-185">启用网亭浏览器的结束会话按钮。</span><span class="sxs-lookup"><span data-stu-id="a2388-185">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="a2388-186">默认情况下禁用结束会话按钮。</span><span class="sxs-lookup"><span data-stu-id="a2388-186">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="a2388-187">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="a2388-187">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="a2388-188">Int32</span><span class="sxs-lookup"><span data-stu-id="a2388-188">Int32</span></span>|<span data-ttu-id="a2388-189">指定网亭浏览器中刷新状态重新启动之前，会话处于空闲状态的分钟数。</span><span class="sxs-lookup"><span data-stu-id="a2388-189">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="a2388-190">有效值为 1 1440年。</span><span class="sxs-lookup"><span data-stu-id="a2388-190">Valid values are 1-1440.</span></span> <span data-ttu-id="a2388-191">1 到 1440 之间的有效值</span><span class="sxs-lookup"><span data-stu-id="a2388-191">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="a2388-192">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="a2388-192">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="a2388-193">String 集合</span><span class="sxs-lookup"><span data-stu-id="a2388-193">String collection</span></span>|<span data-ttu-id="a2388-194">指定网亭浏览器不应导航到的 Url</span><span class="sxs-lookup"><span data-stu-id="a2388-194">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="a2388-195">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="a2388-195">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="a2388-196">String 集合</span><span class="sxs-lookup"><span data-stu-id="a2388-196">String collection</span></span>|<span data-ttu-id="a2388-197">指定允许网亭浏览器导航到的 Url</span><span class="sxs-lookup"><span data-stu-id="a2388-197">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="a2388-198">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="a2388-198">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="a2388-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2388-199">Boolean</span></span>|<span data-ttu-id="a2388-200">启用 Microsoft 边缘浏览器的公共浏览展台模式。</span><span class="sxs-lookup"><span data-stu-id="a2388-200">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="a2388-201">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="a2388-201">The Default is false.</span></span>|
|<span data-ttu-id="a2388-202">edgeKioskResetAfterIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="a2388-202">edgeKioskResetAfterIdleTimeInMinutes</span></span>|<span data-ttu-id="a2388-203">Int32</span><span class="sxs-lookup"><span data-stu-id="a2388-203">Int32</span></span>|<span data-ttu-id="a2388-204">Microsoft 边缘网亭重置之前，请以分钟为单位的最后一个用户活动从指定的时间。</span><span class="sxs-lookup"><span data-stu-id="a2388-204">Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets.</span></span>  <span data-ttu-id="a2388-205">有效值为 0 1440年。</span><span class="sxs-lookup"><span data-stu-id="a2388-205">Valid values are 0-1440.</span></span> <span data-ttu-id="a2388-206">默认值为 5。</span><span class="sxs-lookup"><span data-stu-id="a2388-206">The default is 5.</span></span> <span data-ttu-id="a2388-207">0 指示不重置。</span><span class="sxs-lookup"><span data-stu-id="a2388-207">0 indicates no reset.</span></span> <span data-ttu-id="a2388-208">0 到 1440 之间的有效值</span><span class="sxs-lookup"><span data-stu-id="a2388-208">Valid values 0 to 1440</span></span>|



## <a name="response"></a><span data-ttu-id="a2388-209">响应</span><span class="sxs-lookup"><span data-stu-id="a2388-209">Response</span></span>
<span data-ttu-id="a2388-210">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a2388-210">If successful, this method returns a `200 OK` response code and an updated [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2388-211">示例</span><span class="sxs-lookup"><span data-stu-id="a2388-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2388-212">请求</span><span class="sxs-lookup"><span data-stu-id="a2388-212">Request</span></span>
<span data-ttu-id="a2388-213">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a2388-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="a2388-214">响应</span><span class="sxs-lookup"><span data-stu-id="a2388-214">Response</span></span>
<span data-ttu-id="a2388-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a2388-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




