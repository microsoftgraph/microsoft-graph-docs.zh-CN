# <a name="update-androidstoreapp"></a><span data-ttu-id="451d1-101">更新 androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="451d1-101">Update androidStoreApp</span></span>

> <span data-ttu-id="451d1-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="451d1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="451d1-103">更新 [androidStoreApp](../resources/intune_apps_androidstoreapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="451d1-103">Update the properties of a [calendar](../resources/intune_apps_androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="451d1-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="451d1-104">Prerequisites</span></span>
<span data-ttu-id="451d1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="451d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="451d1-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="451d1-107">Permission type</span></span>|<span data-ttu-id="451d1-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="451d1-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="451d1-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="451d1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="451d1-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="451d1-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="451d1-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="451d1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="451d1-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="451d1-112">Not supported.</span></span>|
|<span data-ttu-id="451d1-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="451d1-113">Application</span></span>|<span data-ttu-id="451d1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="451d1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="451d1-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="451d1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="451d1-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="451d1-116">Request headers</span></span>
|<span data-ttu-id="451d1-117">标头</span><span class="sxs-lookup"><span data-stu-id="451d1-117">Header</span></span>|<span data-ttu-id="451d1-118">值</span><span class="sxs-lookup"><span data-stu-id="451d1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="451d1-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="451d1-119">Authorization</span></span>|<span data-ttu-id="451d1-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="451d1-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="451d1-121">Accept</span><span class="sxs-lookup"><span data-stu-id="451d1-121">Accept</span></span>|<span data-ttu-id="451d1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="451d1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="451d1-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="451d1-123">Request body</span></span>
<span data-ttu-id="451d1-124">在请求正文中，提供 [androidStoreApp](../resources/intune_apps_androidstoreapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="451d1-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_androidstoreapp.md) object.</span></span>

<span data-ttu-id="451d1-125">下表显示了创建 [androidStoreApp](../resources/intune_apps_androidstoreapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="451d1-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="451d1-126">属性</span><span class="sxs-lookup"><span data-stu-id="451d1-126">Property</span></span>|<span data-ttu-id="451d1-127">类型</span><span class="sxs-lookup"><span data-stu-id="451d1-127">Type</span></span>|<span data-ttu-id="451d1-128">说明</span><span class="sxs-lookup"><span data-stu-id="451d1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="451d1-129">id</span><span class="sxs-lookup"><span data-stu-id="451d1-129">id</span></span>|<span data-ttu-id="451d1-130">String</span><span class="sxs-lookup"><span data-stu-id="451d1-130">String</span></span>|<span data-ttu-id="451d1-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="451d1-131">Key of the setting.</span></span> <span data-ttu-id="451d1-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="451d1-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="451d1-133">displayName</span><span class="sxs-lookup"><span data-stu-id="451d1-133">displayName</span></span>|<span data-ttu-id="451d1-134">String</span><span class="sxs-lookup"><span data-stu-id="451d1-134">String</span></span>|<span data-ttu-id="451d1-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="451d1-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="451d1-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="451d1-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="451d1-137">description</span><span class="sxs-lookup"><span data-stu-id="451d1-137">description</span></span>|<span data-ttu-id="451d1-138">String</span><span class="sxs-lookup"><span data-stu-id="451d1-138">String</span></span>|<span data-ttu-id="451d1-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="451d1-139">The description of the app.</span></span> <span data-ttu-id="451d1-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="451d1-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="451d1-141">publisher</span><span class="sxs-lookup"><span data-stu-id="451d1-141">Publisher</span></span>|<span data-ttu-id="451d1-142">String</span><span class="sxs-lookup"><span data-stu-id="451d1-142">String</span></span>|<span data-ttu-id="451d1-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="451d1-143">The name of the app.</span></span> <span data-ttu-id="451d1-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="451d1-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="451d1-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="451d1-145">largeIcon</span></span>|[<span data-ttu-id="451d1-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="451d1-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="451d1-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="451d1-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="451d1-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="451d1-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="451d1-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="451d1-149">createdDateTime</span></span>|<span data-ttu-id="451d1-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="451d1-150">DateTimeOffset</span></span>|<span data-ttu-id="451d1-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="451d1-151">The date and time when the page was created.</span></span> <span data-ttu-id="451d1-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="451d1-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="451d1-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="451d1-153">lastModifiedDateTime</span></span>|<span data-ttu-id="451d1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="451d1-154">DateTimeOffset</span></span>|<span data-ttu-id="451d1-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="451d1-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="451d1-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="451d1-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="451d1-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="451d1-157">isFeatured</span></span>|<span data-ttu-id="451d1-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="451d1-158">Boolean</span></span>|<span data-ttu-id="451d1-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="451d1-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="451d1-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="451d1-160">privacyInformationUrl</span></span>|<span data-ttu-id="451d1-161">String</span><span class="sxs-lookup"><span data-stu-id="451d1-161">String</span></span>|<span data-ttu-id="451d1-162">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="451d1-162">The privacy statement Url.</span></span> <span data-ttu-id="451d1-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="451d1-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="451d1-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="451d1-164">informationUrl</span></span>|<span data-ttu-id="451d1-165">String</span><span class="sxs-lookup"><span data-stu-id="451d1-165">String</span></span>|<span data-ttu-id="451d1-166">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="451d1-166">The more information Url.</span></span> <span data-ttu-id="451d1-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="451d1-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="451d1-168">owner</span><span class="sxs-lookup"><span data-stu-id="451d1-168">owner</span></span>|<span data-ttu-id="451d1-169">String</span><span class="sxs-lookup"><span data-stu-id="451d1-169">String</span></span>|<span data-ttu-id="451d1-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="451d1-170">The owner of the timesheet.</span></span> <span data-ttu-id="451d1-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="451d1-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="451d1-172">developer</span><span class="sxs-lookup"><span data-stu-id="451d1-172">developer</span></span>|<span data-ttu-id="451d1-173">String</span><span class="sxs-lookup"><span data-stu-id="451d1-173">String</span></span>|<span data-ttu-id="451d1-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="451d1-174">The name of the app.</span></span> <span data-ttu-id="451d1-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="451d1-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="451d1-176">notes</span><span class="sxs-lookup"><span data-stu-id="451d1-176">notes</span></span>|<span data-ttu-id="451d1-177">String</span><span class="sxs-lookup"><span data-stu-id="451d1-177">String</span></span>|<span data-ttu-id="451d1-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="451d1-178">Notes for the app.</span></span> <span data-ttu-id="451d1-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="451d1-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="451d1-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="451d1-180">publishingState</span></span>|<span data-ttu-id="451d1-181">String</span><span class="sxs-lookup"><span data-stu-id="451d1-181">String</span></span>|<span data-ttu-id="451d1-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="451d1-182">The publishing state for the app.</span></span> <span data-ttu-id="451d1-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="451d1-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="451d1-184">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="451d1-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="451d1-185">packageId</span><span class="sxs-lookup"><span data-stu-id="451d1-185">PackageId</span></span>|<span data-ttu-id="451d1-186">String</span><span class="sxs-lookup"><span data-stu-id="451d1-186">String</span></span>|<span data-ttu-id="451d1-187">包标识符。</span><span class="sxs-lookup"><span data-stu-id="451d1-187">The package identifier.</span></span>|
|<span data-ttu-id="451d1-188">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="451d1-188">appStoreUrl</span></span>|<span data-ttu-id="451d1-189">String</span><span class="sxs-lookup"><span data-stu-id="451d1-189">String</span></span>|<span data-ttu-id="451d1-190">Android 应用商店 URL。</span><span class="sxs-lookup"><span data-stu-id="451d1-190">The Android app store URL.</span></span>|
|<span data-ttu-id="451d1-191">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="451d1-191">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="451d1-192">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="451d1-192">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="451d1-193">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="451d1-193">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="451d1-194">响应</span><span class="sxs-lookup"><span data-stu-id="451d1-194">Response</span></span>
<span data-ttu-id="451d1-195">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidStoreApp](../resources/intune_apps_androidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="451d1-195">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="451d1-196">示例</span><span class="sxs-lookup"><span data-stu-id="451d1-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="451d1-197">请求</span><span class="sxs-lookup"><span data-stu-id="451d1-197">Request</span></span>
<span data-ttu-id="451d1-198">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="451d1-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="451d1-199">响应</span><span class="sxs-lookup"><span data-stu-id="451d1-199">Response</span></span>
<span data-ttu-id="451d1-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="451d1-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



