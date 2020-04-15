---
title: 更新 androidStoreApp
description: 更新 androidStoreApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 38954ac2ea4aad05e66405aa393e52aba14bb0d9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463186"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="2e136-103">更新 androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="2e136-103">Update androidStoreApp</span></span>

<span data-ttu-id="2e136-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e136-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e136-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2e136-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e136-106">更新 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2e136-106">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e136-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2e136-107">Prerequisites</span></span>
<span data-ttu-id="2e136-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e136-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e136-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e136-110">Permission type</span></span>|<span data-ttu-id="2e136-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2e136-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e136-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e136-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2e136-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e136-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2e136-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e136-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e136-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e136-115">Not supported.</span></span>|
|<span data-ttu-id="2e136-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e136-116">Application</span></span>|<span data-ttu-id="2e136-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e136-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e136-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e136-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="2e136-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e136-119">Request headers</span></span>
|<span data-ttu-id="2e136-120">标头</span><span class="sxs-lookup"><span data-stu-id="2e136-120">Header</span></span>|<span data-ttu-id="2e136-121">值</span><span class="sxs-lookup"><span data-stu-id="2e136-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e136-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e136-122">Authorization</span></span>|<span data-ttu-id="2e136-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2e136-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e136-124">接受</span><span class="sxs-lookup"><span data-stu-id="2e136-124">Accept</span></span>|<span data-ttu-id="2e136-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2e136-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e136-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e136-126">Request body</span></span>
<span data-ttu-id="2e136-127">在请求正文中，提供 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e136-127">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="2e136-128">下表显示了创建 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2e136-128">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="2e136-129">属性</span><span class="sxs-lookup"><span data-stu-id="2e136-129">Property</span></span>|<span data-ttu-id="2e136-130">类型</span><span class="sxs-lookup"><span data-stu-id="2e136-130">Type</span></span>|<span data-ttu-id="2e136-131">说明</span><span class="sxs-lookup"><span data-stu-id="2e136-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e136-132">id</span><span class="sxs-lookup"><span data-stu-id="2e136-132">id</span></span>|<span data-ttu-id="2e136-133">字符串</span><span class="sxs-lookup"><span data-stu-id="2e136-133">String</span></span>|<span data-ttu-id="2e136-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2e136-134">Key of the entity.</span></span> <span data-ttu-id="2e136-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e136-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e136-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2e136-136">displayName</span></span>|<span data-ttu-id="2e136-137">String</span><span class="sxs-lookup"><span data-stu-id="2e136-137">String</span></span>|<span data-ttu-id="2e136-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="2e136-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2e136-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e136-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e136-140">description</span><span class="sxs-lookup"><span data-stu-id="2e136-140">description</span></span>|<span data-ttu-id="2e136-141">字符串</span><span class="sxs-lookup"><span data-stu-id="2e136-141">String</span></span>|<span data-ttu-id="2e136-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="2e136-142">The description of the app.</span></span> <span data-ttu-id="2e136-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e136-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e136-144">publisher</span><span class="sxs-lookup"><span data-stu-id="2e136-144">publisher</span></span>|<span data-ttu-id="2e136-145">String</span><span class="sxs-lookup"><span data-stu-id="2e136-145">String</span></span>|<span data-ttu-id="2e136-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="2e136-146">The publisher of the app.</span></span> <span data-ttu-id="2e136-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e136-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e136-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2e136-148">largeIcon</span></span>|[<span data-ttu-id="2e136-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2e136-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2e136-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="2e136-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2e136-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e136-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e136-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2e136-152">createdDateTime</span></span>|<span data-ttu-id="2e136-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e136-153">DateTimeOffset</span></span>|<span data-ttu-id="2e136-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2e136-154">The date and time the app was created.</span></span> <span data-ttu-id="2e136-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e136-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e136-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e136-156">lastModifiedDateTime</span></span>|<span data-ttu-id="2e136-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e136-157">DateTimeOffset</span></span>|<span data-ttu-id="2e136-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2e136-158">The date and time the app was last modified.</span></span> <span data-ttu-id="2e136-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e136-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e136-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2e136-160">isFeatured</span></span>|<span data-ttu-id="2e136-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e136-161">Boolean</span></span>|<span data-ttu-id="2e136-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e136-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e136-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2e136-163">privacyInformationUrl</span></span>|<span data-ttu-id="2e136-164">String</span><span class="sxs-lookup"><span data-stu-id="2e136-164">String</span></span>|<span data-ttu-id="2e136-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="2e136-165">The privacy statement Url.</span></span> <span data-ttu-id="2e136-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e136-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e136-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2e136-167">informationUrl</span></span>|<span data-ttu-id="2e136-168">String</span><span class="sxs-lookup"><span data-stu-id="2e136-168">String</span></span>|<span data-ttu-id="2e136-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="2e136-169">The more information Url.</span></span> <span data-ttu-id="2e136-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e136-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e136-171">owner</span><span class="sxs-lookup"><span data-stu-id="2e136-171">owner</span></span>|<span data-ttu-id="2e136-172">String</span><span class="sxs-lookup"><span data-stu-id="2e136-172">String</span></span>|<span data-ttu-id="2e136-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="2e136-173">The owner of the app.</span></span> <span data-ttu-id="2e136-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e136-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e136-175">developer</span><span class="sxs-lookup"><span data-stu-id="2e136-175">developer</span></span>|<span data-ttu-id="2e136-176">String</span><span class="sxs-lookup"><span data-stu-id="2e136-176">String</span></span>|<span data-ttu-id="2e136-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="2e136-177">The developer of the app.</span></span> <span data-ttu-id="2e136-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e136-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e136-179">notes</span><span class="sxs-lookup"><span data-stu-id="2e136-179">notes</span></span>|<span data-ttu-id="2e136-180">String</span><span class="sxs-lookup"><span data-stu-id="2e136-180">String</span></span>|<span data-ttu-id="2e136-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="2e136-181">Notes for the app.</span></span> <span data-ttu-id="2e136-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e136-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e136-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="2e136-183">publishingState</span></span>|[<span data-ttu-id="2e136-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2e136-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2e136-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="2e136-185">The publishing state for the app.</span></span> <span data-ttu-id="2e136-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="2e136-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2e136-187">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="2e136-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2e136-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="2e136-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2e136-189">packageId</span><span class="sxs-lookup"><span data-stu-id="2e136-189">packageId</span></span>|<span data-ttu-id="2e136-190">String</span><span class="sxs-lookup"><span data-stu-id="2e136-190">String</span></span>|<span data-ttu-id="2e136-191">包标识符。</span><span class="sxs-lookup"><span data-stu-id="2e136-191">The package identifier.</span></span>|
|<span data-ttu-id="2e136-192">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="2e136-192">appStoreUrl</span></span>|<span data-ttu-id="2e136-193">String</span><span class="sxs-lookup"><span data-stu-id="2e136-193">String</span></span>|<span data-ttu-id="2e136-194">Android 应用商店 URL。</span><span class="sxs-lookup"><span data-stu-id="2e136-194">The Android app store URL.</span></span>|
|<span data-ttu-id="2e136-195">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2e136-195">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2e136-196">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2e136-196">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="2e136-197">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="2e136-197">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="2e136-198">响应</span><span class="sxs-lookup"><span data-stu-id="2e136-198">Response</span></span>
<span data-ttu-id="2e136-199">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2e136-199">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e136-200">示例</span><span class="sxs-lookup"><span data-stu-id="2e136-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e136-201">请求</span><span class="sxs-lookup"><span data-stu-id="2e136-201">Request</span></span>
<span data-ttu-id="2e136-202">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2e136-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 938

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
    "v5_1": true
  }
}
```

### <a name="response"></a><span data-ttu-id="2e136-203">响应</span><span class="sxs-lookup"><span data-stu-id="2e136-203">Response</span></span>
<span data-ttu-id="2e136-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2e136-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1110

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
  "publishingState": "processing",
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
    "v5_1": true
  }
}
```






