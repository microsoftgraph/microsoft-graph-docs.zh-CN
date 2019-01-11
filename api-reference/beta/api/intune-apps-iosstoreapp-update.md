---
title: 更新 iosStoreApp
description: 更新 iosStoreApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3791f7eef7abdc1298289e66f25c156e1bc8848d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870201"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="69711-103">更新 iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="69711-103">Update iosStoreApp</span></span>

> <span data-ttu-id="69711-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="69711-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69711-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="69711-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69711-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="69711-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69711-107">更新 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="69711-107">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69711-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="69711-108">Prerequisites</span></span>
<span data-ttu-id="69711-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="69711-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69711-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="69711-111">Permission type</span></span>|<span data-ttu-id="69711-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="69711-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69711-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69711-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69711-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69711-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="69711-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69711-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69711-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="69711-116">Not supported.</span></span>|
|<span data-ttu-id="69711-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="69711-117">Application</span></span>|<span data-ttu-id="69711-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="69711-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69711-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69711-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="69711-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="69711-120">Request headers</span></span>
|<span data-ttu-id="69711-121">标头</span><span class="sxs-lookup"><span data-stu-id="69711-121">Header</span></span>|<span data-ttu-id="69711-122">值</span><span class="sxs-lookup"><span data-stu-id="69711-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69711-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="69711-123">Authorization</span></span>|<span data-ttu-id="69711-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="69711-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69711-125">Accept</span><span class="sxs-lookup"><span data-stu-id="69711-125">Accept</span></span>|<span data-ttu-id="69711-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69711-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69711-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="69711-127">Request body</span></span>
<span data-ttu-id="69711-128">在请求正文中，提供 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69711-128">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="69711-129">下表显示了创建 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="69711-129">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="69711-130">属性</span><span class="sxs-lookup"><span data-stu-id="69711-130">Property</span></span>|<span data-ttu-id="69711-131">类型</span><span class="sxs-lookup"><span data-stu-id="69711-131">Type</span></span>|<span data-ttu-id="69711-132">说明</span><span class="sxs-lookup"><span data-stu-id="69711-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69711-133">id</span><span class="sxs-lookup"><span data-stu-id="69711-133">id</span></span>|<span data-ttu-id="69711-134">String</span><span class="sxs-lookup"><span data-stu-id="69711-134">String</span></span>|<span data-ttu-id="69711-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="69711-135">Key of the entity.</span></span> <span data-ttu-id="69711-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69711-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69711-137">displayName</span><span class="sxs-lookup"><span data-stu-id="69711-137">displayName</span></span>|<span data-ttu-id="69711-138">String</span><span class="sxs-lookup"><span data-stu-id="69711-138">String</span></span>|<span data-ttu-id="69711-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="69711-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="69711-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69711-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69711-141">description</span><span class="sxs-lookup"><span data-stu-id="69711-141">description</span></span>|<span data-ttu-id="69711-142">String</span><span class="sxs-lookup"><span data-stu-id="69711-142">String</span></span>|<span data-ttu-id="69711-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="69711-143">The description of the app.</span></span> <span data-ttu-id="69711-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69711-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69711-145">publisher</span><span class="sxs-lookup"><span data-stu-id="69711-145">publisher</span></span>|<span data-ttu-id="69711-146">String</span><span class="sxs-lookup"><span data-stu-id="69711-146">String</span></span>|<span data-ttu-id="69711-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="69711-147">The publisher of the app.</span></span> <span data-ttu-id="69711-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69711-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69711-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="69711-149">largeIcon</span></span>|[<span data-ttu-id="69711-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="69711-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="69711-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="69711-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="69711-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69711-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69711-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69711-153">createdDateTime</span></span>|<span data-ttu-id="69711-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69711-154">DateTimeOffset</span></span>|<span data-ttu-id="69711-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="69711-155">The date and time the app was created.</span></span> <span data-ttu-id="69711-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69711-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69711-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69711-157">lastModifiedDateTime</span></span>|<span data-ttu-id="69711-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69711-158">DateTimeOffset</span></span>|<span data-ttu-id="69711-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="69711-159">The date and time the app was last modified.</span></span> <span data-ttu-id="69711-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69711-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69711-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="69711-161">isFeatured</span></span>|<span data-ttu-id="69711-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="69711-162">Boolean</span></span>|<span data-ttu-id="69711-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69711-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69711-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="69711-164">privacyInformationUrl</span></span>|<span data-ttu-id="69711-165">String</span><span class="sxs-lookup"><span data-stu-id="69711-165">String</span></span>|<span data-ttu-id="69711-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="69711-166">The privacy statement Url.</span></span> <span data-ttu-id="69711-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69711-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69711-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="69711-168">informationUrl</span></span>|<span data-ttu-id="69711-169">String</span><span class="sxs-lookup"><span data-stu-id="69711-169">String</span></span>|<span data-ttu-id="69711-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="69711-170">The more information Url.</span></span> <span data-ttu-id="69711-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69711-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69711-172">owner</span><span class="sxs-lookup"><span data-stu-id="69711-172">owner</span></span>|<span data-ttu-id="69711-173">String</span><span class="sxs-lookup"><span data-stu-id="69711-173">String</span></span>|<span data-ttu-id="69711-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="69711-174">The owner of the app.</span></span> <span data-ttu-id="69711-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69711-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69711-176">developer</span><span class="sxs-lookup"><span data-stu-id="69711-176">developer</span></span>|<span data-ttu-id="69711-177">String</span><span class="sxs-lookup"><span data-stu-id="69711-177">String</span></span>|<span data-ttu-id="69711-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="69711-178">The developer of the app.</span></span> <span data-ttu-id="69711-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69711-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69711-180">notes</span><span class="sxs-lookup"><span data-stu-id="69711-180">notes</span></span>|<span data-ttu-id="69711-181">String</span><span class="sxs-lookup"><span data-stu-id="69711-181">String</span></span>|<span data-ttu-id="69711-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="69711-182">Notes for the app.</span></span> <span data-ttu-id="69711-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69711-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69711-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="69711-184">uploadState</span></span>|<span data-ttu-id="69711-185">Int32</span><span class="sxs-lookup"><span data-stu-id="69711-185">Int32</span></span>|<span data-ttu-id="69711-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="69711-186">The upload state.</span></span> <span data-ttu-id="69711-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69711-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69711-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="69711-188">publishingState</span></span>|[<span data-ttu-id="69711-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="69711-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="69711-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="69711-190">The publishing state for the app.</span></span> <span data-ttu-id="69711-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="69711-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="69711-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="69711-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="69711-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="69711-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="69711-194">bundleId</span><span class="sxs-lookup"><span data-stu-id="69711-194">bundleId</span></span>|<span data-ttu-id="69711-195">String</span><span class="sxs-lookup"><span data-stu-id="69711-195">String</span></span>|<span data-ttu-id="69711-196">标识名称。</span><span class="sxs-lookup"><span data-stu-id="69711-196">The Identity Name.</span></span>|
|<span data-ttu-id="69711-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="69711-197">appStoreUrl</span></span>|<span data-ttu-id="69711-198">String</span><span class="sxs-lookup"><span data-stu-id="69711-198">String</span></span>|<span data-ttu-id="69711-199">Apple App Store URL</span><span class="sxs-lookup"><span data-stu-id="69711-199">The Apple App Store URL</span></span>|
|<span data-ttu-id="69711-200">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="69711-200">applicableDeviceType</span></span>|[<span data-ttu-id="69711-201">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="69711-201">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="69711-202">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="69711-202">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="69711-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="69711-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="69711-204">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="69711-204">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="69711-205">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="69711-205">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="69711-206">响应</span><span class="sxs-lookup"><span data-stu-id="69711-206">Response</span></span>
<span data-ttu-id="69711-207">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="69711-207">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69711-208">示例</span><span class="sxs-lookup"><span data-stu-id="69711-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="69711-209">请求</span><span class="sxs-lookup"><span data-stu-id="69711-209">Request</span></span>
<span data-ttu-id="69711-210">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69711-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1042

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
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

### <a name="response"></a><span data-ttu-id="69711-211">响应</span><span class="sxs-lookup"><span data-stu-id="69711-211">Response</span></span>
<span data-ttu-id="69711-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69711-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1200

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
  "uploadState": 11,
  "publishingState": "processing",
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





