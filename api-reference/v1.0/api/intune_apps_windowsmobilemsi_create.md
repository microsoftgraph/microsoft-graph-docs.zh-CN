# <a name="create-windowsmobilemsi"></a><span data-ttu-id="aab43-101">创建 windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="aab43-101">Create windowsMobileMSI</span></span>

> <span data-ttu-id="aab43-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="aab43-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aab43-103">创建新的 [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aab43-103">Create a new [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aab43-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="aab43-104">Prerequisites</span></span>
<span data-ttu-id="aab43-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="aab43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aab43-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="aab43-107">Permission type</span></span>|<span data-ttu-id="aab43-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aab43-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aab43-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aab43-109">Delegated (work or school account)</span></span>|<span data-ttu-id="aab43-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aab43-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aab43-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aab43-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aab43-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="aab43-112">Not supported.</span></span>|
|<span data-ttu-id="aab43-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="aab43-113">Application</span></span>|<span data-ttu-id="aab43-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="aab43-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aab43-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aab43-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="aab43-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="aab43-116">Request headers</span></span>
|<span data-ttu-id="aab43-117">标头</span><span class="sxs-lookup"><span data-stu-id="aab43-117">Header</span></span>|<span data-ttu-id="aab43-118">值</span><span class="sxs-lookup"><span data-stu-id="aab43-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aab43-119">授权</span><span class="sxs-lookup"><span data-stu-id="aab43-119">Authorization</span></span>|<span data-ttu-id="aab43-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aab43-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aab43-121">接受</span><span class="sxs-lookup"><span data-stu-id="aab43-121">Accept</span></span>|<span data-ttu-id="aab43-122">application/json</span><span class="sxs-lookup"><span data-stu-id="aab43-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aab43-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="aab43-123">Request body</span></span>
<span data-ttu-id="aab43-124">在请求正文中，提供 windowsMobileMSI 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aab43-124">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="aab43-125">下表显示创建 windowsMobileMSI 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aab43-125">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="aab43-126">属性</span><span class="sxs-lookup"><span data-stu-id="aab43-126">Property</span></span>|<span data-ttu-id="aab43-127">类型</span><span class="sxs-lookup"><span data-stu-id="aab43-127">Type</span></span>|<span data-ttu-id="aab43-128">说明</span><span class="sxs-lookup"><span data-stu-id="aab43-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aab43-129">ID</span><span class="sxs-lookup"><span data-stu-id="aab43-129">id</span></span>|<span data-ttu-id="aab43-130">字符串</span><span class="sxs-lookup"><span data-stu-id="aab43-130">String</span></span>|<span data-ttu-id="aab43-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="aab43-131">Key of the entity.</span></span> <span data-ttu-id="aab43-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="aab43-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="aab43-133">displayName</span><span class="sxs-lookup"><span data-stu-id="aab43-133">displayName</span></span>|<span data-ttu-id="aab43-134">字符串</span><span class="sxs-lookup"><span data-stu-id="aab43-134">String</span></span>|<span data-ttu-id="aab43-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="aab43-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="aab43-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="aab43-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="aab43-137">描述</span><span class="sxs-lookup"><span data-stu-id="aab43-137">description</span></span>|<span data-ttu-id="aab43-138">字符串</span><span class="sxs-lookup"><span data-stu-id="aab43-138">String</span></span>|<span data-ttu-id="aab43-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="aab43-139">The description of the app.</span></span> <span data-ttu-id="aab43-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="aab43-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="aab43-141">发布服务器</span><span class="sxs-lookup"><span data-stu-id="aab43-141">publisher</span></span>|<span data-ttu-id="aab43-142">字符串</span><span class="sxs-lookup"><span data-stu-id="aab43-142">String</span></span>|<span data-ttu-id="aab43-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="aab43-143">The publisher of the app.</span></span> <span data-ttu-id="aab43-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="aab43-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="aab43-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="aab43-145">largeIcon</span></span>|[<span data-ttu-id="aab43-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="aab43-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="aab43-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="aab43-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="aab43-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="aab43-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="aab43-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aab43-149">createdDateTime</span></span>|<span data-ttu-id="aab43-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aab43-150">DateTimeOffset</span></span>|<span data-ttu-id="aab43-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="aab43-151">The date and time the app was created.</span></span> <span data-ttu-id="aab43-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="aab43-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="aab43-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aab43-153">lastModifiedDateTime</span></span>|<span data-ttu-id="aab43-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aab43-154">DateTimeOffset</span></span>|<span data-ttu-id="aab43-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="aab43-155">The date and time the app was last modified.</span></span> <span data-ttu-id="aab43-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="aab43-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="aab43-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="aab43-157">isFeatured</span></span>|<span data-ttu-id="aab43-158">布尔</span><span class="sxs-lookup"><span data-stu-id="aab43-158">Boolean</span></span>|<span data-ttu-id="aab43-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="aab43-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="aab43-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="aab43-160">privacyInformationUrl</span></span>|<span data-ttu-id="aab43-161">字符串</span><span class="sxs-lookup"><span data-stu-id="aab43-161">String</span></span>|<span data-ttu-id="aab43-162">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="aab43-162">The privacy statement Url.</span></span> <span data-ttu-id="aab43-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="aab43-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="aab43-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="aab43-164">informationUrl</span></span>|<span data-ttu-id="aab43-165">字符串</span><span class="sxs-lookup"><span data-stu-id="aab43-165">String</span></span>|<span data-ttu-id="aab43-166">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="aab43-166">The more information Url.</span></span> <span data-ttu-id="aab43-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="aab43-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="aab43-168">所有者</span><span class="sxs-lookup"><span data-stu-id="aab43-168">owner</span></span>|<span data-ttu-id="aab43-169">字符串</span><span class="sxs-lookup"><span data-stu-id="aab43-169">String</span></span>|<span data-ttu-id="aab43-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="aab43-170">The owner of the app.</span></span> <span data-ttu-id="aab43-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="aab43-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="aab43-172">开发者</span><span class="sxs-lookup"><span data-stu-id="aab43-172">developer</span></span>|<span data-ttu-id="aab43-173">字符串</span><span class="sxs-lookup"><span data-stu-id="aab43-173">String</span></span>|<span data-ttu-id="aab43-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="aab43-174">The developer of the app.</span></span> <span data-ttu-id="aab43-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="aab43-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="aab43-176">备注</span><span class="sxs-lookup"><span data-stu-id="aab43-176">notes</span></span>|<span data-ttu-id="aab43-177">字符串</span><span class="sxs-lookup"><span data-stu-id="aab43-177">String</span></span>|<span data-ttu-id="aab43-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="aab43-178">Notes for the app.</span></span> <span data-ttu-id="aab43-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="aab43-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="aab43-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="aab43-180">publishingState</span></span>|[<span data-ttu-id="aab43-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="aab43-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="aab43-p114">应用的发布状态。除非应用已发布，否则不能被分配。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="aab43-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="aab43-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="aab43-186">committedContentVersion</span></span>|<span data-ttu-id="aab43-187">字符串</span><span class="sxs-lookup"><span data-stu-id="aab43-187">String</span></span>|<span data-ttu-id="aab43-188">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="aab43-188">The internal committed content version.</span></span> <span data-ttu-id="aab43-189">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="aab43-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="aab43-190">fileName</span><span class="sxs-lookup"><span data-stu-id="aab43-190">fileName</span></span>|<span data-ttu-id="aab43-191">字符串</span><span class="sxs-lookup"><span data-stu-id="aab43-191">String</span></span>|<span data-ttu-id="aab43-192">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="aab43-192">The name of the main Lob application file.</span></span> <span data-ttu-id="aab43-193">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="aab43-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="aab43-194">大小</span><span class="sxs-lookup"><span data-stu-id="aab43-194">size</span></span>|<span data-ttu-id="aab43-195">Int64</span><span class="sxs-lookup"><span data-stu-id="aab43-195">Int64</span></span>|<span data-ttu-id="aab43-196">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="aab43-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="aab43-197">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="aab43-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="aab43-198">commandLine</span><span class="sxs-lookup"><span data-stu-id="aab43-198">commandLine</span></span>|<span data-ttu-id="aab43-199">字符串</span><span class="sxs-lookup"><span data-stu-id="aab43-199">String</span></span>|<span data-ttu-id="aab43-200">命令行。</span><span class="sxs-lookup"><span data-stu-id="aab43-200">The command line.</span></span>|
|<span data-ttu-id="aab43-201">productCode</span><span class="sxs-lookup"><span data-stu-id="aab43-201">productCode</span></span>|<span data-ttu-id="aab43-202">字符串</span><span class="sxs-lookup"><span data-stu-id="aab43-202">String</span></span>|<span data-ttu-id="aab43-203">产品代码。</span><span class="sxs-lookup"><span data-stu-id="aab43-203">The product code.</span></span>|
|<span data-ttu-id="aab43-204">productVersion</span><span class="sxs-lookup"><span data-stu-id="aab43-204">productVersion</span></span>|<span data-ttu-id="aab43-205">字符串</span><span class="sxs-lookup"><span data-stu-id="aab43-205">String</span></span>|<span data-ttu-id="aab43-206">Windows Mobile MSI 业务线 (LoB) 应用的产品版本。</span><span class="sxs-lookup"><span data-stu-id="aab43-206">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="aab43-207">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="aab43-207">ignoreVersionDetection</span></span>|<span data-ttu-id="aab43-208">布尔</span><span class="sxs-lookup"><span data-stu-id="aab43-208">Boolean</span></span>|<span data-ttu-id="aab43-209">控制应用的版本是否将用于检测安装在设备上的应用的布尔值。</span><span class="sxs-lookup"><span data-stu-id="aab43-209">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="aab43-210">对于使用自更新功能的 Windows Mobile MSI 业务线 (LoB) 应用，将此值设置为 true。</span><span class="sxs-lookup"><span data-stu-id="aab43-210">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="aab43-211">响应</span><span class="sxs-lookup"><span data-stu-id="aab43-211">Response</span></span>
<span data-ttu-id="aab43-212">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aab43-212">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aab43-213">示例</span><span class="sxs-lookup"><span data-stu-id="aab43-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="aab43-214">请求</span><span class="sxs-lookup"><span data-stu-id="aab43-214">Request</span></span>
<span data-ttu-id="aab43-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aab43-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 919

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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

### <a name="response"></a><span data-ttu-id="aab43-216">响应</span><span class="sxs-lookup"><span data-stu-id="aab43-216">Response</span></span>
<span data-ttu-id="aab43-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aab43-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








