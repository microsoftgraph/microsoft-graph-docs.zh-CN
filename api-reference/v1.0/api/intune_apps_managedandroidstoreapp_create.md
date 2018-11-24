# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="fb408-101">创建 managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="fb408-101">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="fb408-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fb408-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb408-103">创建新的 [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb408-103">Create a new [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb408-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="fb408-104">Prerequisites</span></span>
<span data-ttu-id="fb408-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fb408-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fb408-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb408-107">Permission type</span></span>|<span data-ttu-id="fb408-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fb408-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb408-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb408-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fb408-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb408-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fb408-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb408-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb408-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb408-112">Not supported.</span></span>|
|<span data-ttu-id="fb408-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb408-113">Application</span></span>|<span data-ttu-id="fb408-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb408-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb408-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb408-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fb408-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb408-116">Request headers</span></span>
|<span data-ttu-id="fb408-117">标头</span><span class="sxs-lookup"><span data-stu-id="fb408-117">Header</span></span>|<span data-ttu-id="fb408-118">值</span><span class="sxs-lookup"><span data-stu-id="fb408-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb408-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb408-119">Authorization</span></span>|<span data-ttu-id="fb408-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fb408-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb408-121">Accept</span><span class="sxs-lookup"><span data-stu-id="fb408-121">Accept</span></span>|<span data-ttu-id="fb408-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fb408-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb408-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb408-123">Request body</span></span>
<span data-ttu-id="fb408-124">在请求正文中，提供 managedAndroidStoreApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb408-124">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="fb408-125">下表显示了创建 managedAndroidStoreApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fb408-125">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="fb408-126">属性</span><span class="sxs-lookup"><span data-stu-id="fb408-126">Property</span></span>|<span data-ttu-id="fb408-127">类型</span><span class="sxs-lookup"><span data-stu-id="fb408-127">Type</span></span>|<span data-ttu-id="fb408-128">说明</span><span class="sxs-lookup"><span data-stu-id="fb408-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb408-129">id</span><span class="sxs-lookup"><span data-stu-id="fb408-129">id</span></span>|<span data-ttu-id="fb408-130">String</span><span class="sxs-lookup"><span data-stu-id="fb408-130">String</span></span>|<span data-ttu-id="fb408-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fb408-131">Key of the entity.</span></span> <span data-ttu-id="fb408-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb408-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb408-133">displayName</span><span class="sxs-lookup"><span data-stu-id="fb408-133">displayName</span></span>|<span data-ttu-id="fb408-134">String</span><span class="sxs-lookup"><span data-stu-id="fb408-134">String</span></span>|<span data-ttu-id="fb408-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="fb408-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fb408-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb408-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb408-137">description</span><span class="sxs-lookup"><span data-stu-id="fb408-137">description</span></span>|<span data-ttu-id="fb408-138">String</span><span class="sxs-lookup"><span data-stu-id="fb408-138">String</span></span>|<span data-ttu-id="fb408-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="fb408-139">The description of the app.</span></span> <span data-ttu-id="fb408-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb408-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb408-141">publisher</span><span class="sxs-lookup"><span data-stu-id="fb408-141">publisher</span></span>|<span data-ttu-id="fb408-142">String</span><span class="sxs-lookup"><span data-stu-id="fb408-142">String</span></span>|<span data-ttu-id="fb408-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="fb408-143">The publisher of the app.</span></span> <span data-ttu-id="fb408-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb408-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb408-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fb408-145">largeIcon</span></span>|[<span data-ttu-id="fb408-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fb408-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="fb408-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="fb408-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fb408-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb408-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb408-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb408-149">createdDateTime</span></span>|<span data-ttu-id="fb408-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb408-150">DateTimeOffset</span></span>|<span data-ttu-id="fb408-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fb408-151">The date and time the app was created.</span></span> <span data-ttu-id="fb408-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb408-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb408-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb408-153">lastModifiedDateTime</span></span>|<span data-ttu-id="fb408-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb408-154">DateTimeOffset</span></span>|<span data-ttu-id="fb408-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fb408-155">The date and time the app was last modified.</span></span> <span data-ttu-id="fb408-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb408-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb408-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fb408-157">isFeatured</span></span>|<span data-ttu-id="fb408-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb408-158">Boolean</span></span>|<span data-ttu-id="fb408-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb408-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb408-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fb408-160">privacyInformationUrl</span></span>|<span data-ttu-id="fb408-161">String</span><span class="sxs-lookup"><span data-stu-id="fb408-161">String</span></span>|<span data-ttu-id="fb408-162">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="fb408-162">The privacy statement Url.</span></span> <span data-ttu-id="fb408-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb408-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb408-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fb408-164">informationUrl</span></span>|<span data-ttu-id="fb408-165">String</span><span class="sxs-lookup"><span data-stu-id="fb408-165">String</span></span>|<span data-ttu-id="fb408-166">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="fb408-166">The more information Url.</span></span> <span data-ttu-id="fb408-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb408-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb408-168">owner</span><span class="sxs-lookup"><span data-stu-id="fb408-168">owner</span></span>|<span data-ttu-id="fb408-169">String</span><span class="sxs-lookup"><span data-stu-id="fb408-169">String</span></span>|<span data-ttu-id="fb408-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="fb408-170">The owner of the app.</span></span> <span data-ttu-id="fb408-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb408-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb408-172">developer</span><span class="sxs-lookup"><span data-stu-id="fb408-172">developer</span></span>|<span data-ttu-id="fb408-173">String</span><span class="sxs-lookup"><span data-stu-id="fb408-173">String</span></span>|<span data-ttu-id="fb408-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="fb408-174">The developer of the app.</span></span> <span data-ttu-id="fb408-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb408-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb408-176">notes</span><span class="sxs-lookup"><span data-stu-id="fb408-176">notes</span></span>|<span data-ttu-id="fb408-177">String</span><span class="sxs-lookup"><span data-stu-id="fb408-177">String</span></span>|<span data-ttu-id="fb408-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="fb408-178">Notes for the app.</span></span> <span data-ttu-id="fb408-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb408-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb408-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="fb408-180">publishingState</span></span>|[<span data-ttu-id="fb408-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="fb408-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="fb408-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="fb408-182">The publishing state for the app.</span></span> <span data-ttu-id="fb408-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="fb408-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fb408-184">继承自[mobileApp](../resources/intune_apps_mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="fb408-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="fb408-185">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="fb408-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fb408-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="fb408-186">appAvailability</span></span>|[<span data-ttu-id="fb408-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="fb408-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="fb408-188">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="fb408-188">The Application's availability.</span></span> <span data-ttu-id="fb408-189">继承自[managedApp](../resources/intune_apps_managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="fb408-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md).</span></span> <span data-ttu-id="fb408-190">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="fb408-190">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="fb408-191">version</span><span class="sxs-lookup"><span data-stu-id="fb408-191">version</span></span>|<span data-ttu-id="fb408-192">String</span><span class="sxs-lookup"><span data-stu-id="fb408-192">String</span></span>|<span data-ttu-id="fb408-193">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="fb408-193">The Application's version.</span></span> <span data-ttu-id="fb408-194">继承自 [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb408-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="fb408-195">packageId</span><span class="sxs-lookup"><span data-stu-id="fb408-195">packageId</span></span>|<span data-ttu-id="fb408-196">String</span><span class="sxs-lookup"><span data-stu-id="fb408-196">String</span></span>|<span data-ttu-id="fb408-197">应用的包 ID。</span><span class="sxs-lookup"><span data-stu-id="fb408-197">The app's package ID.</span></span>|
|<span data-ttu-id="fb408-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="fb408-198">appStoreUrl</span></span>|<span data-ttu-id="fb408-199">String</span><span class="sxs-lookup"><span data-stu-id="fb408-199">String</span></span>|<span data-ttu-id="fb408-200">Android AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="fb408-200">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="fb408-201">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fb408-201">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fb408-202">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fb408-202">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="fb408-203">最低受支持操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="fb408-203">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="fb408-204">响应</span><span class="sxs-lookup"><span data-stu-id="fb408-204">Response</span></span>
<span data-ttu-id="fb408-205">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb408-205">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb408-206">示例</span><span class="sxs-lookup"><span data-stu-id="fb408-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb408-207">请求</span><span class="sxs-lookup"><span data-stu-id="fb408-207">Request</span></span>
<span data-ttu-id="fb408-208">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb408-208">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1016

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
    "v5_1": true
  }
}
```

### <a name="response"></a><span data-ttu-id="fb408-209">响应</span><span class="sxs-lookup"><span data-stu-id="fb408-209">Response</span></span>
<span data-ttu-id="fb408-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb408-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1188

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
    "v5_1": true
  }
}
```



