---
title: 创建 iosStoreApp
description: 创建新的 iosStoreApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d665c23c53a0c646ad00b691f14f8a612b142181
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985578"
---
# <a name="create-iosstoreapp"></a><span data-ttu-id="40b68-103">创建 iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="40b68-103">Create iosStoreApp</span></span>

<span data-ttu-id="40b68-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40b68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40b68-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="40b68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40b68-106">创建新的 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="40b68-106">Create a new [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40b68-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="40b68-107">Prerequisites</span></span>
<span data-ttu-id="40b68-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="40b68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="40b68-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="40b68-110">Permission type</span></span>|<span data-ttu-id="40b68-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="40b68-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40b68-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40b68-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40b68-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40b68-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="40b68-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40b68-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40b68-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="40b68-115">Not supported.</span></span>|
|<span data-ttu-id="40b68-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="40b68-116">Application</span></span>|<span data-ttu-id="40b68-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40b68-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40b68-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40b68-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="40b68-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="40b68-119">Request headers</span></span>
|<span data-ttu-id="40b68-120">标头</span><span class="sxs-lookup"><span data-stu-id="40b68-120">Header</span></span>|<span data-ttu-id="40b68-121">值</span><span class="sxs-lookup"><span data-stu-id="40b68-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40b68-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="40b68-122">Authorization</span></span>|<span data-ttu-id="40b68-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="40b68-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40b68-124">接受</span><span class="sxs-lookup"><span data-stu-id="40b68-124">Accept</span></span>|<span data-ttu-id="40b68-125">application/json</span><span class="sxs-lookup"><span data-stu-id="40b68-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40b68-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="40b68-126">Request body</span></span>
<span data-ttu-id="40b68-127">在请求正文中，提供 iosStoreApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40b68-127">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="40b68-128">下表显示了创建 iosStoreApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="40b68-128">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="40b68-129">属性</span><span class="sxs-lookup"><span data-stu-id="40b68-129">Property</span></span>|<span data-ttu-id="40b68-130">类型</span><span class="sxs-lookup"><span data-stu-id="40b68-130">Type</span></span>|<span data-ttu-id="40b68-131">说明</span><span class="sxs-lookup"><span data-stu-id="40b68-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40b68-132">id</span><span class="sxs-lookup"><span data-stu-id="40b68-132">id</span></span>|<span data-ttu-id="40b68-133">String</span><span class="sxs-lookup"><span data-stu-id="40b68-133">String</span></span>|<span data-ttu-id="40b68-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="40b68-134">Key of the entity.</span></span> <span data-ttu-id="40b68-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40b68-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40b68-136">displayName</span><span class="sxs-lookup"><span data-stu-id="40b68-136">displayName</span></span>|<span data-ttu-id="40b68-137">String</span><span class="sxs-lookup"><span data-stu-id="40b68-137">String</span></span>|<span data-ttu-id="40b68-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="40b68-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="40b68-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40b68-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40b68-140">description</span><span class="sxs-lookup"><span data-stu-id="40b68-140">description</span></span>|<span data-ttu-id="40b68-141">String</span><span class="sxs-lookup"><span data-stu-id="40b68-141">String</span></span>|<span data-ttu-id="40b68-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="40b68-142">The description of the app.</span></span> <span data-ttu-id="40b68-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40b68-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40b68-144">publisher</span><span class="sxs-lookup"><span data-stu-id="40b68-144">publisher</span></span>|<span data-ttu-id="40b68-145">String</span><span class="sxs-lookup"><span data-stu-id="40b68-145">String</span></span>|<span data-ttu-id="40b68-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="40b68-146">The publisher of the app.</span></span> <span data-ttu-id="40b68-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40b68-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40b68-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="40b68-148">largeIcon</span></span>|[<span data-ttu-id="40b68-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="40b68-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="40b68-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="40b68-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="40b68-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40b68-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40b68-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40b68-152">createdDateTime</span></span>|<span data-ttu-id="40b68-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40b68-153">DateTimeOffset</span></span>|<span data-ttu-id="40b68-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="40b68-154">The date and time the app was created.</span></span> <span data-ttu-id="40b68-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40b68-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40b68-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40b68-156">lastModifiedDateTime</span></span>|<span data-ttu-id="40b68-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40b68-157">DateTimeOffset</span></span>|<span data-ttu-id="40b68-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="40b68-158">The date and time the app was last modified.</span></span> <span data-ttu-id="40b68-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40b68-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40b68-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="40b68-160">isFeatured</span></span>|<span data-ttu-id="40b68-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="40b68-161">Boolean</span></span>|<span data-ttu-id="40b68-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40b68-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40b68-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="40b68-163">privacyInformationUrl</span></span>|<span data-ttu-id="40b68-164">String</span><span class="sxs-lookup"><span data-stu-id="40b68-164">String</span></span>|<span data-ttu-id="40b68-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="40b68-165">The privacy statement Url.</span></span> <span data-ttu-id="40b68-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40b68-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40b68-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="40b68-167">informationUrl</span></span>|<span data-ttu-id="40b68-168">String</span><span class="sxs-lookup"><span data-stu-id="40b68-168">String</span></span>|<span data-ttu-id="40b68-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="40b68-169">The more information Url.</span></span> <span data-ttu-id="40b68-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40b68-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40b68-171">所有者</span><span class="sxs-lookup"><span data-stu-id="40b68-171">owner</span></span>|<span data-ttu-id="40b68-172">String</span><span class="sxs-lookup"><span data-stu-id="40b68-172">String</span></span>|<span data-ttu-id="40b68-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="40b68-173">The owner of the app.</span></span> <span data-ttu-id="40b68-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40b68-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40b68-175">developer</span><span class="sxs-lookup"><span data-stu-id="40b68-175">developer</span></span>|<span data-ttu-id="40b68-176">String</span><span class="sxs-lookup"><span data-stu-id="40b68-176">String</span></span>|<span data-ttu-id="40b68-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="40b68-177">The developer of the app.</span></span> <span data-ttu-id="40b68-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40b68-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40b68-179">notes</span><span class="sxs-lookup"><span data-stu-id="40b68-179">notes</span></span>|<span data-ttu-id="40b68-180">String</span><span class="sxs-lookup"><span data-stu-id="40b68-180">String</span></span>|<span data-ttu-id="40b68-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="40b68-181">Notes for the app.</span></span> <span data-ttu-id="40b68-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40b68-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40b68-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="40b68-183">publishingState</span></span>|[<span data-ttu-id="40b68-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="40b68-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="40b68-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="40b68-185">The publishing state for the app.</span></span> <span data-ttu-id="40b68-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="40b68-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="40b68-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="40b68-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="40b68-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="40b68-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="40b68-189">bundleId</span><span class="sxs-lookup"><span data-stu-id="40b68-189">bundleId</span></span>|<span data-ttu-id="40b68-190">String</span><span class="sxs-lookup"><span data-stu-id="40b68-190">String</span></span>|<span data-ttu-id="40b68-191">标识名称。</span><span class="sxs-lookup"><span data-stu-id="40b68-191">The Identity Name.</span></span>|
|<span data-ttu-id="40b68-192">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="40b68-192">appStoreUrl</span></span>|<span data-ttu-id="40b68-193">String</span><span class="sxs-lookup"><span data-stu-id="40b68-193">String</span></span>|<span data-ttu-id="40b68-194">Apple App Store URL</span><span class="sxs-lookup"><span data-stu-id="40b68-194">The Apple App Store URL</span></span>|
|<span data-ttu-id="40b68-195">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="40b68-195">applicableDeviceType</span></span>|[<span data-ttu-id="40b68-196">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="40b68-196">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="40b68-197">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="40b68-197">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="40b68-198">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="40b68-198">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="40b68-199">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="40b68-199">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="40b68-200">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="40b68-200">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="40b68-201">响应</span><span class="sxs-lookup"><span data-stu-id="40b68-201">Response</span></span>
<span data-ttu-id="40b68-202">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="40b68-202">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40b68-203">示例</span><span class="sxs-lookup"><span data-stu-id="40b68-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="40b68-204">请求</span><span class="sxs-lookup"><span data-stu-id="40b68-204">Request</span></span>
<span data-ttu-id="40b68-205">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="40b68-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1026

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
    "v12_0": true,
    "v13_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="40b68-206">响应</span><span class="sxs-lookup"><span data-stu-id="40b68-206">Response</span></span>
<span data-ttu-id="40b68-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="40b68-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1198

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
    "v12_0": true,
    "v13_0": true
  }
}
```









