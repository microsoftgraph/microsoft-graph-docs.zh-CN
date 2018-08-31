# <a name="update-androidstoreapp"></a><span data-ttu-id="12395-101">更新 androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="12395-101">Update androidStoreApp</span></span>

> <span data-ttu-id="12395-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="12395-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12395-103">更新 [androidStoreApp](../resources/intune_apps_androidstoreapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="12395-103">Update the properties of a [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12395-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="12395-104">Prerequisites</span></span>
<span data-ttu-id="12395-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="12395-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="12395-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="12395-107">Permission type</span></span>|<span data-ttu-id="12395-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12395-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12395-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12395-109">Delegated (work or school account)</span></span>|<span data-ttu-id="12395-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12395-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="12395-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12395-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12395-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="12395-112">Not supported.</span></span>|
|<span data-ttu-id="12395-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="12395-113">Application</span></span>|<span data-ttu-id="12395-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="12395-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12395-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12395-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="12395-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="12395-116">Request headers</span></span>
|<span data-ttu-id="12395-117">标头</span><span class="sxs-lookup"><span data-stu-id="12395-117">Header</span></span>|<span data-ttu-id="12395-118">值</span><span class="sxs-lookup"><span data-stu-id="12395-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12395-119">授权</span><span class="sxs-lookup"><span data-stu-id="12395-119">Authorization</span></span>|<span data-ttu-id="12395-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12395-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12395-121">接受</span><span class="sxs-lookup"><span data-stu-id="12395-121">Accept</span></span>|<span data-ttu-id="12395-122">application/json</span><span class="sxs-lookup"><span data-stu-id="12395-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12395-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="12395-123">Request body</span></span>
<span data-ttu-id="12395-124">在请求正文中，提供 [androidStoreApp](../resources/intune_apps_androidstoreapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12395-124">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object.</span></span>

<span data-ttu-id="12395-125">下表显示了创建 [androidStoreApp](../resources/intune_apps_androidstoreapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="12395-125">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune_apps_androidstoreapp.md).</span></span>

|<span data-ttu-id="12395-126">属性</span><span class="sxs-lookup"><span data-stu-id="12395-126">Property</span></span>|<span data-ttu-id="12395-127">类型</span><span class="sxs-lookup"><span data-stu-id="12395-127">Type</span></span>|<span data-ttu-id="12395-128">说明</span><span class="sxs-lookup"><span data-stu-id="12395-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12395-129">id</span><span class="sxs-lookup"><span data-stu-id="12395-129">id</span></span>|<span data-ttu-id="12395-130">字符串</span><span class="sxs-lookup"><span data-stu-id="12395-130">String</span></span>|<span data-ttu-id="12395-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="12395-131">Key of the entity.</span></span> <span data-ttu-id="12395-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12395-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12395-133">displayName</span><span class="sxs-lookup"><span data-stu-id="12395-133">displayName</span></span>|<span data-ttu-id="12395-134">字符串</span><span class="sxs-lookup"><span data-stu-id="12395-134">String</span></span>|<span data-ttu-id="12395-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="12395-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="12395-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12395-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12395-137">description</span><span class="sxs-lookup"><span data-stu-id="12395-137">description</span></span>|<span data-ttu-id="12395-138">字符串</span><span class="sxs-lookup"><span data-stu-id="12395-138">String</span></span>|<span data-ttu-id="12395-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="12395-139">The description of the app.</span></span> <span data-ttu-id="12395-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12395-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12395-141">publisher</span><span class="sxs-lookup"><span data-stu-id="12395-141">publisher</span></span>|<span data-ttu-id="12395-142">字符串</span><span class="sxs-lookup"><span data-stu-id="12395-142">String</span></span>|<span data-ttu-id="12395-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="12395-143">The publisher of the app.</span></span> <span data-ttu-id="12395-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12395-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12395-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="12395-145">largeIcon</span></span>|[<span data-ttu-id="12395-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="12395-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="12395-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="12395-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="12395-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12395-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12395-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12395-149">createdDateTime</span></span>|<span data-ttu-id="12395-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12395-150">DateTimeOffset</span></span>|<span data-ttu-id="12395-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="12395-151">The date and time the app was created.</span></span> <span data-ttu-id="12395-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12395-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12395-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12395-153">lastModifiedDateTime</span></span>|<span data-ttu-id="12395-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12395-154">DateTimeOffset</span></span>|<span data-ttu-id="12395-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="12395-155">The date and time the app was last modified.</span></span> <span data-ttu-id="12395-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12395-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12395-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="12395-157">isFeatured</span></span>|<span data-ttu-id="12395-158">布尔值</span><span class="sxs-lookup"><span data-stu-id="12395-158">Boolean</span></span>|<span data-ttu-id="12395-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12395-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12395-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="12395-160">privacyInformationUrl</span></span>|<span data-ttu-id="12395-161">字符串</span><span class="sxs-lookup"><span data-stu-id="12395-161">String</span></span>|<span data-ttu-id="12395-162">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="12395-162">The privacy statement Url.</span></span> <span data-ttu-id="12395-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12395-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12395-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="12395-164">informationUrl</span></span>|<span data-ttu-id="12395-165">字符串</span><span class="sxs-lookup"><span data-stu-id="12395-165">String</span></span>|<span data-ttu-id="12395-166">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="12395-166">The more information Url.</span></span> <span data-ttu-id="12395-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12395-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12395-168">owner</span><span class="sxs-lookup"><span data-stu-id="12395-168">owner</span></span>|<span data-ttu-id="12395-169">字符串</span><span class="sxs-lookup"><span data-stu-id="12395-169">String</span></span>|<span data-ttu-id="12395-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="12395-170">The owner of the app.</span></span> <span data-ttu-id="12395-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12395-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12395-172">developer</span><span class="sxs-lookup"><span data-stu-id="12395-172">developer</span></span>|<span data-ttu-id="12395-173">字符串</span><span class="sxs-lookup"><span data-stu-id="12395-173">String</span></span>|<span data-ttu-id="12395-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="12395-174">The developer of the app.</span></span> <span data-ttu-id="12395-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12395-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12395-176">notes</span><span class="sxs-lookup"><span data-stu-id="12395-176">notes</span></span>|<span data-ttu-id="12395-177">字符串</span><span class="sxs-lookup"><span data-stu-id="12395-177">String</span></span>|<span data-ttu-id="12395-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="12395-178">Notes for the app.</span></span> <span data-ttu-id="12395-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12395-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12395-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="12395-180">publishingState</span></span>|[<span data-ttu-id="12395-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="12395-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="12395-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="12395-182">The publishing state for the app.</span></span> <span data-ttu-id="12395-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="12395-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="12395-184">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="12395-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="12395-185">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="12395-185">The possible values are `notPublished`, `processing`, `published`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="12395-186">packageId</span><span class="sxs-lookup"><span data-stu-id="12395-186">packageId</span></span>|<span data-ttu-id="12395-187">字符串</span><span class="sxs-lookup"><span data-stu-id="12395-187">String</span></span>|<span data-ttu-id="12395-188">包标识符。</span><span class="sxs-lookup"><span data-stu-id="12395-188">The package identifier.</span></span>|
|<span data-ttu-id="12395-189">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="12395-189">appStoreUrl</span></span>|<span data-ttu-id="12395-190">字符串</span><span class="sxs-lookup"><span data-stu-id="12395-190">String</span></span>|<span data-ttu-id="12395-191">Android 应用商店 URL。</span><span class="sxs-lookup"><span data-stu-id="12395-191">The Android app store URL.</span></span>|
|<span data-ttu-id="12395-192">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="12395-192">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="12395-193">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="12395-193">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="12395-194">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="12395-194">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="12395-195">响应</span><span class="sxs-lookup"><span data-stu-id="12395-195">Response</span></span>
<span data-ttu-id="12395-196">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidStoreApp](../resources/intune_apps_androidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12395-196">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12395-197">示例</span><span class="sxs-lookup"><span data-stu-id="12395-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="12395-198">请求</span><span class="sxs-lookup"><span data-stu-id="12395-198">Request</span></span>
<span data-ttu-id="12395-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12395-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 948

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

### <a name="response"></a><span data-ttu-id="12395-200">响应</span><span class="sxs-lookup"><span data-stu-id="12395-200">Response</span></span>
<span data-ttu-id="12395-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12395-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



