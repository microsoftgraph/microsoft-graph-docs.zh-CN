# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="fbcbc-101">更新 macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="fbcbc-101">Update macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="fbcbc-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbcbc-103">更新 [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-103">Update the properties of a [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fbcbc-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="fbcbc-104">Prerequisites</span></span>
<span data-ttu-id="fbcbc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fbcbc-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="fbcbc-107">Permission type</span></span>|<span data-ttu-id="fbcbc-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fbcbc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbcbc-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fbcbc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fbcbc-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbcbc-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fbcbc-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fbcbc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbcbc-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-112">Not supported.</span></span>|
|<span data-ttu-id="fbcbc-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="fbcbc-113">Application</span></span>|<span data-ttu-id="fbcbc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbcbc-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fbcbc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="fbcbc-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="fbcbc-116">Request headers</span></span>
|<span data-ttu-id="fbcbc-117">标头</span><span class="sxs-lookup"><span data-stu-id="fbcbc-117">Header</span></span>|<span data-ttu-id="fbcbc-118">值</span><span class="sxs-lookup"><span data-stu-id="fbcbc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbcbc-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbcbc-119">Authorization</span></span>|<span data-ttu-id="fbcbc-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbcbc-121">Accept</span><span class="sxs-lookup"><span data-stu-id="fbcbc-121">Accept</span></span>|<span data-ttu-id="fbcbc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fbcbc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbcbc-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="fbcbc-123">Request body</span></span>
<span data-ttu-id="fbcbc-124">在请求正文中，提供 [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-124">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="fbcbc-125">下表显示创建 [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-125">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="fbcbc-126">属性</span><span class="sxs-lookup"><span data-stu-id="fbcbc-126">Property</span></span>|<span data-ttu-id="fbcbc-127">类型</span><span class="sxs-lookup"><span data-stu-id="fbcbc-127">Type</span></span>|<span data-ttu-id="fbcbc-128">说明</span><span class="sxs-lookup"><span data-stu-id="fbcbc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbcbc-129">id</span><span class="sxs-lookup"><span data-stu-id="fbcbc-129">id</span></span>|<span data-ttu-id="fbcbc-130">String</span><span class="sxs-lookup"><span data-stu-id="fbcbc-130">String</span></span>|<span data-ttu-id="fbcbc-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-131">Key of the entity.</span></span> <span data-ttu-id="fbcbc-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbcbc-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fbcbc-133">displayName</span><span class="sxs-lookup"><span data-stu-id="fbcbc-133">displayName</span></span>|<span data-ttu-id="fbcbc-134">String</span><span class="sxs-lookup"><span data-stu-id="fbcbc-134">String</span></span>|<span data-ttu-id="fbcbc-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fbcbc-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbcbc-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fbcbc-137">description</span><span class="sxs-lookup"><span data-stu-id="fbcbc-137">description</span></span>|<span data-ttu-id="fbcbc-138">String</span><span class="sxs-lookup"><span data-stu-id="fbcbc-138">String</span></span>|<span data-ttu-id="fbcbc-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-139">The description of the app.</span></span> <span data-ttu-id="fbcbc-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbcbc-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fbcbc-141">publisher</span><span class="sxs-lookup"><span data-stu-id="fbcbc-141">publisher</span></span>|<span data-ttu-id="fbcbc-142">String</span><span class="sxs-lookup"><span data-stu-id="fbcbc-142">String</span></span>|<span data-ttu-id="fbcbc-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-143">The publisher of the app.</span></span> <span data-ttu-id="fbcbc-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbcbc-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fbcbc-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fbcbc-145">largeIcon</span></span>|[<span data-ttu-id="fbcbc-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fbcbc-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="fbcbc-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fbcbc-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbcbc-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fbcbc-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fbcbc-149">createdDateTime</span></span>|<span data-ttu-id="fbcbc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbcbc-150">DateTimeOffset</span></span>|<span data-ttu-id="fbcbc-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-151">The date and time the app was created.</span></span> <span data-ttu-id="fbcbc-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbcbc-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fbcbc-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbcbc-153">lastModifiedDateTime</span></span>|<span data-ttu-id="fbcbc-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbcbc-154">DateTimeOffset</span></span>|<span data-ttu-id="fbcbc-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-155">The date and time the app was last modified.</span></span> <span data-ttu-id="fbcbc-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbcbc-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fbcbc-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fbcbc-157">isFeatured</span></span>|<span data-ttu-id="fbcbc-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbcbc-158">Boolean</span></span>|<span data-ttu-id="fbcbc-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbcbc-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fbcbc-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fbcbc-160">privacyInformationUrl</span></span>|<span data-ttu-id="fbcbc-161">String</span><span class="sxs-lookup"><span data-stu-id="fbcbc-161">String</span></span>|<span data-ttu-id="fbcbc-162">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-162">The privacy statement Url.</span></span> <span data-ttu-id="fbcbc-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbcbc-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fbcbc-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fbcbc-164">informationUrl</span></span>|<span data-ttu-id="fbcbc-165">String</span><span class="sxs-lookup"><span data-stu-id="fbcbc-165">String</span></span>|<span data-ttu-id="fbcbc-166">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-166">The more information Url.</span></span> <span data-ttu-id="fbcbc-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbcbc-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fbcbc-168">owner</span><span class="sxs-lookup"><span data-stu-id="fbcbc-168">owner</span></span>|<span data-ttu-id="fbcbc-169">String</span><span class="sxs-lookup"><span data-stu-id="fbcbc-169">String</span></span>|<span data-ttu-id="fbcbc-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-170">The owner of the app.</span></span> <span data-ttu-id="fbcbc-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbcbc-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fbcbc-172">developer</span><span class="sxs-lookup"><span data-stu-id="fbcbc-172">developer</span></span>|<span data-ttu-id="fbcbc-173">String</span><span class="sxs-lookup"><span data-stu-id="fbcbc-173">String</span></span>|<span data-ttu-id="fbcbc-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-174">The developer of the app.</span></span> <span data-ttu-id="fbcbc-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbcbc-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fbcbc-176">notes</span><span class="sxs-lookup"><span data-stu-id="fbcbc-176">notes</span></span>|<span data-ttu-id="fbcbc-177">String</span><span class="sxs-lookup"><span data-stu-id="fbcbc-177">String</span></span>|<span data-ttu-id="fbcbc-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-178">Notes for the app.</span></span> <span data-ttu-id="fbcbc-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbcbc-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fbcbc-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="fbcbc-180">publishingState</span></span>|[<span data-ttu-id="fbcbc-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="fbcbc-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="fbcbc-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-182">The publishing state for the app.</span></span> <span data-ttu-id="fbcbc-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fbcbc-184">继承自[mobileApp](../resources/intune_apps_mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="fbcbc-185">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="fbcbc-186">响应</span><span class="sxs-lookup"><span data-stu-id="fbcbc-186">Response</span></span>
<span data-ttu-id="fbcbc-187">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-187">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbcbc-188">示例</span><span class="sxs-lookup"><span data-stu-id="fbcbc-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="fbcbc-189">请求</span><span class="sxs-lookup"><span data-stu-id="fbcbc-189">Request</span></span>
<span data-ttu-id="fbcbc-190">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 584

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
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="fbcbc-191">响应</span><span class="sxs-lookup"><span data-stu-id="fbcbc-191">Response</span></span>
<span data-ttu-id="fbcbc-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fbcbc-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



