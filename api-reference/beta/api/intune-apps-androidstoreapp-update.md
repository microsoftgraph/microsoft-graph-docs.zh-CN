---
title: 更新 androidStoreApp
description: 更新 androidStoreApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8cd9efebe6d7a68c2b0e023e17e881850e01843f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818835"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="bd288-103">更新 androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="bd288-103">Update androidStoreApp</span></span>

> <span data-ttu-id="bd288-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bd288-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd288-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bd288-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd288-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bd288-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd288-107">更新 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bd288-107">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bd288-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bd288-108">Prerequisites</span></span>
<span data-ttu-id="bd288-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="bd288-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd288-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd288-111">Permission type</span></span>|<span data-ttu-id="bd288-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bd288-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd288-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd288-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd288-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd288-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bd288-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd288-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd288-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd288-116">Not supported.</span></span>|
|<span data-ttu-id="bd288-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd288-117">Application</span></span>|<span data-ttu-id="bd288-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd288-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd288-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd288-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="bd288-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd288-120">Request headers</span></span>
|<span data-ttu-id="bd288-121">标头</span><span class="sxs-lookup"><span data-stu-id="bd288-121">Header</span></span>|<span data-ttu-id="bd288-122">值</span><span class="sxs-lookup"><span data-stu-id="bd288-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd288-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd288-123">Authorization</span></span>|<span data-ttu-id="bd288-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bd288-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd288-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bd288-125">Accept</span></span>|<span data-ttu-id="bd288-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd288-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd288-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd288-127">Request body</span></span>
<span data-ttu-id="bd288-128">在请求正文中，提供 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd288-128">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="bd288-129">下表显示了创建 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bd288-129">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="bd288-130">属性</span><span class="sxs-lookup"><span data-stu-id="bd288-130">Property</span></span>|<span data-ttu-id="bd288-131">类型</span><span class="sxs-lookup"><span data-stu-id="bd288-131">Type</span></span>|<span data-ttu-id="bd288-132">说明</span><span class="sxs-lookup"><span data-stu-id="bd288-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd288-133">id</span><span class="sxs-lookup"><span data-stu-id="bd288-133">id</span></span>|<span data-ttu-id="bd288-134">String</span><span class="sxs-lookup"><span data-stu-id="bd288-134">String</span></span>|<span data-ttu-id="bd288-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bd288-135">Key of the entity.</span></span> <span data-ttu-id="bd288-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd288-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd288-137">displayName</span><span class="sxs-lookup"><span data-stu-id="bd288-137">displayName</span></span>|<span data-ttu-id="bd288-138">String</span><span class="sxs-lookup"><span data-stu-id="bd288-138">String</span></span>|<span data-ttu-id="bd288-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="bd288-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bd288-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd288-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd288-141">description</span><span class="sxs-lookup"><span data-stu-id="bd288-141">description</span></span>|<span data-ttu-id="bd288-142">String</span><span class="sxs-lookup"><span data-stu-id="bd288-142">String</span></span>|<span data-ttu-id="bd288-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="bd288-143">The description of the app.</span></span> <span data-ttu-id="bd288-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd288-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd288-145">publisher</span><span class="sxs-lookup"><span data-stu-id="bd288-145">publisher</span></span>|<span data-ttu-id="bd288-146">String</span><span class="sxs-lookup"><span data-stu-id="bd288-146">String</span></span>|<span data-ttu-id="bd288-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="bd288-147">The publisher of the app.</span></span> <span data-ttu-id="bd288-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd288-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd288-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bd288-149">largeIcon</span></span>|[<span data-ttu-id="bd288-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bd288-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bd288-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="bd288-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bd288-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd288-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd288-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd288-153">createdDateTime</span></span>|<span data-ttu-id="bd288-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd288-154">DateTimeOffset</span></span>|<span data-ttu-id="bd288-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bd288-155">The date and time the app was created.</span></span> <span data-ttu-id="bd288-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd288-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd288-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd288-157">lastModifiedDateTime</span></span>|<span data-ttu-id="bd288-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd288-158">DateTimeOffset</span></span>|<span data-ttu-id="bd288-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bd288-159">The date and time the app was last modified.</span></span> <span data-ttu-id="bd288-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd288-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd288-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bd288-161">isFeatured</span></span>|<span data-ttu-id="bd288-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd288-162">Boolean</span></span>|<span data-ttu-id="bd288-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd288-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd288-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bd288-164">privacyInformationUrl</span></span>|<span data-ttu-id="bd288-165">String</span><span class="sxs-lookup"><span data-stu-id="bd288-165">String</span></span>|<span data-ttu-id="bd288-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="bd288-166">The privacy statement Url.</span></span> <span data-ttu-id="bd288-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd288-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd288-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bd288-168">informationUrl</span></span>|<span data-ttu-id="bd288-169">String</span><span class="sxs-lookup"><span data-stu-id="bd288-169">String</span></span>|<span data-ttu-id="bd288-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="bd288-170">The more information Url.</span></span> <span data-ttu-id="bd288-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd288-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd288-172">owner</span><span class="sxs-lookup"><span data-stu-id="bd288-172">owner</span></span>|<span data-ttu-id="bd288-173">String</span><span class="sxs-lookup"><span data-stu-id="bd288-173">String</span></span>|<span data-ttu-id="bd288-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="bd288-174">The owner of the app.</span></span> <span data-ttu-id="bd288-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd288-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd288-176">developer</span><span class="sxs-lookup"><span data-stu-id="bd288-176">developer</span></span>|<span data-ttu-id="bd288-177">String</span><span class="sxs-lookup"><span data-stu-id="bd288-177">String</span></span>|<span data-ttu-id="bd288-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="bd288-178">The developer of the app.</span></span> <span data-ttu-id="bd288-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd288-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd288-180">notes</span><span class="sxs-lookup"><span data-stu-id="bd288-180">notes</span></span>|<span data-ttu-id="bd288-181">String</span><span class="sxs-lookup"><span data-stu-id="bd288-181">String</span></span>|<span data-ttu-id="bd288-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="bd288-182">Notes for the app.</span></span> <span data-ttu-id="bd288-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd288-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd288-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="bd288-184">uploadState</span></span>|<span data-ttu-id="bd288-185">Int32</span><span class="sxs-lookup"><span data-stu-id="bd288-185">Int32</span></span>|<span data-ttu-id="bd288-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="bd288-186">The upload state.</span></span> <span data-ttu-id="bd288-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd288-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd288-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="bd288-188">publishingState</span></span>|[<span data-ttu-id="bd288-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bd288-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bd288-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="bd288-190">The publishing state for the app.</span></span> <span data-ttu-id="bd288-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="bd288-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bd288-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="bd288-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="bd288-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="bd288-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bd288-194">packageId</span><span class="sxs-lookup"><span data-stu-id="bd288-194">packageId</span></span>|<span data-ttu-id="bd288-195">String</span><span class="sxs-lookup"><span data-stu-id="bd288-195">String</span></span>|<span data-ttu-id="bd288-196">包标识符。</span><span class="sxs-lookup"><span data-stu-id="bd288-196">The package identifier.</span></span>|
|<span data-ttu-id="bd288-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="bd288-197">appIdentifier</span></span>|<span data-ttu-id="bd288-198">String</span><span class="sxs-lookup"><span data-stu-id="bd288-198">String</span></span>|<span data-ttu-id="bd288-199">标识名称。</span><span class="sxs-lookup"><span data-stu-id="bd288-199">The Identity Name.</span></span>|
|<span data-ttu-id="bd288-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="bd288-200">appStoreUrl</span></span>|<span data-ttu-id="bd288-201">String</span><span class="sxs-lookup"><span data-stu-id="bd288-201">String</span></span>|<span data-ttu-id="bd288-202">Android 应用商店 URL。</span><span class="sxs-lookup"><span data-stu-id="bd288-202">The Android app store URL.</span></span>|
|<span data-ttu-id="bd288-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bd288-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="bd288-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bd288-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="bd288-205">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="bd288-205">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="bd288-206">响应</span><span class="sxs-lookup"><span data-stu-id="bd288-206">Response</span></span>
<span data-ttu-id="bd288-207">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bd288-207">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd288-208">示例</span><span class="sxs-lookup"><span data-stu-id="bd288-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="bd288-209">请求</span><span class="sxs-lookup"><span data-stu-id="bd288-209">Request</span></span>
<span data-ttu-id="bd288-210">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bd288-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1128

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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
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
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="bd288-211">响应</span><span class="sxs-lookup"><span data-stu-id="bd288-211">Response</span></span>
<span data-ttu-id="bd288-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bd288-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1290

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
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
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```





