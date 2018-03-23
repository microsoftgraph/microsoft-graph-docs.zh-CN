# <a name="update-windowsmobilemsi"></a><span data-ttu-id="cff48-101">更新 windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="cff48-101">Update windowsMobileMSI</span></span>

> <span data-ttu-id="cff48-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cff48-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cff48-103">更新 [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cff48-103">Update the properties of a [calendar](../resources/intune_apps_windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cff48-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="cff48-104">Prerequisites</span></span>
<span data-ttu-id="cff48-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cff48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cff48-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="cff48-107">Permission type</span></span>|<span data-ttu-id="cff48-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cff48-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cff48-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cff48-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cff48-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cff48-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cff48-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cff48-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cff48-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="cff48-112">Not supported.</span></span>|
|<span data-ttu-id="cff48-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="cff48-113">Application</span></span>|<span data-ttu-id="cff48-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cff48-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cff48-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cff48-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="cff48-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="cff48-116">Request headers</span></span>
|<span data-ttu-id="cff48-117">标头</span><span class="sxs-lookup"><span data-stu-id="cff48-117">Header</span></span>|<span data-ttu-id="cff48-118">值</span><span class="sxs-lookup"><span data-stu-id="cff48-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cff48-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="cff48-119">Authorization</span></span>|<span data-ttu-id="cff48-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cff48-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cff48-121">Accept</span><span class="sxs-lookup"><span data-stu-id="cff48-121">Accept</span></span>|<span data-ttu-id="cff48-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cff48-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cff48-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="cff48-123">Request body</span></span>
<span data-ttu-id="cff48-124">在请求正文中，提供 [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cff48-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="cff48-125">下表显示创建 [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cff48-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="cff48-126">属性</span><span class="sxs-lookup"><span data-stu-id="cff48-126">Property</span></span>|<span data-ttu-id="cff48-127">类型</span><span class="sxs-lookup"><span data-stu-id="cff48-127">Type</span></span>|<span data-ttu-id="cff48-128">说明</span><span class="sxs-lookup"><span data-stu-id="cff48-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cff48-129">id</span><span class="sxs-lookup"><span data-stu-id="cff48-129">id</span></span>|<span data-ttu-id="cff48-130">String</span><span class="sxs-lookup"><span data-stu-id="cff48-130">String</span></span>|<span data-ttu-id="cff48-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cff48-131">Key of the setting.</span></span> <span data-ttu-id="cff48-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cff48-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cff48-133">displayName</span><span class="sxs-lookup"><span data-stu-id="cff48-133">displayName</span></span>|<span data-ttu-id="cff48-134">String</span><span class="sxs-lookup"><span data-stu-id="cff48-134">String</span></span>|<span data-ttu-id="cff48-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="cff48-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cff48-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cff48-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cff48-137">description</span><span class="sxs-lookup"><span data-stu-id="cff48-137">description</span></span>|<span data-ttu-id="cff48-138">String</span><span class="sxs-lookup"><span data-stu-id="cff48-138">String</span></span>|<span data-ttu-id="cff48-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="cff48-139">The description of the app.</span></span> <span data-ttu-id="cff48-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cff48-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cff48-141">publisher</span><span class="sxs-lookup"><span data-stu-id="cff48-141">Publisher</span></span>|<span data-ttu-id="cff48-142">String</span><span class="sxs-lookup"><span data-stu-id="cff48-142">String</span></span>|<span data-ttu-id="cff48-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="cff48-143">The name of the app.</span></span> <span data-ttu-id="cff48-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cff48-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cff48-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cff48-145">largeIcon</span></span>|[<span data-ttu-id="cff48-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cff48-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="cff48-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="cff48-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cff48-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cff48-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cff48-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cff48-149">createdDateTime</span></span>|<span data-ttu-id="cff48-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cff48-150">DateTimeOffset</span></span>|<span data-ttu-id="cff48-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cff48-151">The date and time when the page was created.</span></span> <span data-ttu-id="cff48-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cff48-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cff48-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cff48-153">lastModifiedDateTime</span></span>|<span data-ttu-id="cff48-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cff48-154">DateTimeOffset</span></span>|<span data-ttu-id="cff48-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cff48-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="cff48-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cff48-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cff48-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cff48-157">isFeatured</span></span>|<span data-ttu-id="cff48-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="cff48-158">Boolean</span></span>|<span data-ttu-id="cff48-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cff48-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cff48-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cff48-160">privacyInformationUrl</span></span>|<span data-ttu-id="cff48-161">String</span><span class="sxs-lookup"><span data-stu-id="cff48-161">String</span></span>|<span data-ttu-id="cff48-162">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="cff48-162">The privacy statement Url.</span></span> <span data-ttu-id="cff48-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cff48-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cff48-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cff48-164">informationUrl</span></span>|<span data-ttu-id="cff48-165">String</span><span class="sxs-lookup"><span data-stu-id="cff48-165">String</span></span>|<span data-ttu-id="cff48-166">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="cff48-166">The more information Url.</span></span> <span data-ttu-id="cff48-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cff48-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cff48-168">owner</span><span class="sxs-lookup"><span data-stu-id="cff48-168">owner</span></span>|<span data-ttu-id="cff48-169">String</span><span class="sxs-lookup"><span data-stu-id="cff48-169">String</span></span>|<span data-ttu-id="cff48-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="cff48-170">The owner of the timesheet.</span></span> <span data-ttu-id="cff48-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cff48-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cff48-172">developer</span><span class="sxs-lookup"><span data-stu-id="cff48-172">developer</span></span>|<span data-ttu-id="cff48-173">String</span><span class="sxs-lookup"><span data-stu-id="cff48-173">String</span></span>|<span data-ttu-id="cff48-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="cff48-174">The name of the app.</span></span> <span data-ttu-id="cff48-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cff48-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cff48-176">notes</span><span class="sxs-lookup"><span data-stu-id="cff48-176">notes</span></span>|<span data-ttu-id="cff48-177">String</span><span class="sxs-lookup"><span data-stu-id="cff48-177">String</span></span>|<span data-ttu-id="cff48-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="cff48-178">Notes for the app.</span></span> <span data-ttu-id="cff48-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cff48-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cff48-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="cff48-180">publishingState</span></span>|<span data-ttu-id="cff48-181">String</span><span class="sxs-lookup"><span data-stu-id="cff48-181">String</span></span>|<span data-ttu-id="cff48-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="cff48-182">The publishing state for the app.</span></span> <span data-ttu-id="cff48-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="cff48-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cff48-184">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="cff48-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cff48-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="cff48-185">committedContentVersion</span></span>|<span data-ttu-id="cff48-186">String</span><span class="sxs-lookup"><span data-stu-id="cff48-186">String</span></span>|<span data-ttu-id="cff48-187">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="cff48-187">The internal committed content version.</span></span> <span data-ttu-id="cff48-188">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cff48-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="cff48-189">fileName</span><span class="sxs-lookup"><span data-stu-id="cff48-189">fileName</span></span>|<span data-ttu-id="cff48-190">String</span><span class="sxs-lookup"><span data-stu-id="cff48-190">String</span></span>|<span data-ttu-id="cff48-191">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="cff48-191">The name of the main Lob application file.</span></span> <span data-ttu-id="cff48-192">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cff48-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="cff48-193">size</span><span class="sxs-lookup"><span data-stu-id="cff48-193">size</span></span>|<span data-ttu-id="cff48-194">Int64</span><span class="sxs-lookup"><span data-stu-id="cff48-194">Int64</span></span>|<span data-ttu-id="cff48-195">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="cff48-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="cff48-196">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cff48-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="cff48-197">commandLine</span><span class="sxs-lookup"><span data-stu-id="cff48-197">Command-line:</span></span>|<span data-ttu-id="cff48-198">String</span><span class="sxs-lookup"><span data-stu-id="cff48-198">String</span></span>|<span data-ttu-id="cff48-199">命令行。</span><span class="sxs-lookup"><span data-stu-id="cff48-199">The command line.</span></span>|
|<span data-ttu-id="cff48-200">productCode</span><span class="sxs-lookup"><span data-stu-id="cff48-200">ProductCode</span></span>|<span data-ttu-id="cff48-201">String</span><span class="sxs-lookup"><span data-stu-id="cff48-201">String</span></span>|<span data-ttu-id="cff48-202">产品代码。</span><span class="sxs-lookup"><span data-stu-id="cff48-202">The product code.</span></span>|
|<span data-ttu-id="cff48-203">productVersion</span><span class="sxs-lookup"><span data-stu-id="cff48-203">productVersion</span></span>|<span data-ttu-id="cff48-204">String</span><span class="sxs-lookup"><span data-stu-id="cff48-204">String</span></span>|<span data-ttu-id="cff48-205">Windows Mobile MSI 业务线 (LoB) 应用的产品版本。</span><span class="sxs-lookup"><span data-stu-id="cff48-205">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="cff48-206">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="cff48-206">ignoreVersionDetection</span></span>|<span data-ttu-id="cff48-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="cff48-207">Boolean</span></span>|<span data-ttu-id="cff48-208">控制应用的版本是否将用于检测安装在设备上的应用的布尔值。</span><span class="sxs-lookup"><span data-stu-id="cff48-208">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="cff48-209">对于使用自更新功能的 Windows Mobile MSI 业务线 (LoB) 应用，将此值设置为 true。</span><span class="sxs-lookup"><span data-stu-id="cff48-209">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="cff48-210">响应</span><span class="sxs-lookup"><span data-stu-id="cff48-210">Response</span></span>
<span data-ttu-id="cff48-211">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cff48-211">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cff48-212">示例</span><span class="sxs-lookup"><span data-stu-id="cff48-212">Example</span></span>
### <a name="request"></a><span data-ttu-id="cff48-213">请求</span><span class="sxs-lookup"><span data-stu-id="cff48-213">Request</span></span>
<span data-ttu-id="cff48-214">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cff48-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 864

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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="cff48-215">响应</span><span class="sxs-lookup"><span data-stu-id="cff48-215">Response</span></span>
<span data-ttu-id="cff48-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cff48-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1027

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```



