# <a name="create-androidstoreapp"></a><span data-ttu-id="851d7-101">创建 androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="851d7-101">Create androidStoreApp</span></span>

> <span data-ttu-id="851d7-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="851d7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="851d7-103">创建新的 [androidStoreApp](../resources/intune_apps_androidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="851d7-103">Create a new [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="851d7-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="851d7-104">Prerequisites</span></span>
<span data-ttu-id="851d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="851d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="851d7-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="851d7-107">Permission type</span></span>|<span data-ttu-id="851d7-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="851d7-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="851d7-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="851d7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="851d7-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="851d7-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="851d7-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="851d7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="851d7-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="851d7-112">Not supported.</span></span>|
|<span data-ttu-id="851d7-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="851d7-113">Application</span></span>|<span data-ttu-id="851d7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="851d7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="851d7-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="851d7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="851d7-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="851d7-116">Request headers</span></span>
|<span data-ttu-id="851d7-117">标头</span><span class="sxs-lookup"><span data-stu-id="851d7-117">Header</span></span>|<span data-ttu-id="851d7-118">值</span><span class="sxs-lookup"><span data-stu-id="851d7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="851d7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="851d7-119">Authorization</span></span>|<span data-ttu-id="851d7-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="851d7-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="851d7-121">Accept</span><span class="sxs-lookup"><span data-stu-id="851d7-121">Accept</span></span>|<span data-ttu-id="851d7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="851d7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="851d7-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="851d7-123">Request body</span></span>
<span data-ttu-id="851d7-124">在请求正文中，提供 androidStoreApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="851d7-124">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="851d7-125">下表显示创建 androidStoreApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="851d7-125">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="851d7-126">属性</span><span class="sxs-lookup"><span data-stu-id="851d7-126">Property</span></span>|<span data-ttu-id="851d7-127">类型</span><span class="sxs-lookup"><span data-stu-id="851d7-127">Type</span></span>|<span data-ttu-id="851d7-128">说明</span><span class="sxs-lookup"><span data-stu-id="851d7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="851d7-129">id</span><span class="sxs-lookup"><span data-stu-id="851d7-129">id</span></span>|<span data-ttu-id="851d7-130">String</span><span class="sxs-lookup"><span data-stu-id="851d7-130">String</span></span>|<span data-ttu-id="851d7-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="851d7-131">Key of the entity.</span></span> <span data-ttu-id="851d7-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="851d7-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="851d7-133">displayName</span><span class="sxs-lookup"><span data-stu-id="851d7-133">displayName</span></span>|<span data-ttu-id="851d7-134">String</span><span class="sxs-lookup"><span data-stu-id="851d7-134">String</span></span>|<span data-ttu-id="851d7-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="851d7-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="851d7-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="851d7-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="851d7-137">description</span><span class="sxs-lookup"><span data-stu-id="851d7-137">description</span></span>|<span data-ttu-id="851d7-138">String</span><span class="sxs-lookup"><span data-stu-id="851d7-138">String</span></span>|<span data-ttu-id="851d7-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="851d7-139">The description of the app.</span></span> <span data-ttu-id="851d7-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="851d7-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="851d7-141">publisher</span><span class="sxs-lookup"><span data-stu-id="851d7-141">publisher</span></span>|<span data-ttu-id="851d7-142">String</span><span class="sxs-lookup"><span data-stu-id="851d7-142">String</span></span>|<span data-ttu-id="851d7-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="851d7-143">The publisher of the app.</span></span> <span data-ttu-id="851d7-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="851d7-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="851d7-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="851d7-145">largeIcon</span></span>|[<span data-ttu-id="851d7-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="851d7-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="851d7-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="851d7-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="851d7-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="851d7-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="851d7-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="851d7-149">createdDateTime</span></span>|<span data-ttu-id="851d7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="851d7-150">DateTimeOffset</span></span>|<span data-ttu-id="851d7-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="851d7-151">The date and time the app was created.</span></span> <span data-ttu-id="851d7-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="851d7-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="851d7-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="851d7-153">lastModifiedDateTime</span></span>|<span data-ttu-id="851d7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="851d7-154">DateTimeOffset</span></span>|<span data-ttu-id="851d7-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="851d7-155">The date and time the app was last modified.</span></span> <span data-ttu-id="851d7-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="851d7-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="851d7-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="851d7-157">isFeatured</span></span>|<span data-ttu-id="851d7-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="851d7-158">Boolean</span></span>|<span data-ttu-id="851d7-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="851d7-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="851d7-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="851d7-160">privacyInformationUrl</span></span>|<span data-ttu-id="851d7-161">String</span><span class="sxs-lookup"><span data-stu-id="851d7-161">String</span></span>|<span data-ttu-id="851d7-162">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="851d7-162">The privacy statement Url.</span></span> <span data-ttu-id="851d7-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="851d7-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="851d7-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="851d7-164">informationUrl</span></span>|<span data-ttu-id="851d7-165">String</span><span class="sxs-lookup"><span data-stu-id="851d7-165">String</span></span>|<span data-ttu-id="851d7-166">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="851d7-166">The more information Url.</span></span> <span data-ttu-id="851d7-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="851d7-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="851d7-168">owner</span><span class="sxs-lookup"><span data-stu-id="851d7-168">owner</span></span>|<span data-ttu-id="851d7-169">String</span><span class="sxs-lookup"><span data-stu-id="851d7-169">String</span></span>|<span data-ttu-id="851d7-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="851d7-170">The owner of the app.</span></span> <span data-ttu-id="851d7-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="851d7-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="851d7-172">developer</span><span class="sxs-lookup"><span data-stu-id="851d7-172">developer</span></span>|<span data-ttu-id="851d7-173">String</span><span class="sxs-lookup"><span data-stu-id="851d7-173">String</span></span>|<span data-ttu-id="851d7-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="851d7-174">The developer of the app.</span></span> <span data-ttu-id="851d7-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="851d7-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="851d7-176">notes</span><span class="sxs-lookup"><span data-stu-id="851d7-176">notes</span></span>|<span data-ttu-id="851d7-177">String</span><span class="sxs-lookup"><span data-stu-id="851d7-177">String</span></span>|<span data-ttu-id="851d7-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="851d7-178">Notes for the app.</span></span> <span data-ttu-id="851d7-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="851d7-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="851d7-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="851d7-180">publishingState</span></span>|[<span data-ttu-id="851d7-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="851d7-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="851d7-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="851d7-182">The publishing state for the app.</span></span> <span data-ttu-id="851d7-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="851d7-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="851d7-184">继承自[mobileApp](../resources/intune_apps_mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="851d7-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="851d7-185">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="851d7-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="851d7-186">packageId</span><span class="sxs-lookup"><span data-stu-id="851d7-186">packageId</span></span>|<span data-ttu-id="851d7-187">String</span><span class="sxs-lookup"><span data-stu-id="851d7-187">String</span></span>|<span data-ttu-id="851d7-188">包标识符。</span><span class="sxs-lookup"><span data-stu-id="851d7-188">The package identifier.</span></span>|
|<span data-ttu-id="851d7-189">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="851d7-189">appStoreUrl</span></span>|<span data-ttu-id="851d7-190">String</span><span class="sxs-lookup"><span data-stu-id="851d7-190">String</span></span>|<span data-ttu-id="851d7-191">Android 应用商店 URL。</span><span class="sxs-lookup"><span data-stu-id="851d7-191">The Android app store URL.</span></span>|
|<span data-ttu-id="851d7-192">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="851d7-192">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="851d7-193">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="851d7-193">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="851d7-194">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="851d7-194">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="851d7-195">响应</span><span class="sxs-lookup"><span data-stu-id="851d7-195">Response</span></span>
<span data-ttu-id="851d7-196">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [androidStoreApp](../resources/intune_apps_androidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="851d7-196">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="851d7-197">示例</span><span class="sxs-lookup"><span data-stu-id="851d7-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="851d7-198">请求</span><span class="sxs-lookup"><span data-stu-id="851d7-198">Request</span></span>
<span data-ttu-id="851d7-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="851d7-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="851d7-200">响应</span><span class="sxs-lookup"><span data-stu-id="851d7-200">Response</span></span>
<span data-ttu-id="851d7-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="851d7-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



