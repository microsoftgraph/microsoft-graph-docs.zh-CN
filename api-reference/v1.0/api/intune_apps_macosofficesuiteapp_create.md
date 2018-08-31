# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="3abaa-101">创建 macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="3abaa-101">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="3abaa-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3abaa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3abaa-103">创建新的 [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3abaa-103">Create a new [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3abaa-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="3abaa-104">Prerequisites</span></span>
<span data-ttu-id="3abaa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3abaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3abaa-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="3abaa-107">Permission type</span></span>|<span data-ttu-id="3abaa-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3abaa-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3abaa-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3abaa-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3abaa-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3abaa-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3abaa-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3abaa-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3abaa-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="3abaa-112">Not supported.</span></span>|
|<span data-ttu-id="3abaa-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="3abaa-113">Application</span></span>|<span data-ttu-id="3abaa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3abaa-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3abaa-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3abaa-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3abaa-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="3abaa-116">Request headers</span></span>
|<span data-ttu-id="3abaa-117">标头</span><span class="sxs-lookup"><span data-stu-id="3abaa-117">Header</span></span>|<span data-ttu-id="3abaa-118">值</span><span class="sxs-lookup"><span data-stu-id="3abaa-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3abaa-119">授权</span><span class="sxs-lookup"><span data-stu-id="3abaa-119">Authorization</span></span>|<span data-ttu-id="3abaa-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3abaa-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3abaa-121">接受</span><span class="sxs-lookup"><span data-stu-id="3abaa-121">Accept</span></span>|<span data-ttu-id="3abaa-122">application/JSON</span><span class="sxs-lookup"><span data-stu-id="3abaa-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3abaa-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3abaa-123">Request body</span></span>
<span data-ttu-id="3abaa-124">在请求正文中，提供 macOSOfficeSuiteApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3abaa-124">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="3abaa-125">下表显示创建 macOSOfficeSuiteApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3abaa-125">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="3abaa-126">属性</span><span class="sxs-lookup"><span data-stu-id="3abaa-126">Property</span></span>|<span data-ttu-id="3abaa-127">类型</span><span class="sxs-lookup"><span data-stu-id="3abaa-127">Type</span></span>|<span data-ttu-id="3abaa-128">说明</span><span class="sxs-lookup"><span data-stu-id="3abaa-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3abaa-129">ID</span><span class="sxs-lookup"><span data-stu-id="3abaa-129">id</span></span>|<span data-ttu-id="3abaa-130">字符串</span><span class="sxs-lookup"><span data-stu-id="3abaa-130">String</span></span>|<span data-ttu-id="3abaa-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3abaa-131">Key of the entity.</span></span> <span data-ttu-id="3abaa-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3abaa-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3abaa-133">显示名称</span><span class="sxs-lookup"><span data-stu-id="3abaa-133">displayName</span></span>|<span data-ttu-id="3abaa-134">字符串</span><span class="sxs-lookup"><span data-stu-id="3abaa-134">String</span></span>|<span data-ttu-id="3abaa-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="3abaa-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3abaa-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3abaa-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3abaa-137">说明</span><span class="sxs-lookup"><span data-stu-id="3abaa-137">description</span></span>|<span data-ttu-id="3abaa-138">字符串</span><span class="sxs-lookup"><span data-stu-id="3abaa-138">String</span></span>|<span data-ttu-id="3abaa-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="3abaa-139">The description of the app.</span></span> <span data-ttu-id="3abaa-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3abaa-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3abaa-141">出版商</span><span class="sxs-lookup"><span data-stu-id="3abaa-141">publisher</span></span>|<span data-ttu-id="3abaa-142">字符串</span><span class="sxs-lookup"><span data-stu-id="3abaa-142">String</span></span>|<span data-ttu-id="3abaa-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="3abaa-143">The publisher of the app.</span></span> <span data-ttu-id="3abaa-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3abaa-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3abaa-145">视图</span><span class="sxs-lookup"><span data-stu-id="3abaa-145">largeIcon</span></span>|[<span data-ttu-id="3abaa-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3abaa-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="3abaa-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="3abaa-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3abaa-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3abaa-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3abaa-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3abaa-149">createdDateTime</span></span>|<span data-ttu-id="3abaa-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3abaa-150">DateTimeOffset</span></span>|<span data-ttu-id="3abaa-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3abaa-151">The date and time the app was created.</span></span> <span data-ttu-id="3abaa-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3abaa-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3abaa-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3abaa-153">lastModifiedDateTime</span></span>|<span data-ttu-id="3abaa-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3abaa-154">DateTimeOffset</span></span>|<span data-ttu-id="3abaa-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3abaa-155">The date and time the app was last modified.</span></span> <span data-ttu-id="3abaa-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3abaa-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3abaa-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3abaa-157">isFeatured</span></span>|<span data-ttu-id="3abaa-158">布尔值</span><span class="sxs-lookup"><span data-stu-id="3abaa-158">Boolean</span></span>|<span data-ttu-id="3abaa-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3abaa-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3abaa-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3abaa-160">privacyInformationUrl</span></span>|<span data-ttu-id="3abaa-161">字符串</span><span class="sxs-lookup"><span data-stu-id="3abaa-161">String</span></span>|<span data-ttu-id="3abaa-162">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="3abaa-162">The privacy statement Url.</span></span> <span data-ttu-id="3abaa-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3abaa-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3abaa-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3abaa-164">informationUrl</span></span>|<span data-ttu-id="3abaa-165">字符串</span><span class="sxs-lookup"><span data-stu-id="3abaa-165">String</span></span>|<span data-ttu-id="3abaa-166">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="3abaa-166">The more information Url.</span></span> <span data-ttu-id="3abaa-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3abaa-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3abaa-168">拥有者</span><span class="sxs-lookup"><span data-stu-id="3abaa-168">owner</span></span>|<span data-ttu-id="3abaa-169">字符串</span><span class="sxs-lookup"><span data-stu-id="3abaa-169">String</span></span>|<span data-ttu-id="3abaa-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="3abaa-170">The owner of the app.</span></span> <span data-ttu-id="3abaa-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3abaa-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3abaa-172">开发人员</span><span class="sxs-lookup"><span data-stu-id="3abaa-172">developer</span></span>|<span data-ttu-id="3abaa-173">字符串</span><span class="sxs-lookup"><span data-stu-id="3abaa-173">String</span></span>|<span data-ttu-id="3abaa-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="3abaa-174">The developer of the app.</span></span> <span data-ttu-id="3abaa-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3abaa-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3abaa-176">注释</span><span class="sxs-lookup"><span data-stu-id="3abaa-176">notes</span></span>|<span data-ttu-id="3abaa-177">字符串</span><span class="sxs-lookup"><span data-stu-id="3abaa-177">String</span></span>|<span data-ttu-id="3abaa-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="3abaa-178">Notes for the app.</span></span> <span data-ttu-id="3abaa-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3abaa-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3abaa-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="3abaa-180">publishingState</span></span>|[<span data-ttu-id="3abaa-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3abaa-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="3abaa-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="3abaa-182">The publishing state for the app.</span></span> <span data-ttu-id="3abaa-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="3abaa-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3abaa-184">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="3abaa-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="3abaa-185">可能的取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="3abaa-185">The possible values are `notPublished`, `processing`, `published`, , , , , , , , , or .</span></span>|



## <a name="response"></a><span data-ttu-id="3abaa-186">响应</span><span class="sxs-lookup"><span data-stu-id="3abaa-186">Response</span></span>
<span data-ttu-id="3abaa-187">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3abaa-187">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3abaa-188">示例</span><span class="sxs-lookup"><span data-stu-id="3abaa-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="3abaa-189">请求</span><span class="sxs-lookup"><span data-stu-id="3abaa-189">Request</span></span>
<span data-ttu-id="3abaa-190">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3abaa-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 648

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="3abaa-191">响应</span><span class="sxs-lookup"><span data-stu-id="3abaa-191">Response</span></span>
<span data-ttu-id="3abaa-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3abaa-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 756

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
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
  "publishingState": "processing"
}
```



