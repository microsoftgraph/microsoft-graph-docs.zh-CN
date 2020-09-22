---
title: 更新 iosStoreApp
description: 更新 iosStoreApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ea6354c3d6e2996ab15903f1ad38ee9f1079478c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070126"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="7fdc2-103">更新 iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="7fdc2-103">Update iosStoreApp</span></span>

<span data-ttu-id="7fdc2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fdc2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7fdc2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fdc2-106">更新 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-106">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7fdc2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7fdc2-107">Prerequisites</span></span>
<span data-ttu-id="7fdc2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7fdc2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7fdc2-110">Permission type</span></span>|<span data-ttu-id="7fdc2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7fdc2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fdc2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7fdc2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7fdc2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fdc2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7fdc2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7fdc2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fdc2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-115">Not supported.</span></span>|
|<span data-ttu-id="7fdc2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7fdc2-116">Application</span></span>|<span data-ttu-id="7fdc2-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fdc2-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fdc2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7fdc2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="7fdc2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7fdc2-119">Request headers</span></span>
|<span data-ttu-id="7fdc2-120">标头</span><span class="sxs-lookup"><span data-stu-id="7fdc2-120">Header</span></span>|<span data-ttu-id="7fdc2-121">值</span><span class="sxs-lookup"><span data-stu-id="7fdc2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fdc2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fdc2-122">Authorization</span></span>|<span data-ttu-id="7fdc2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fdc2-124">接受</span><span class="sxs-lookup"><span data-stu-id="7fdc2-124">Accept</span></span>|<span data-ttu-id="7fdc2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7fdc2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fdc2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7fdc2-126">Request body</span></span>
<span data-ttu-id="7fdc2-127">在请求正文中，提供 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-127">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="7fdc2-128">下表显示了创建 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-128">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="7fdc2-129">属性</span><span class="sxs-lookup"><span data-stu-id="7fdc2-129">Property</span></span>|<span data-ttu-id="7fdc2-130">类型</span><span class="sxs-lookup"><span data-stu-id="7fdc2-130">Type</span></span>|<span data-ttu-id="7fdc2-131">说明</span><span class="sxs-lookup"><span data-stu-id="7fdc2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fdc2-132">id</span><span class="sxs-lookup"><span data-stu-id="7fdc2-132">id</span></span>|<span data-ttu-id="7fdc2-133">String</span><span class="sxs-lookup"><span data-stu-id="7fdc2-133">String</span></span>|<span data-ttu-id="7fdc2-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-134">Key of the entity.</span></span> <span data-ttu-id="7fdc2-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7fdc2-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7fdc2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7fdc2-136">displayName</span></span>|<span data-ttu-id="7fdc2-137">String</span><span class="sxs-lookup"><span data-stu-id="7fdc2-137">String</span></span>|<span data-ttu-id="7fdc2-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7fdc2-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7fdc2-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7fdc2-140">description</span><span class="sxs-lookup"><span data-stu-id="7fdc2-140">description</span></span>|<span data-ttu-id="7fdc2-141">String</span><span class="sxs-lookup"><span data-stu-id="7fdc2-141">String</span></span>|<span data-ttu-id="7fdc2-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-142">The description of the app.</span></span> <span data-ttu-id="7fdc2-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7fdc2-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7fdc2-144">publisher</span><span class="sxs-lookup"><span data-stu-id="7fdc2-144">publisher</span></span>|<span data-ttu-id="7fdc2-145">String</span><span class="sxs-lookup"><span data-stu-id="7fdc2-145">String</span></span>|<span data-ttu-id="7fdc2-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-146">The publisher of the app.</span></span> <span data-ttu-id="7fdc2-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7fdc2-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7fdc2-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7fdc2-148">largeIcon</span></span>|[<span data-ttu-id="7fdc2-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7fdc2-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7fdc2-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7fdc2-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7fdc2-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7fdc2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7fdc2-152">createdDateTime</span></span>|<span data-ttu-id="7fdc2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fdc2-153">DateTimeOffset</span></span>|<span data-ttu-id="7fdc2-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-154">The date and time the app was created.</span></span> <span data-ttu-id="7fdc2-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7fdc2-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7fdc2-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7fdc2-156">lastModifiedDateTime</span></span>|<span data-ttu-id="7fdc2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fdc2-157">DateTimeOffset</span></span>|<span data-ttu-id="7fdc2-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-158">The date and time the app was last modified.</span></span> <span data-ttu-id="7fdc2-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7fdc2-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7fdc2-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7fdc2-160">isFeatured</span></span>|<span data-ttu-id="7fdc2-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fdc2-161">Boolean</span></span>|<span data-ttu-id="7fdc2-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7fdc2-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7fdc2-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7fdc2-163">privacyInformationUrl</span></span>|<span data-ttu-id="7fdc2-164">String</span><span class="sxs-lookup"><span data-stu-id="7fdc2-164">String</span></span>|<span data-ttu-id="7fdc2-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-165">The privacy statement Url.</span></span> <span data-ttu-id="7fdc2-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7fdc2-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7fdc2-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7fdc2-167">informationUrl</span></span>|<span data-ttu-id="7fdc2-168">String</span><span class="sxs-lookup"><span data-stu-id="7fdc2-168">String</span></span>|<span data-ttu-id="7fdc2-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-169">The more information Url.</span></span> <span data-ttu-id="7fdc2-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7fdc2-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7fdc2-171">owner</span><span class="sxs-lookup"><span data-stu-id="7fdc2-171">owner</span></span>|<span data-ttu-id="7fdc2-172">String</span><span class="sxs-lookup"><span data-stu-id="7fdc2-172">String</span></span>|<span data-ttu-id="7fdc2-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-173">The owner of the app.</span></span> <span data-ttu-id="7fdc2-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7fdc2-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7fdc2-175">developer</span><span class="sxs-lookup"><span data-stu-id="7fdc2-175">developer</span></span>|<span data-ttu-id="7fdc2-176">String</span><span class="sxs-lookup"><span data-stu-id="7fdc2-176">String</span></span>|<span data-ttu-id="7fdc2-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-177">The developer of the app.</span></span> <span data-ttu-id="7fdc2-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7fdc2-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7fdc2-179">notes</span><span class="sxs-lookup"><span data-stu-id="7fdc2-179">notes</span></span>|<span data-ttu-id="7fdc2-180">String</span><span class="sxs-lookup"><span data-stu-id="7fdc2-180">String</span></span>|<span data-ttu-id="7fdc2-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-181">Notes for the app.</span></span> <span data-ttu-id="7fdc2-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7fdc2-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7fdc2-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="7fdc2-183">publishingState</span></span>|[<span data-ttu-id="7fdc2-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7fdc2-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7fdc2-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-185">The publishing state for the app.</span></span> <span data-ttu-id="7fdc2-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7fdc2-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7fdc2-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7fdc2-189">bundleId</span><span class="sxs-lookup"><span data-stu-id="7fdc2-189">bundleId</span></span>|<span data-ttu-id="7fdc2-190">String</span><span class="sxs-lookup"><span data-stu-id="7fdc2-190">String</span></span>|<span data-ttu-id="7fdc2-191">标识名称。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-191">The Identity Name.</span></span>|
|<span data-ttu-id="7fdc2-192">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7fdc2-192">appStoreUrl</span></span>|<span data-ttu-id="7fdc2-193">String</span><span class="sxs-lookup"><span data-stu-id="7fdc2-193">String</span></span>|<span data-ttu-id="7fdc2-194">Apple App Store URL</span><span class="sxs-lookup"><span data-stu-id="7fdc2-194">The Apple App Store URL</span></span>|
|<span data-ttu-id="7fdc2-195">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="7fdc2-195">applicableDeviceType</span></span>|[<span data-ttu-id="7fdc2-196">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="7fdc2-196">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="7fdc2-197">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-197">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="7fdc2-198">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7fdc2-198">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7fdc2-199">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7fdc2-199">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="7fdc2-200">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-200">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="7fdc2-201">响应</span><span class="sxs-lookup"><span data-stu-id="7fdc2-201">Response</span></span>
<span data-ttu-id="7fdc2-202">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-202">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fdc2-203">示例</span><span class="sxs-lookup"><span data-stu-id="7fdc2-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fdc2-204">请求</span><span class="sxs-lookup"><span data-stu-id="7fdc2-204">Request</span></span>
<span data-ttu-id="7fdc2-205">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="7fdc2-206">响应</span><span class="sxs-lookup"><span data-stu-id="7fdc2-206">Response</span></span>
<span data-ttu-id="7fdc2-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7fdc2-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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









