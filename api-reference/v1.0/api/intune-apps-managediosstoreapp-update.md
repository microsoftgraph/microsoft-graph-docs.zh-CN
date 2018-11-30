---
title: 更新 managedIOSStoreApp
description: 更新 managedIOSStoreApp 对象的属性。
ms.openlocfilehash: feb77514d7b36e5915611168714d14e4c2705760
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008937"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="80da9-103">更新 managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="80da9-103">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="80da9-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="80da9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80da9-105">更新 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="80da9-105">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80da9-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="80da9-106">Prerequisites</span></span>
<span data-ttu-id="80da9-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="80da9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80da9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="80da9-109">Permission type</span></span>|<span data-ttu-id="80da9-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="80da9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80da9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80da9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="80da9-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80da9-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="80da9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80da9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80da9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="80da9-114">Not supported.</span></span>|
|<span data-ttu-id="80da9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="80da9-115">Application</span></span>|<span data-ttu-id="80da9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="80da9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80da9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80da9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="80da9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="80da9-118">Request headers</span></span>
|<span data-ttu-id="80da9-119">标头</span><span class="sxs-lookup"><span data-stu-id="80da9-119">Header</span></span>|<span data-ttu-id="80da9-120">值</span><span class="sxs-lookup"><span data-stu-id="80da9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80da9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="80da9-121">Authorization</span></span>|<span data-ttu-id="80da9-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="80da9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80da9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="80da9-123">Accept</span></span>|<span data-ttu-id="80da9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="80da9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80da9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="80da9-125">Request body</span></span>
<span data-ttu-id="80da9-126">在请求正文中，提供 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80da9-126">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="80da9-127">下表显示创建 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="80da9-127">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="80da9-128">属性</span><span class="sxs-lookup"><span data-stu-id="80da9-128">Property</span></span>|<span data-ttu-id="80da9-129">类型</span><span class="sxs-lookup"><span data-stu-id="80da9-129">Type</span></span>|<span data-ttu-id="80da9-130">说明</span><span class="sxs-lookup"><span data-stu-id="80da9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80da9-131">id</span><span class="sxs-lookup"><span data-stu-id="80da9-131">id</span></span>|<span data-ttu-id="80da9-132">String</span><span class="sxs-lookup"><span data-stu-id="80da9-132">String</span></span>|<span data-ttu-id="80da9-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="80da9-133">Key of the entity.</span></span> <span data-ttu-id="80da9-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80da9-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80da9-135">displayName</span><span class="sxs-lookup"><span data-stu-id="80da9-135">displayName</span></span>|<span data-ttu-id="80da9-136">String</span><span class="sxs-lookup"><span data-stu-id="80da9-136">String</span></span>|<span data-ttu-id="80da9-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="80da9-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="80da9-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80da9-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80da9-139">description</span><span class="sxs-lookup"><span data-stu-id="80da9-139">description</span></span>|<span data-ttu-id="80da9-140">String</span><span class="sxs-lookup"><span data-stu-id="80da9-140">String</span></span>|<span data-ttu-id="80da9-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="80da9-141">The description of the app.</span></span> <span data-ttu-id="80da9-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80da9-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80da9-143">publisher</span><span class="sxs-lookup"><span data-stu-id="80da9-143">publisher</span></span>|<span data-ttu-id="80da9-144">String</span><span class="sxs-lookup"><span data-stu-id="80da9-144">String</span></span>|<span data-ttu-id="80da9-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="80da9-145">The publisher of the app.</span></span> <span data-ttu-id="80da9-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80da9-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80da9-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="80da9-147">largeIcon</span></span>|[<span data-ttu-id="80da9-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="80da9-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="80da9-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="80da9-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="80da9-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80da9-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80da9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80da9-151">createdDateTime</span></span>|<span data-ttu-id="80da9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80da9-152">DateTimeOffset</span></span>|<span data-ttu-id="80da9-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="80da9-153">The date and time the app was created.</span></span> <span data-ttu-id="80da9-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80da9-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80da9-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80da9-155">lastModifiedDateTime</span></span>|<span data-ttu-id="80da9-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80da9-156">DateTimeOffset</span></span>|<span data-ttu-id="80da9-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="80da9-157">The date and time the app was last modified.</span></span> <span data-ttu-id="80da9-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80da9-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80da9-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="80da9-159">isFeatured</span></span>|<span data-ttu-id="80da9-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="80da9-160">Boolean</span></span>|<span data-ttu-id="80da9-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80da9-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80da9-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="80da9-162">privacyInformationUrl</span></span>|<span data-ttu-id="80da9-163">String</span><span class="sxs-lookup"><span data-stu-id="80da9-163">String</span></span>|<span data-ttu-id="80da9-164">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="80da9-164">The privacy statement Url.</span></span> <span data-ttu-id="80da9-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80da9-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80da9-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="80da9-166">informationUrl</span></span>|<span data-ttu-id="80da9-167">String</span><span class="sxs-lookup"><span data-stu-id="80da9-167">String</span></span>|<span data-ttu-id="80da9-168">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="80da9-168">The more information Url.</span></span> <span data-ttu-id="80da9-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80da9-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80da9-170">owner</span><span class="sxs-lookup"><span data-stu-id="80da9-170">owner</span></span>|<span data-ttu-id="80da9-171">String</span><span class="sxs-lookup"><span data-stu-id="80da9-171">String</span></span>|<span data-ttu-id="80da9-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="80da9-172">The owner of the app.</span></span> <span data-ttu-id="80da9-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80da9-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80da9-174">developer</span><span class="sxs-lookup"><span data-stu-id="80da9-174">developer</span></span>|<span data-ttu-id="80da9-175">String</span><span class="sxs-lookup"><span data-stu-id="80da9-175">String</span></span>|<span data-ttu-id="80da9-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="80da9-176">The developer of the app.</span></span> <span data-ttu-id="80da9-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80da9-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80da9-178">notes</span><span class="sxs-lookup"><span data-stu-id="80da9-178">notes</span></span>|<span data-ttu-id="80da9-179">String</span><span class="sxs-lookup"><span data-stu-id="80da9-179">String</span></span>|<span data-ttu-id="80da9-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="80da9-180">Notes for the app.</span></span> <span data-ttu-id="80da9-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80da9-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80da9-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="80da9-182">publishingState</span></span>|[<span data-ttu-id="80da9-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="80da9-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="80da9-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="80da9-184">The publishing state for the app.</span></span> <span data-ttu-id="80da9-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="80da9-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="80da9-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="80da9-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="80da9-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="80da9-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="80da9-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="80da9-188">appAvailability</span></span>|[<span data-ttu-id="80da9-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="80da9-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="80da9-190">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="80da9-190">The Application's availability.</span></span> <span data-ttu-id="80da9-191">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="80da9-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="80da9-192">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="80da9-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="80da9-193">version</span><span class="sxs-lookup"><span data-stu-id="80da9-193">version</span></span>|<span data-ttu-id="80da9-194">String</span><span class="sxs-lookup"><span data-stu-id="80da9-194">String</span></span>|<span data-ttu-id="80da9-195">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="80da9-195">The Application's version.</span></span> <span data-ttu-id="80da9-196">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="80da9-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="80da9-197">bundleId</span><span class="sxs-lookup"><span data-stu-id="80da9-197">bundleId</span></span>|<span data-ttu-id="80da9-198">String</span><span class="sxs-lookup"><span data-stu-id="80da9-198">String</span></span>|<span data-ttu-id="80da9-199">应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="80da9-199">The app's Bundle ID.</span></span>|
|<span data-ttu-id="80da9-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="80da9-200">appStoreUrl</span></span>|<span data-ttu-id="80da9-201">String</span><span class="sxs-lookup"><span data-stu-id="80da9-201">String</span></span>|<span data-ttu-id="80da9-202">Apple AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="80da9-202">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="80da9-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="80da9-203">applicableDeviceType</span></span>|[<span data-ttu-id="80da9-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="80da9-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="80da9-205">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="80da9-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="80da9-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="80da9-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="80da9-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="80da9-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="80da9-208">最低受支持操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="80da9-208">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="80da9-209">响应</span><span class="sxs-lookup"><span data-stu-id="80da9-209">Response</span></span>
<span data-ttu-id="80da9-210">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80da9-210">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80da9-211">示例</span><span class="sxs-lookup"><span data-stu-id="80da9-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="80da9-212">请求</span><span class="sxs-lookup"><span data-stu-id="80da9-212">Request</span></span>
<span data-ttu-id="80da9-213">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="80da9-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1084

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="80da9-214">响应</span><span class="sxs-lookup"><span data-stu-id="80da9-214">Response</span></span>
<span data-ttu-id="80da9-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80da9-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1256

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```



