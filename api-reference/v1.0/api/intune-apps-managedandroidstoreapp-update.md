---
title: 更新 managedAndroidStoreApp
description: 更新 managedAndroidStoreApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f0d76b4960a336e5bddb1c60887b18b64328dbd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754278"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="77737-103">更新 managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="77737-103">Update managedAndroidStoreApp</span></span>

<span data-ttu-id="77737-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77737-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77737-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77737-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77737-106">更新 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="77737-106">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77737-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="77737-107">Prerequisites</span></span>
<span data-ttu-id="77737-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77737-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77737-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="77737-110">Permission type</span></span>|<span data-ttu-id="77737-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77737-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77737-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77737-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77737-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77737-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="77737-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77737-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77737-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="77737-115">Not supported.</span></span>|
|<span data-ttu-id="77737-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="77737-116">Application</span></span>|<span data-ttu-id="77737-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77737-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77737-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77737-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="77737-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="77737-119">Request headers</span></span>
|<span data-ttu-id="77737-120">标头</span><span class="sxs-lookup"><span data-stu-id="77737-120">Header</span></span>|<span data-ttu-id="77737-121">值</span><span class="sxs-lookup"><span data-stu-id="77737-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77737-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="77737-122">Authorization</span></span>|<span data-ttu-id="77737-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="77737-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77737-124">接受</span><span class="sxs-lookup"><span data-stu-id="77737-124">Accept</span></span>|<span data-ttu-id="77737-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77737-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77737-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="77737-126">Request body</span></span>
<span data-ttu-id="77737-127">在请求正文中，提供 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77737-127">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="77737-128">下表显示了创建 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="77737-128">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="77737-129">属性</span><span class="sxs-lookup"><span data-stu-id="77737-129">Property</span></span>|<span data-ttu-id="77737-130">类型</span><span class="sxs-lookup"><span data-stu-id="77737-130">Type</span></span>|<span data-ttu-id="77737-131">说明</span><span class="sxs-lookup"><span data-stu-id="77737-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77737-132">id</span><span class="sxs-lookup"><span data-stu-id="77737-132">id</span></span>|<span data-ttu-id="77737-133">String</span><span class="sxs-lookup"><span data-stu-id="77737-133">String</span></span>|<span data-ttu-id="77737-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="77737-134">Key of the entity.</span></span> <span data-ttu-id="77737-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="77737-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77737-136">displayName</span><span class="sxs-lookup"><span data-stu-id="77737-136">displayName</span></span>|<span data-ttu-id="77737-137">String</span><span class="sxs-lookup"><span data-stu-id="77737-137">String</span></span>|<span data-ttu-id="77737-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="77737-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="77737-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="77737-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77737-140">说明</span><span class="sxs-lookup"><span data-stu-id="77737-140">description</span></span>|<span data-ttu-id="77737-141">String</span><span class="sxs-lookup"><span data-stu-id="77737-141">String</span></span>|<span data-ttu-id="77737-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="77737-142">The description of the app.</span></span> <span data-ttu-id="77737-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="77737-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77737-144">publisher</span><span class="sxs-lookup"><span data-stu-id="77737-144">publisher</span></span>|<span data-ttu-id="77737-145">String</span><span class="sxs-lookup"><span data-stu-id="77737-145">String</span></span>|<span data-ttu-id="77737-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="77737-146">The publisher of the app.</span></span> <span data-ttu-id="77737-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="77737-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77737-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="77737-148">largeIcon</span></span>|[<span data-ttu-id="77737-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="77737-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="77737-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="77737-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="77737-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="77737-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77737-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77737-152">createdDateTime</span></span>|<span data-ttu-id="77737-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77737-153">DateTimeOffset</span></span>|<span data-ttu-id="77737-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="77737-154">The date and time the app was created.</span></span> <span data-ttu-id="77737-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="77737-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77737-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77737-156">lastModifiedDateTime</span></span>|<span data-ttu-id="77737-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77737-157">DateTimeOffset</span></span>|<span data-ttu-id="77737-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="77737-158">The date and time the app was last modified.</span></span> <span data-ttu-id="77737-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="77737-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77737-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="77737-160">isFeatured</span></span>|<span data-ttu-id="77737-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="77737-161">Boolean</span></span>|<span data-ttu-id="77737-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="77737-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77737-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="77737-163">privacyInformationUrl</span></span>|<span data-ttu-id="77737-164">String</span><span class="sxs-lookup"><span data-stu-id="77737-164">String</span></span>|<span data-ttu-id="77737-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="77737-165">The privacy statement Url.</span></span> <span data-ttu-id="77737-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="77737-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77737-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="77737-167">informationUrl</span></span>|<span data-ttu-id="77737-168">String</span><span class="sxs-lookup"><span data-stu-id="77737-168">String</span></span>|<span data-ttu-id="77737-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="77737-169">The more information Url.</span></span> <span data-ttu-id="77737-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="77737-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77737-171">所有者</span><span class="sxs-lookup"><span data-stu-id="77737-171">owner</span></span>|<span data-ttu-id="77737-172">String</span><span class="sxs-lookup"><span data-stu-id="77737-172">String</span></span>|<span data-ttu-id="77737-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="77737-173">The owner of the app.</span></span> <span data-ttu-id="77737-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="77737-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77737-175">developer</span><span class="sxs-lookup"><span data-stu-id="77737-175">developer</span></span>|<span data-ttu-id="77737-176">String</span><span class="sxs-lookup"><span data-stu-id="77737-176">String</span></span>|<span data-ttu-id="77737-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="77737-177">The developer of the app.</span></span> <span data-ttu-id="77737-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="77737-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77737-179">notes</span><span class="sxs-lookup"><span data-stu-id="77737-179">notes</span></span>|<span data-ttu-id="77737-180">String</span><span class="sxs-lookup"><span data-stu-id="77737-180">String</span></span>|<span data-ttu-id="77737-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="77737-181">Notes for the app.</span></span> <span data-ttu-id="77737-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="77737-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77737-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="77737-183">publishingState</span></span>|[<span data-ttu-id="77737-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="77737-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="77737-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="77737-185">The publishing state for the app.</span></span> <span data-ttu-id="77737-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="77737-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="77737-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="77737-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="77737-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="77737-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="77737-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="77737-189">appAvailability</span></span>|[<span data-ttu-id="77737-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="77737-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="77737-191">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="77737-191">The Application's availability.</span></span> <span data-ttu-id="77737-192">继承自 [managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="77737-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="77737-193">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="77737-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="77737-194">version</span><span class="sxs-lookup"><span data-stu-id="77737-194">version</span></span>|<span data-ttu-id="77737-195">String</span><span class="sxs-lookup"><span data-stu-id="77737-195">String</span></span>|<span data-ttu-id="77737-196">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="77737-196">The Application's version.</span></span> <span data-ttu-id="77737-197">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="77737-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="77737-198">packageId</span><span class="sxs-lookup"><span data-stu-id="77737-198">packageId</span></span>|<span data-ttu-id="77737-199">String</span><span class="sxs-lookup"><span data-stu-id="77737-199">String</span></span>|<span data-ttu-id="77737-200">应用的包 ID。</span><span class="sxs-lookup"><span data-stu-id="77737-200">The app's package ID.</span></span>|
|<span data-ttu-id="77737-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="77737-201">appStoreUrl</span></span>|<span data-ttu-id="77737-202">String</span><span class="sxs-lookup"><span data-stu-id="77737-202">String</span></span>|<span data-ttu-id="77737-203">Android AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="77737-203">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="77737-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="77737-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="77737-205">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="77737-205">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="77737-206">最低受支持操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="77737-206">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="77737-207">响应</span><span class="sxs-lookup"><span data-stu-id="77737-207">Response</span></span>
<span data-ttu-id="77737-208">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="77737-208">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77737-209">示例</span><span class="sxs-lookup"><span data-stu-id="77737-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="77737-210">请求</span><span class="sxs-lookup"><span data-stu-id="77737-210">Request</span></span>
<span data-ttu-id="77737-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="77737-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1056

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v10_0": true,
    "v11_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="77737-212">响应</span><span class="sxs-lookup"><span data-stu-id="77737-212">Response</span></span>
<span data-ttu-id="77737-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77737-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1228

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v10_0": true,
    "v11_0": true
  }
}
```




