# <a name="create-managediosstoreapp"></a><span data-ttu-id="3576e-101">创建 managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="3576e-101">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="3576e-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3576e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3576e-103">创建新的 [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3576e-103">Create a new [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3576e-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="3576e-104">Prerequisites</span></span>
<span data-ttu-id="3576e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3576e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3576e-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="3576e-107">Permission type</span></span>|<span data-ttu-id="3576e-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3576e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3576e-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3576e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3576e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3576e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3576e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3576e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3576e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="3576e-112">Not supported.</span></span>|
|<span data-ttu-id="3576e-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="3576e-113">Application</span></span>|<span data-ttu-id="3576e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3576e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3576e-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3576e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3576e-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="3576e-116">Request headers</span></span>
|<span data-ttu-id="3576e-117">标头</span><span class="sxs-lookup"><span data-stu-id="3576e-117">Header</span></span>|<span data-ttu-id="3576e-118">值</span><span class="sxs-lookup"><span data-stu-id="3576e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3576e-119">授权</span><span class="sxs-lookup"><span data-stu-id="3576e-119">Authorization</span></span>|<span data-ttu-id="3576e-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3576e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3576e-121">接受</span><span class="sxs-lookup"><span data-stu-id="3576e-121">Accept</span></span>|<span data-ttu-id="3576e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3576e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3576e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3576e-123">Request body</span></span>
<span data-ttu-id="3576e-124">在请求正文中，提供 managedIOSStoreApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3576e-124">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="3576e-125">下表显示创建 managedIOSStoreApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3576e-125">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="3576e-126">属性</span><span class="sxs-lookup"><span data-stu-id="3576e-126">Property</span></span>|<span data-ttu-id="3576e-127">类型</span><span class="sxs-lookup"><span data-stu-id="3576e-127">Type</span></span>|<span data-ttu-id="3576e-128">说明</span><span class="sxs-lookup"><span data-stu-id="3576e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3576e-129">id</span><span class="sxs-lookup"><span data-stu-id="3576e-129">id</span></span>|<span data-ttu-id="3576e-130">字符串</span><span class="sxs-lookup"><span data-stu-id="3576e-130">String</span></span>|<span data-ttu-id="3576e-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3576e-131">Key of the entity.</span></span> <span data-ttu-id="3576e-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3576e-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3576e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3576e-133">displayName</span></span>|<span data-ttu-id="3576e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="3576e-134">String</span></span>|<span data-ttu-id="3576e-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="3576e-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3576e-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3576e-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3576e-137">description</span><span class="sxs-lookup"><span data-stu-id="3576e-137">description</span></span>|<span data-ttu-id="3576e-138">字符串</span><span class="sxs-lookup"><span data-stu-id="3576e-138">String</span></span>|<span data-ttu-id="3576e-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="3576e-139">The description of the app.</span></span> <span data-ttu-id="3576e-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3576e-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3576e-141">publisher</span><span class="sxs-lookup"><span data-stu-id="3576e-141">publisher</span></span>|<span data-ttu-id="3576e-142">字符串</span><span class="sxs-lookup"><span data-stu-id="3576e-142">String</span></span>|<span data-ttu-id="3576e-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="3576e-143">The publisher of the app.</span></span> <span data-ttu-id="3576e-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3576e-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3576e-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3576e-145">largeIcon</span></span>|[<span data-ttu-id="3576e-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3576e-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="3576e-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="3576e-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3576e-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3576e-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3576e-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3576e-149">createdDateTime</span></span>|<span data-ttu-id="3576e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3576e-150">DateTimeOffset</span></span>|<span data-ttu-id="3576e-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3576e-151">The date and time the app was created.</span></span> <span data-ttu-id="3576e-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3576e-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3576e-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3576e-153">lastModifiedDateTime</span></span>|<span data-ttu-id="3576e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3576e-154">DateTimeOffset</span></span>|<span data-ttu-id="3576e-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3576e-155">The date and time the app was last modified.</span></span> <span data-ttu-id="3576e-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3576e-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3576e-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3576e-157">isFeatured</span></span>|<span data-ttu-id="3576e-158">布尔</span><span class="sxs-lookup"><span data-stu-id="3576e-158">Boolean</span></span>|<span data-ttu-id="3576e-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3576e-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3576e-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3576e-160">privacyInformationUrl</span></span>|<span data-ttu-id="3576e-161">字符串</span><span class="sxs-lookup"><span data-stu-id="3576e-161">String</span></span>|<span data-ttu-id="3576e-162">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="3576e-162">The privacy statement Url.</span></span> <span data-ttu-id="3576e-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3576e-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3576e-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3576e-164">informationUrl</span></span>|<span data-ttu-id="3576e-165">字符串</span><span class="sxs-lookup"><span data-stu-id="3576e-165">String</span></span>|<span data-ttu-id="3576e-166">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="3576e-166">The more information Url.</span></span> <span data-ttu-id="3576e-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3576e-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3576e-168">owner</span><span class="sxs-lookup"><span data-stu-id="3576e-168">owner</span></span>|<span data-ttu-id="3576e-169">字符串</span><span class="sxs-lookup"><span data-stu-id="3576e-169">String</span></span>|<span data-ttu-id="3576e-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="3576e-170">The owner of the app.</span></span> <span data-ttu-id="3576e-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3576e-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3576e-172">developer</span><span class="sxs-lookup"><span data-stu-id="3576e-172">developer</span></span>|<span data-ttu-id="3576e-173">字符串</span><span class="sxs-lookup"><span data-stu-id="3576e-173">String</span></span>|<span data-ttu-id="3576e-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="3576e-174">The developer of the app.</span></span> <span data-ttu-id="3576e-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3576e-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3576e-176">notes</span><span class="sxs-lookup"><span data-stu-id="3576e-176">notes</span></span>|<span data-ttu-id="3576e-177">字符串</span><span class="sxs-lookup"><span data-stu-id="3576e-177">String</span></span>|<span data-ttu-id="3576e-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="3576e-178">Notes for the app.</span></span> <span data-ttu-id="3576e-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3576e-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3576e-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="3576e-180">publishingState</span></span>|[<span data-ttu-id="3576e-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3576e-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="3576e-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="3576e-182">The publishing state for the app.</span></span> <span data-ttu-id="3576e-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="3576e-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3576e-184">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="3576e-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="3576e-185">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="3576e-185">The possible values are `notPublished`, `processing`, `published`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="3576e-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="3576e-186">appAvailability</span></span>|[<span data-ttu-id="3576e-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="3576e-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="3576e-188">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="3576e-188">The Application's availability.</span></span> <span data-ttu-id="3576e-189">继承自 [managedApp](../resources/intune_apps_managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="3576e-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span> <span data-ttu-id="3576e-190">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="3576e-190">The possible values are:</span></span>|
|<span data-ttu-id="3576e-191">version</span><span class="sxs-lookup"><span data-stu-id="3576e-191">version</span></span>|<span data-ttu-id="3576e-192">字符串</span><span class="sxs-lookup"><span data-stu-id="3576e-192">String</span></span>|<span data-ttu-id="3576e-193">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="3576e-193">The Application's version.</span></span> <span data-ttu-id="3576e-194">继承自 [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="3576e-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="3576e-195">bundleId</span><span class="sxs-lookup"><span data-stu-id="3576e-195">bundleId</span></span>|<span data-ttu-id="3576e-196">字符串</span><span class="sxs-lookup"><span data-stu-id="3576e-196">String</span></span>|<span data-ttu-id="3576e-197">应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="3576e-197">The app's Bundle ID.</span></span>|
|<span data-ttu-id="3576e-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="3576e-198">appStoreUrl</span></span>|<span data-ttu-id="3576e-199">字符串</span><span class="sxs-lookup"><span data-stu-id="3576e-199">String</span></span>|<span data-ttu-id="3576e-200">Apple AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="3576e-200">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="3576e-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="3576e-201">applicableDeviceType</span></span>|[<span data-ttu-id="3576e-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="3576e-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="3576e-203">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="3576e-203">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="3576e-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3576e-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3576e-205">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3576e-205">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="3576e-206">最低受支持操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="3576e-206">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="3576e-207">响应</span><span class="sxs-lookup"><span data-stu-id="3576e-207">Response</span></span>
<span data-ttu-id="3576e-208">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3576e-208">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3576e-209">示例</span><span class="sxs-lookup"><span data-stu-id="3576e-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="3576e-210">请求</span><span class="sxs-lookup"><span data-stu-id="3576e-210">Request</span></span>
<span data-ttu-id="3576e-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3576e-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1128

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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
    "v11_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="3576e-212">响应</span><span class="sxs-lookup"><span data-stu-id="3576e-212">Response</span></span>
<span data-ttu-id="3576e-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3576e-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1236

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
    "v11_0": true
  }
}
```



