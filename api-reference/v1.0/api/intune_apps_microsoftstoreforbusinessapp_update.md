# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="6010b-101">更新 microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="6010b-101">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="6010b-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6010b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6010b-103">更新 [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6010b-103">Update the properties of a [calendar](../resources/intune_apps_microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6010b-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="6010b-104">Prerequisites</span></span>
<span data-ttu-id="6010b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6010b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6010b-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="6010b-107">Permission type</span></span>|<span data-ttu-id="6010b-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6010b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6010b-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6010b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6010b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6010b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6010b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6010b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6010b-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="6010b-112">Not supported.</span></span>|
|<span data-ttu-id="6010b-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="6010b-113">Application</span></span>|<span data-ttu-id="6010b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6010b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6010b-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6010b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="6010b-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="6010b-116">Request headers</span></span>
|<span data-ttu-id="6010b-117">标头</span><span class="sxs-lookup"><span data-stu-id="6010b-117">Header</span></span>|<span data-ttu-id="6010b-118">值</span><span class="sxs-lookup"><span data-stu-id="6010b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6010b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="6010b-119">Authorization</span></span>|<span data-ttu-id="6010b-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6010b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6010b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="6010b-121">Accept</span></span>|<span data-ttu-id="6010b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6010b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6010b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6010b-123">Request body</span></span>
<span data-ttu-id="6010b-124">在请求正文中，提供 [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6010b-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="6010b-125">下表显示了创建 [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6010b-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="6010b-126">属性</span><span class="sxs-lookup"><span data-stu-id="6010b-126">Property</span></span>|<span data-ttu-id="6010b-127">类型</span><span class="sxs-lookup"><span data-stu-id="6010b-127">Type</span></span>|<span data-ttu-id="6010b-128">说明</span><span class="sxs-lookup"><span data-stu-id="6010b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6010b-129">id</span><span class="sxs-lookup"><span data-stu-id="6010b-129">id</span></span>|<span data-ttu-id="6010b-130">String</span><span class="sxs-lookup"><span data-stu-id="6010b-130">String</span></span>|<span data-ttu-id="6010b-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6010b-131">Key of the setting.</span></span> <span data-ttu-id="6010b-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6010b-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6010b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6010b-133">displayName</span></span>|<span data-ttu-id="6010b-134">String</span><span class="sxs-lookup"><span data-stu-id="6010b-134">String</span></span>|<span data-ttu-id="6010b-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="6010b-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6010b-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6010b-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6010b-137">description</span><span class="sxs-lookup"><span data-stu-id="6010b-137">description</span></span>|<span data-ttu-id="6010b-138">String</span><span class="sxs-lookup"><span data-stu-id="6010b-138">String</span></span>|<span data-ttu-id="6010b-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="6010b-139">The description of the app.</span></span> <span data-ttu-id="6010b-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6010b-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6010b-141">publisher</span><span class="sxs-lookup"><span data-stu-id="6010b-141">Publisher</span></span>|<span data-ttu-id="6010b-142">String</span><span class="sxs-lookup"><span data-stu-id="6010b-142">String</span></span>|<span data-ttu-id="6010b-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="6010b-143">The name of the app.</span></span> <span data-ttu-id="6010b-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6010b-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6010b-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6010b-145">largeIcon</span></span>|[<span data-ttu-id="6010b-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6010b-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="6010b-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="6010b-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6010b-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6010b-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6010b-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6010b-149">createdDateTime</span></span>|<span data-ttu-id="6010b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6010b-150">DateTimeOffset</span></span>|<span data-ttu-id="6010b-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6010b-151">The date and time when the page was created.</span></span> <span data-ttu-id="6010b-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6010b-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6010b-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6010b-153">lastModifiedDateTime</span></span>|<span data-ttu-id="6010b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6010b-154">DateTimeOffset</span></span>|<span data-ttu-id="6010b-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6010b-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="6010b-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6010b-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6010b-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6010b-157">isFeatured</span></span>|<span data-ttu-id="6010b-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="6010b-158">Boolean</span></span>|<span data-ttu-id="6010b-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6010b-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6010b-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6010b-160">privacyInformationUrl</span></span>|<span data-ttu-id="6010b-161">String</span><span class="sxs-lookup"><span data-stu-id="6010b-161">String</span></span>|<span data-ttu-id="6010b-162">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="6010b-162">The privacy statement Url.</span></span> <span data-ttu-id="6010b-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6010b-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6010b-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6010b-164">informationUrl</span></span>|<span data-ttu-id="6010b-165">String</span><span class="sxs-lookup"><span data-stu-id="6010b-165">String</span></span>|<span data-ttu-id="6010b-166">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="6010b-166">The more information Url.</span></span> <span data-ttu-id="6010b-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6010b-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6010b-168">owner</span><span class="sxs-lookup"><span data-stu-id="6010b-168">owner</span></span>|<span data-ttu-id="6010b-169">String</span><span class="sxs-lookup"><span data-stu-id="6010b-169">String</span></span>|<span data-ttu-id="6010b-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="6010b-170">The owner of the timesheet.</span></span> <span data-ttu-id="6010b-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6010b-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6010b-172">developer</span><span class="sxs-lookup"><span data-stu-id="6010b-172">developer</span></span>|<span data-ttu-id="6010b-173">String</span><span class="sxs-lookup"><span data-stu-id="6010b-173">String</span></span>|<span data-ttu-id="6010b-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="6010b-174">The name of the app.</span></span> <span data-ttu-id="6010b-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6010b-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6010b-176">notes</span><span class="sxs-lookup"><span data-stu-id="6010b-176">notes</span></span>|<span data-ttu-id="6010b-177">String</span><span class="sxs-lookup"><span data-stu-id="6010b-177">String</span></span>|<span data-ttu-id="6010b-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="6010b-178">Notes for the app.</span></span> <span data-ttu-id="6010b-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6010b-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6010b-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="6010b-180">publishingState</span></span>|<span data-ttu-id="6010b-181">String</span><span class="sxs-lookup"><span data-stu-id="6010b-181">String</span></span>|<span data-ttu-id="6010b-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="6010b-182">The publishing state for the app.</span></span> <span data-ttu-id="6010b-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="6010b-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6010b-184">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="6010b-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6010b-185">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6010b-185">usedLicenseCount</span></span>|<span data-ttu-id="6010b-186">Int32</span><span class="sxs-lookup"><span data-stu-id="6010b-186">Int32</span></span>|<span data-ttu-id="6010b-187">使用中的适用于企业的 Microsoft Store 许可证数。</span><span class="sxs-lookup"><span data-stu-id="6010b-187">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="6010b-188">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6010b-188">totalLicenseCount</span></span>|<span data-ttu-id="6010b-189">Int32</span><span class="sxs-lookup"><span data-stu-id="6010b-189">Int32</span></span>|<span data-ttu-id="6010b-190">适用于企业的 Microsoft Store 许可证总数。</span><span class="sxs-lookup"><span data-stu-id="6010b-190">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="6010b-191">productKey</span><span class="sxs-lookup"><span data-stu-id="6010b-191">productKey</span></span>|<span data-ttu-id="6010b-192">String</span><span class="sxs-lookup"><span data-stu-id="6010b-192">String</span></span>|<span data-ttu-id="6010b-193">应用产品密钥</span><span class="sxs-lookup"><span data-stu-id="6010b-193">The app product key</span></span>|
|<span data-ttu-id="6010b-194">licenseType</span><span class="sxs-lookup"><span data-stu-id="6010b-194">licenseType</span></span>|<span data-ttu-id="6010b-195">String</span><span class="sxs-lookup"><span data-stu-id="6010b-195">String</span></span>|<span data-ttu-id="6010b-196">应用许可证类型。可取值为：`offline`、`online`。</span><span class="sxs-lookup"><span data-stu-id="6010b-196">The app license type Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="6010b-197">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="6010b-197">packageIdentityName</span></span>|<span data-ttu-id="6010b-198">String</span><span class="sxs-lookup"><span data-stu-id="6010b-198">String</span></span>|<span data-ttu-id="6010b-199">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="6010b-199">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="6010b-200">响应</span><span class="sxs-lookup"><span data-stu-id="6010b-200">Response</span></span>
<span data-ttu-id="6010b-201">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6010b-201">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6010b-202">示例</span><span class="sxs-lookup"><span data-stu-id="6010b-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="6010b-203">请求</span><span class="sxs-lookup"><span data-stu-id="6010b-203">Request</span></span>
<span data-ttu-id="6010b-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6010b-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 766

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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="6010b-205">响应</span><span class="sxs-lookup"><span data-stu-id="6010b-205">Response</span></span>
<span data-ttu-id="6010b-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6010b-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



