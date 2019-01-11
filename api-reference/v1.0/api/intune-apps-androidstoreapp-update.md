---
title: 更新 androidStoreApp
description: 更新 androidStoreApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d233792054166dcb88c2b8a29891ecad13a743de
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847290"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="e4fc0-103">更新 androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="e4fc0-103">Update androidStoreApp</span></span>

> <span data-ttu-id="e4fc0-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4fc0-105">更新 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-105">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e4fc0-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="e4fc0-106">Prerequisites</span></span>
<span data-ttu-id="e4fc0-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e4fc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4fc0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4fc0-109">Permission type</span></span>|<span data-ttu-id="e4fc0-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e4fc0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4fc0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4fc0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e4fc0-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4fc0-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e4fc0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4fc0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4fc0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-114">Not supported.</span></span>|
|<span data-ttu-id="e4fc0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4fc0-115">Application</span></span>|<span data-ttu-id="e4fc0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4fc0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4fc0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="e4fc0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4fc0-118">Request headers</span></span>
|<span data-ttu-id="e4fc0-119">标头</span><span class="sxs-lookup"><span data-stu-id="e4fc0-119">Header</span></span>|<span data-ttu-id="e4fc0-120">值</span><span class="sxs-lookup"><span data-stu-id="e4fc0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4fc0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4fc0-121">Authorization</span></span>|<span data-ttu-id="e4fc0-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4fc0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e4fc0-123">Accept</span></span>|<span data-ttu-id="e4fc0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e4fc0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4fc0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4fc0-125">Request body</span></span>
<span data-ttu-id="e4fc0-126">在请求正文中，提供 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-126">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="e4fc0-127">下表显示了创建 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-127">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="e4fc0-128">属性</span><span class="sxs-lookup"><span data-stu-id="e4fc0-128">Property</span></span>|<span data-ttu-id="e4fc0-129">类型</span><span class="sxs-lookup"><span data-stu-id="e4fc0-129">Type</span></span>|<span data-ttu-id="e4fc0-130">说明</span><span class="sxs-lookup"><span data-stu-id="e4fc0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4fc0-131">id</span><span class="sxs-lookup"><span data-stu-id="e4fc0-131">id</span></span>|<span data-ttu-id="e4fc0-132">String</span><span class="sxs-lookup"><span data-stu-id="e4fc0-132">String</span></span>|<span data-ttu-id="e4fc0-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-133">Key of the entity.</span></span> <span data-ttu-id="e4fc0-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e4fc0-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4fc0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e4fc0-135">displayName</span></span>|<span data-ttu-id="e4fc0-136">String</span><span class="sxs-lookup"><span data-stu-id="e4fc0-136">String</span></span>|<span data-ttu-id="e4fc0-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e4fc0-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e4fc0-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4fc0-139">description</span><span class="sxs-lookup"><span data-stu-id="e4fc0-139">description</span></span>|<span data-ttu-id="e4fc0-140">String</span><span class="sxs-lookup"><span data-stu-id="e4fc0-140">String</span></span>|<span data-ttu-id="e4fc0-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-141">The description of the app.</span></span> <span data-ttu-id="e4fc0-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e4fc0-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4fc0-143">publisher</span><span class="sxs-lookup"><span data-stu-id="e4fc0-143">publisher</span></span>|<span data-ttu-id="e4fc0-144">String</span><span class="sxs-lookup"><span data-stu-id="e4fc0-144">String</span></span>|<span data-ttu-id="e4fc0-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-145">The publisher of the app.</span></span> <span data-ttu-id="e4fc0-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e4fc0-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4fc0-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e4fc0-147">largeIcon</span></span>|[<span data-ttu-id="e4fc0-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e4fc0-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e4fc0-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e4fc0-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e4fc0-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4fc0-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4fc0-151">createdDateTime</span></span>|<span data-ttu-id="e4fc0-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4fc0-152">DateTimeOffset</span></span>|<span data-ttu-id="e4fc0-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-153">The date and time the app was created.</span></span> <span data-ttu-id="e4fc0-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e4fc0-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4fc0-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4fc0-155">lastModifiedDateTime</span></span>|<span data-ttu-id="e4fc0-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4fc0-156">DateTimeOffset</span></span>|<span data-ttu-id="e4fc0-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-157">The date and time the app was last modified.</span></span> <span data-ttu-id="e4fc0-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e4fc0-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4fc0-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e4fc0-159">isFeatured</span></span>|<span data-ttu-id="e4fc0-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4fc0-160">Boolean</span></span>|<span data-ttu-id="e4fc0-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e4fc0-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4fc0-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e4fc0-162">privacyInformationUrl</span></span>|<span data-ttu-id="e4fc0-163">String</span><span class="sxs-lookup"><span data-stu-id="e4fc0-163">String</span></span>|<span data-ttu-id="e4fc0-164">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-164">The privacy statement Url.</span></span> <span data-ttu-id="e4fc0-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e4fc0-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4fc0-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e4fc0-166">informationUrl</span></span>|<span data-ttu-id="e4fc0-167">String</span><span class="sxs-lookup"><span data-stu-id="e4fc0-167">String</span></span>|<span data-ttu-id="e4fc0-168">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-168">The more information Url.</span></span> <span data-ttu-id="e4fc0-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e4fc0-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4fc0-170">owner</span><span class="sxs-lookup"><span data-stu-id="e4fc0-170">owner</span></span>|<span data-ttu-id="e4fc0-171">String</span><span class="sxs-lookup"><span data-stu-id="e4fc0-171">String</span></span>|<span data-ttu-id="e4fc0-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-172">The owner of the app.</span></span> <span data-ttu-id="e4fc0-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e4fc0-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4fc0-174">developer</span><span class="sxs-lookup"><span data-stu-id="e4fc0-174">developer</span></span>|<span data-ttu-id="e4fc0-175">String</span><span class="sxs-lookup"><span data-stu-id="e4fc0-175">String</span></span>|<span data-ttu-id="e4fc0-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-176">The developer of the app.</span></span> <span data-ttu-id="e4fc0-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e4fc0-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4fc0-178">notes</span><span class="sxs-lookup"><span data-stu-id="e4fc0-178">notes</span></span>|<span data-ttu-id="e4fc0-179">String</span><span class="sxs-lookup"><span data-stu-id="e4fc0-179">String</span></span>|<span data-ttu-id="e4fc0-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-180">Notes for the app.</span></span> <span data-ttu-id="e4fc0-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e4fc0-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4fc0-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="e4fc0-182">publishingState</span></span>|[<span data-ttu-id="e4fc0-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e4fc0-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e4fc0-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-184">The publishing state for the app.</span></span> <span data-ttu-id="e4fc0-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e4fc0-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e4fc0-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e4fc0-188">packageId</span><span class="sxs-lookup"><span data-stu-id="e4fc0-188">packageId</span></span>|<span data-ttu-id="e4fc0-189">String</span><span class="sxs-lookup"><span data-stu-id="e4fc0-189">String</span></span>|<span data-ttu-id="e4fc0-190">包标识符。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-190">The package identifier.</span></span>|
|<span data-ttu-id="e4fc0-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="e4fc0-191">appStoreUrl</span></span>|<span data-ttu-id="e4fc0-192">String</span><span class="sxs-lookup"><span data-stu-id="e4fc0-192">String</span></span>|<span data-ttu-id="e4fc0-193">Android 应用商店 URL。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-193">The Android app store URL.</span></span>|
|<span data-ttu-id="e4fc0-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e4fc0-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e4fc0-195">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e4fc0-195">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="e4fc0-196">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="e4fc0-197">响应</span><span class="sxs-lookup"><span data-stu-id="e4fc0-197">Response</span></span>
<span data-ttu-id="e4fc0-198">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-198">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4fc0-199">示例</span><span class="sxs-lookup"><span data-stu-id="e4fc0-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="e4fc0-200">请求</span><span class="sxs-lookup"><span data-stu-id="e4fc0-200">Request</span></span>
<span data-ttu-id="e4fc0-201">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e4fc0-202">响应</span><span class="sxs-lookup"><span data-stu-id="e4fc0-202">Response</span></span>
<span data-ttu-id="e4fc0-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e4fc0-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



