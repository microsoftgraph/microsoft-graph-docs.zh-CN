# <a name="create-webapp"></a><span data-ttu-id="1d545-101">创建 webApp</span><span class="sxs-lookup"><span data-stu-id="1d545-101">Create webApp</span></span>

> <span data-ttu-id="1d545-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1d545-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d545-103">创建新的 [webApp](../resources/intune_apps_webapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1d545-103">Create a new [plannerBucket](../resources/intune_apps_webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d545-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="1d545-104">Prerequisites</span></span>
<span data-ttu-id="1d545-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1d545-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1d545-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d545-107">Permission type</span></span>|<span data-ttu-id="1d545-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1d545-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d545-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d545-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1d545-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d545-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1d545-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d545-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d545-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d545-112">Not supported.</span></span>|
|<span data-ttu-id="1d545-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d545-113">Application</span></span>|<span data-ttu-id="1d545-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d545-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d545-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d545-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1d545-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d545-116">Request headers</span></span>
|<span data-ttu-id="1d545-117">标头</span><span class="sxs-lookup"><span data-stu-id="1d545-117">Header</span></span>|<span data-ttu-id="1d545-118">值</span><span class="sxs-lookup"><span data-stu-id="1d545-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d545-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d545-119">Authorization</span></span>|<span data-ttu-id="1d545-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1d545-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1d545-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1d545-121">Accept</span></span>|<span data-ttu-id="1d545-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1d545-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d545-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d545-123">Request body</span></span>
<span data-ttu-id="1d545-124">在请求正文中，提供 webApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d545-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="1d545-125">下表显示创建 webApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1d545-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="1d545-126">属性</span><span class="sxs-lookup"><span data-stu-id="1d545-126">Property</span></span>|<span data-ttu-id="1d545-127">类型</span><span class="sxs-lookup"><span data-stu-id="1d545-127">Type</span></span>|<span data-ttu-id="1d545-128">说明</span><span class="sxs-lookup"><span data-stu-id="1d545-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d545-129">id</span><span class="sxs-lookup"><span data-stu-id="1d545-129">id</span></span>|<span data-ttu-id="1d545-130">String</span><span class="sxs-lookup"><span data-stu-id="1d545-130">String</span></span>|<span data-ttu-id="1d545-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1d545-131">Key of the setting.</span></span> <span data-ttu-id="1d545-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d545-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1d545-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1d545-133">displayName</span></span>|<span data-ttu-id="1d545-134">String</span><span class="sxs-lookup"><span data-stu-id="1d545-134">String</span></span>|<span data-ttu-id="1d545-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="1d545-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1d545-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d545-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1d545-137">description</span><span class="sxs-lookup"><span data-stu-id="1d545-137">description</span></span>|<span data-ttu-id="1d545-138">String</span><span class="sxs-lookup"><span data-stu-id="1d545-138">String</span></span>|<span data-ttu-id="1d545-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="1d545-139">The description of the app.</span></span> <span data-ttu-id="1d545-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d545-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1d545-141">publisher</span><span class="sxs-lookup"><span data-stu-id="1d545-141">Publisher</span></span>|<span data-ttu-id="1d545-142">String</span><span class="sxs-lookup"><span data-stu-id="1d545-142">String</span></span>|<span data-ttu-id="1d545-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="1d545-143">The name of the app.</span></span> <span data-ttu-id="1d545-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d545-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1d545-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1d545-145">largeIcon</span></span>|[<span data-ttu-id="1d545-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1d545-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="1d545-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="1d545-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1d545-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d545-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1d545-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d545-149">createdDateTime</span></span>|<span data-ttu-id="1d545-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d545-150">DateTimeOffset</span></span>|<span data-ttu-id="1d545-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1d545-151">The date and time when the page was created.</span></span> <span data-ttu-id="1d545-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d545-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1d545-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d545-153">lastModifiedDateTime</span></span>|<span data-ttu-id="1d545-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d545-154">DateTimeOffset</span></span>|<span data-ttu-id="1d545-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1d545-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="1d545-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d545-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1d545-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1d545-157">isFeatured</span></span>|<span data-ttu-id="1d545-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d545-158">Boolean</span></span>|<span data-ttu-id="1d545-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d545-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1d545-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1d545-160">privacyInformationUrl</span></span>|<span data-ttu-id="1d545-161">String</span><span class="sxs-lookup"><span data-stu-id="1d545-161">String</span></span>|<span data-ttu-id="1d545-162">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="1d545-162">The privacy statement Url.</span></span> <span data-ttu-id="1d545-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d545-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1d545-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1d545-164">informationUrl</span></span>|<span data-ttu-id="1d545-165">String</span><span class="sxs-lookup"><span data-stu-id="1d545-165">String</span></span>|<span data-ttu-id="1d545-166">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="1d545-166">The more information Url.</span></span> <span data-ttu-id="1d545-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d545-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1d545-168">owner</span><span class="sxs-lookup"><span data-stu-id="1d545-168">owner</span></span>|<span data-ttu-id="1d545-169">String</span><span class="sxs-lookup"><span data-stu-id="1d545-169">String</span></span>|<span data-ttu-id="1d545-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="1d545-170">The owner of the timesheet.</span></span> <span data-ttu-id="1d545-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d545-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1d545-172">developer</span><span class="sxs-lookup"><span data-stu-id="1d545-172">developer</span></span>|<span data-ttu-id="1d545-173">String</span><span class="sxs-lookup"><span data-stu-id="1d545-173">String</span></span>|<span data-ttu-id="1d545-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="1d545-174">The name of the app.</span></span> <span data-ttu-id="1d545-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d545-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1d545-176">notes</span><span class="sxs-lookup"><span data-stu-id="1d545-176">notes</span></span>|<span data-ttu-id="1d545-177">String</span><span class="sxs-lookup"><span data-stu-id="1d545-177">String</span></span>|<span data-ttu-id="1d545-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="1d545-178">Notes for the app.</span></span> <span data-ttu-id="1d545-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d545-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1d545-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="1d545-180">publishingState</span></span>|<span data-ttu-id="1d545-181">String</span><span class="sxs-lookup"><span data-stu-id="1d545-181">String</span></span>|<span data-ttu-id="1d545-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="1d545-182">The publishing state for the app.</span></span> <span data-ttu-id="1d545-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="1d545-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1d545-184">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="1d545-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1d545-185">appUrl</span><span class="sxs-lookup"><span data-stu-id="1d545-185">appUrl</span></span>|<span data-ttu-id="1d545-186">String</span><span class="sxs-lookup"><span data-stu-id="1d545-186">String</span></span>|<span data-ttu-id="1d545-187">Web 应用 URL。</span><span class="sxs-lookup"><span data-stu-id="1d545-187">The web app URL.</span></span>|
|<span data-ttu-id="1d545-188">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="1d545-188">useManagedBrowser</span></span>|<span data-ttu-id="1d545-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d545-189">Boolean</span></span>|<span data-ttu-id="1d545-190">是否使用托管浏览器。</span><span class="sxs-lookup"><span data-stu-id="1d545-190">Whether or not to use managed browser.</span></span> <span data-ttu-id="1d545-191">此属性仅适用于 Android 和 iOS。</span><span class="sxs-lookup"><span data-stu-id="1d545-191">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="1d545-192">响应</span><span class="sxs-lookup"><span data-stu-id="1d545-192">Response</span></span>
<span data-ttu-id="1d545-193">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [webApp](../resources/intune_apps_webapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1d545-193">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_apps_webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d545-194">示例</span><span class="sxs-lookup"><span data-stu-id="1d545-194">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d545-195">请求</span><span class="sxs-lookup"><span data-stu-id="1d545-195">Request</span></span>
<span data-ttu-id="1d545-196">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1d545-196">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 709

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="1d545-197">响应</span><span class="sxs-lookup"><span data-stu-id="1d545-197">Response</span></span>
<span data-ttu-id="1d545-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1d545-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 817

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```



