---
title: 创建 iosStoreApp
description: 创建新的 iosStoreApp 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dca2d1092620c10e2f5d8484d3ccdc43903ffd15
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002522"
---
# <a name="create-iosstoreapp"></a><span data-ttu-id="60739-103">创建 iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="60739-103">Create iosStoreApp</span></span>

> <span data-ttu-id="60739-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="60739-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60739-105">创建新的 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60739-105">Create a new [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60739-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="60739-106">Prerequisites</span></span>
<span data-ttu-id="60739-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60739-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60739-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="60739-109">Permission type</span></span>|<span data-ttu-id="60739-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="60739-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60739-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60739-111">Delegated (work or school account)</span></span>|<span data-ttu-id="60739-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60739-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="60739-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60739-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60739-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="60739-114">Not supported.</span></span>|
|<span data-ttu-id="60739-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="60739-115">Application</span></span>|<span data-ttu-id="60739-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="60739-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60739-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60739-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="60739-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="60739-118">Request headers</span></span>
|<span data-ttu-id="60739-119">标头</span><span class="sxs-lookup"><span data-stu-id="60739-119">Header</span></span>|<span data-ttu-id="60739-120">值</span><span class="sxs-lookup"><span data-stu-id="60739-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60739-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="60739-121">Authorization</span></span>|<span data-ttu-id="60739-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="60739-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60739-123">接受</span><span class="sxs-lookup"><span data-stu-id="60739-123">Accept</span></span>|<span data-ttu-id="60739-124">application/json</span><span class="sxs-lookup"><span data-stu-id="60739-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60739-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="60739-125">Request body</span></span>
<span data-ttu-id="60739-126">在请求正文中，提供 iosStoreApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60739-126">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="60739-127">下表显示了创建 iosStoreApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="60739-127">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="60739-128">属性</span><span class="sxs-lookup"><span data-stu-id="60739-128">Property</span></span>|<span data-ttu-id="60739-129">类型</span><span class="sxs-lookup"><span data-stu-id="60739-129">Type</span></span>|<span data-ttu-id="60739-130">说明</span><span class="sxs-lookup"><span data-stu-id="60739-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60739-131">id</span><span class="sxs-lookup"><span data-stu-id="60739-131">id</span></span>|<span data-ttu-id="60739-132">字符串</span><span class="sxs-lookup"><span data-stu-id="60739-132">String</span></span>|<span data-ttu-id="60739-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="60739-133">Key of the entity.</span></span> <span data-ttu-id="60739-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="60739-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="60739-135">displayName</span><span class="sxs-lookup"><span data-stu-id="60739-135">displayName</span></span>|<span data-ttu-id="60739-136">String</span><span class="sxs-lookup"><span data-stu-id="60739-136">String</span></span>|<span data-ttu-id="60739-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="60739-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="60739-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="60739-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="60739-139">说明</span><span class="sxs-lookup"><span data-stu-id="60739-139">description</span></span>|<span data-ttu-id="60739-140">字符串</span><span class="sxs-lookup"><span data-stu-id="60739-140">String</span></span>|<span data-ttu-id="60739-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="60739-141">The description of the app.</span></span> <span data-ttu-id="60739-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="60739-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="60739-143">publisher</span><span class="sxs-lookup"><span data-stu-id="60739-143">publisher</span></span>|<span data-ttu-id="60739-144">String</span><span class="sxs-lookup"><span data-stu-id="60739-144">String</span></span>|<span data-ttu-id="60739-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="60739-145">The publisher of the app.</span></span> <span data-ttu-id="60739-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="60739-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="60739-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="60739-147">largeIcon</span></span>|[<span data-ttu-id="60739-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="60739-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="60739-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="60739-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="60739-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="60739-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="60739-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="60739-151">createdDateTime</span></span>|<span data-ttu-id="60739-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60739-152">DateTimeOffset</span></span>|<span data-ttu-id="60739-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="60739-153">The date and time the app was created.</span></span> <span data-ttu-id="60739-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="60739-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="60739-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="60739-155">lastModifiedDateTime</span></span>|<span data-ttu-id="60739-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60739-156">DateTimeOffset</span></span>|<span data-ttu-id="60739-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="60739-157">The date and time the app was last modified.</span></span> <span data-ttu-id="60739-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="60739-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="60739-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="60739-159">isFeatured</span></span>|<span data-ttu-id="60739-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="60739-160">Boolean</span></span>|<span data-ttu-id="60739-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="60739-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="60739-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="60739-162">privacyInformationUrl</span></span>|<span data-ttu-id="60739-163">String</span><span class="sxs-lookup"><span data-stu-id="60739-163">String</span></span>|<span data-ttu-id="60739-164">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="60739-164">The privacy statement Url.</span></span> <span data-ttu-id="60739-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="60739-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="60739-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="60739-166">informationUrl</span></span>|<span data-ttu-id="60739-167">String</span><span class="sxs-lookup"><span data-stu-id="60739-167">String</span></span>|<span data-ttu-id="60739-168">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="60739-168">The more information Url.</span></span> <span data-ttu-id="60739-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="60739-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="60739-170">owner</span><span class="sxs-lookup"><span data-stu-id="60739-170">owner</span></span>|<span data-ttu-id="60739-171">String</span><span class="sxs-lookup"><span data-stu-id="60739-171">String</span></span>|<span data-ttu-id="60739-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="60739-172">The owner of the app.</span></span> <span data-ttu-id="60739-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="60739-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="60739-174">developer</span><span class="sxs-lookup"><span data-stu-id="60739-174">developer</span></span>|<span data-ttu-id="60739-175">String</span><span class="sxs-lookup"><span data-stu-id="60739-175">String</span></span>|<span data-ttu-id="60739-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="60739-176">The developer of the app.</span></span> <span data-ttu-id="60739-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="60739-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="60739-178">notes</span><span class="sxs-lookup"><span data-stu-id="60739-178">notes</span></span>|<span data-ttu-id="60739-179">String</span><span class="sxs-lookup"><span data-stu-id="60739-179">String</span></span>|<span data-ttu-id="60739-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="60739-180">Notes for the app.</span></span> <span data-ttu-id="60739-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="60739-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="60739-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="60739-182">publishingState</span></span>|[<span data-ttu-id="60739-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="60739-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="60739-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="60739-184">The publishing state for the app.</span></span> <span data-ttu-id="60739-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="60739-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="60739-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="60739-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="60739-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="60739-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="60739-188">bundleId</span><span class="sxs-lookup"><span data-stu-id="60739-188">bundleId</span></span>|<span data-ttu-id="60739-189">String</span><span class="sxs-lookup"><span data-stu-id="60739-189">String</span></span>|<span data-ttu-id="60739-190">标识名称。</span><span class="sxs-lookup"><span data-stu-id="60739-190">The Identity Name.</span></span>|
|<span data-ttu-id="60739-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="60739-191">appStoreUrl</span></span>|<span data-ttu-id="60739-192">String</span><span class="sxs-lookup"><span data-stu-id="60739-192">String</span></span>|<span data-ttu-id="60739-193">Apple App Store URL</span><span class="sxs-lookup"><span data-stu-id="60739-193">The Apple App Store URL</span></span>|
|<span data-ttu-id="60739-194">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="60739-194">applicableDeviceType</span></span>|[<span data-ttu-id="60739-195">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="60739-195">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="60739-196">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="60739-196">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="60739-197">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="60739-197">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="60739-198">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="60739-198">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="60739-199">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="60739-199">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="60739-200">响应</span><span class="sxs-lookup"><span data-stu-id="60739-200">Response</span></span>
<span data-ttu-id="60739-201">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60739-201">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60739-202">示例</span><span class="sxs-lookup"><span data-stu-id="60739-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="60739-203">请求</span><span class="sxs-lookup"><span data-stu-id="60739-203">Request</span></span>
<span data-ttu-id="60739-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="60739-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1006

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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

### <a name="response"></a><span data-ttu-id="60739-205">响应</span><span class="sxs-lookup"><span data-stu-id="60739-205">Response</span></span>
<span data-ttu-id="60739-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="60739-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1178

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



