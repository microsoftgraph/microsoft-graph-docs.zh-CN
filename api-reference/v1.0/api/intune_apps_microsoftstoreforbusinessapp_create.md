# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="f2fb2-101">创建 microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="f2fb2-101">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="f2fb2-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2fb2-103">创建新的 [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-103">Create a new [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f2fb2-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="f2fb2-104">Prerequisites</span></span>
<span data-ttu-id="f2fb2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f2fb2-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2fb2-107">Permission type</span></span>|<span data-ttu-id="f2fb2-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f2fb2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2fb2-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2fb2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f2fb2-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2fb2-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f2fb2-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2fb2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2fb2-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-112">Not supported.</span></span>|
|<span data-ttu-id="f2fb2-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2fb2-113">Application</span></span>|<span data-ttu-id="f2fb2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2fb2-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2fb2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f2fb2-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2fb2-116">Request headers</span></span>
|<span data-ttu-id="f2fb2-117">标头</span><span class="sxs-lookup"><span data-stu-id="f2fb2-117">Header</span></span>|<span data-ttu-id="f2fb2-118">值</span><span class="sxs-lookup"><span data-stu-id="f2fb2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2fb2-119">授权</span><span class="sxs-lookup"><span data-stu-id="f2fb2-119">Authorization</span></span>|<span data-ttu-id="f2fb2-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2fb2-121">接受</span><span class="sxs-lookup"><span data-stu-id="f2fb2-121">Accept</span></span>|<span data-ttu-id="f2fb2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f2fb2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2fb2-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2fb2-123">Request body</span></span>
<span data-ttu-id="f2fb2-124">在请求正文中，提供 microsoftStoreForBusinessApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-124">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="f2fb2-125">下表显示了创建 microsoftStoreForBusinessApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-125">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="f2fb2-126">属性</span><span class="sxs-lookup"><span data-stu-id="f2fb2-126">Property</span></span>|<span data-ttu-id="f2fb2-127">类型</span><span class="sxs-lookup"><span data-stu-id="f2fb2-127">Type</span></span>|<span data-ttu-id="f2fb2-128">说明</span><span class="sxs-lookup"><span data-stu-id="f2fb2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2fb2-129">ID</span><span class="sxs-lookup"><span data-stu-id="f2fb2-129">id</span></span>|<span data-ttu-id="f2fb2-130">字符串</span><span class="sxs-lookup"><span data-stu-id="f2fb2-130">String</span></span>|<span data-ttu-id="f2fb2-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-131">Key of the entity.</span></span> <span data-ttu-id="f2fb2-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2fb2-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f2fb2-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f2fb2-133">displayName</span></span>|<span data-ttu-id="f2fb2-134">字符串</span><span class="sxs-lookup"><span data-stu-id="f2fb2-134">String</span></span>|<span data-ttu-id="f2fb2-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f2fb2-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2fb2-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f2fb2-137">说明</span><span class="sxs-lookup"><span data-stu-id="f2fb2-137">description</span></span>|<span data-ttu-id="f2fb2-138">字符串</span><span class="sxs-lookup"><span data-stu-id="f2fb2-138">String</span></span>|<span data-ttu-id="f2fb2-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-139">The description of the app.</span></span> <span data-ttu-id="f2fb2-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2fb2-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f2fb2-141">publisher</span><span class="sxs-lookup"><span data-stu-id="f2fb2-141">publisher</span></span>|<span data-ttu-id="f2fb2-142">字符串</span><span class="sxs-lookup"><span data-stu-id="f2fb2-142">String</span></span>|<span data-ttu-id="f2fb2-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-143">The publisher of the app.</span></span> <span data-ttu-id="f2fb2-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2fb2-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f2fb2-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f2fb2-145">largeIcon</span></span>|[<span data-ttu-id="f2fb2-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f2fb2-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="f2fb2-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f2fb2-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2fb2-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f2fb2-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2fb2-149">createdDateTime</span></span>|<span data-ttu-id="f2fb2-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2fb2-150">DateTimeOffset</span></span>|<span data-ttu-id="f2fb2-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-151">The date and time the app was created.</span></span> <span data-ttu-id="f2fb2-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2fb2-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f2fb2-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2fb2-153">lastModifiedDateTime</span></span>|<span data-ttu-id="f2fb2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2fb2-154">DateTimeOffset</span></span>|<span data-ttu-id="f2fb2-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-155">The date and time the app was last modified.</span></span> <span data-ttu-id="f2fb2-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2fb2-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f2fb2-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f2fb2-157">isFeatured</span></span>|<span data-ttu-id="f2fb2-158">布尔</span><span class="sxs-lookup"><span data-stu-id="f2fb2-158">Boolean</span></span>|<span data-ttu-id="f2fb2-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2fb2-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f2fb2-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f2fb2-160">privacyInformationUrl</span></span>|<span data-ttu-id="f2fb2-161">字符串</span><span class="sxs-lookup"><span data-stu-id="f2fb2-161">String</span></span>|<span data-ttu-id="f2fb2-162">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-162">The privacy statement Url.</span></span> <span data-ttu-id="f2fb2-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2fb2-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f2fb2-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f2fb2-164">informationUrl</span></span>|<span data-ttu-id="f2fb2-165">字符串</span><span class="sxs-lookup"><span data-stu-id="f2fb2-165">String</span></span>|<span data-ttu-id="f2fb2-166">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-166">The more information Url.</span></span> <span data-ttu-id="f2fb2-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2fb2-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f2fb2-168">owner</span><span class="sxs-lookup"><span data-stu-id="f2fb2-168">owner</span></span>|<span data-ttu-id="f2fb2-169">字符串</span><span class="sxs-lookup"><span data-stu-id="f2fb2-169">String</span></span>|<span data-ttu-id="f2fb2-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-170">The owner of the app.</span></span> <span data-ttu-id="f2fb2-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2fb2-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f2fb2-172">developer</span><span class="sxs-lookup"><span data-stu-id="f2fb2-172">developer</span></span>|<span data-ttu-id="f2fb2-173">字符串</span><span class="sxs-lookup"><span data-stu-id="f2fb2-173">String</span></span>|<span data-ttu-id="f2fb2-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-174">The developer of the app.</span></span> <span data-ttu-id="f2fb2-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2fb2-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f2fb2-176">注释</span><span class="sxs-lookup"><span data-stu-id="f2fb2-176">notes</span></span>|<span data-ttu-id="f2fb2-177">字符串</span><span class="sxs-lookup"><span data-stu-id="f2fb2-177">String</span></span>|<span data-ttu-id="f2fb2-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-178">Notes for the app.</span></span> <span data-ttu-id="f2fb2-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2fb2-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f2fb2-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="f2fb2-180">publishingState</span></span>|[<span data-ttu-id="f2fb2-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f2fb2-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="f2fb2-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-182">The publishing state for the app.</span></span> <span data-ttu-id="f2fb2-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f2fb2-184">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="f2fb2-185">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f2fb2-186">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f2fb2-186">usedLicenseCount</span></span>|<span data-ttu-id="f2fb2-187">Int32</span><span class="sxs-lookup"><span data-stu-id="f2fb2-187">Int32</span></span>|<span data-ttu-id="f2fb2-188">使用中的适用于企业的 Microsoft Store 许可证数。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-188">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="f2fb2-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f2fb2-189">totalLicenseCount</span></span>|<span data-ttu-id="f2fb2-190">Int32</span><span class="sxs-lookup"><span data-stu-id="f2fb2-190">Int32</span></span>|<span data-ttu-id="f2fb2-191">适用于企业的 Microsoft Store 许可证总数。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-191">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="f2fb2-192">productKey</span><span class="sxs-lookup"><span data-stu-id="f2fb2-192">productKey</span></span>|<span data-ttu-id="f2fb2-193">字符串</span><span class="sxs-lookup"><span data-stu-id="f2fb2-193">String</span></span>|<span data-ttu-id="f2fb2-194">应用产品密钥</span><span class="sxs-lookup"><span data-stu-id="f2fb2-194">The app product key</span></span>|
|<span data-ttu-id="f2fb2-195">licenseType</span><span class="sxs-lookup"><span data-stu-id="f2fb2-195">licenseType</span></span>|[<span data-ttu-id="f2fb2-196">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="f2fb2-196">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune_apps_microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="f2fb2-197">应用许可证类型。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-197">The app license type Possible values are: , .</span></span> <span data-ttu-id="f2fb2-198">可取值为：`offline`、`online`。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-198">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="f2fb2-199">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="f2fb2-199">packageIdentityName</span></span>|<span data-ttu-id="f2fb2-200">字符串</span><span class="sxs-lookup"><span data-stu-id="f2fb2-200">String</span></span>|<span data-ttu-id="f2fb2-201">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="f2fb2-201">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="f2fb2-202">响应</span><span class="sxs-lookup"><span data-stu-id="f2fb2-202">Response</span></span>
<span data-ttu-id="f2fb2-203">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-203">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2fb2-204">示例</span><span class="sxs-lookup"><span data-stu-id="f2fb2-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="f2fb2-205">请求</span><span class="sxs-lookup"><span data-stu-id="f2fb2-205">Request</span></span>
<span data-ttu-id="f2fb2-206">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 833

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="f2fb2-207">响应</span><span class="sxs-lookup"><span data-stu-id="f2fb2-207">Response</span></span>
<span data-ttu-id="f2fb2-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 941

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```








