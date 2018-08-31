# <a name="update-ioslobapp"></a><span data-ttu-id="0963b-101">更新 iosLobApp</span><span class="sxs-lookup"><span data-stu-id="0963b-101">Update iosLobApp</span></span>

> <span data-ttu-id="0963b-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0963b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0963b-103">更新 [iosLobApp](../resources/intune_apps_ioslobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0963b-103">Update the properties of a [iosLobApp](../resources/intune_apps_ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0963b-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="0963b-104">Prerequisites</span></span>
<span data-ttu-id="0963b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0963b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0963b-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="0963b-107">Permission type</span></span>|<span data-ttu-id="0963b-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0963b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0963b-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0963b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0963b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0963b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0963b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0963b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0963b-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="0963b-112">Not supported.</span></span>|
|<span data-ttu-id="0963b-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="0963b-113">Application</span></span>|<span data-ttu-id="0963b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0963b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0963b-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0963b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="0963b-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="0963b-116">Request headers</span></span>
|<span data-ttu-id="0963b-117">标头</span><span class="sxs-lookup"><span data-stu-id="0963b-117">Header</span></span>|<span data-ttu-id="0963b-118">值</span><span class="sxs-lookup"><span data-stu-id="0963b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0963b-119">授权</span><span class="sxs-lookup"><span data-stu-id="0963b-119">Authorization</span></span>|<span data-ttu-id="0963b-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0963b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0963b-121">接受</span><span class="sxs-lookup"><span data-stu-id="0963b-121">Accept</span></span>|<span data-ttu-id="0963b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0963b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0963b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0963b-123">Request body</span></span>
<span data-ttu-id="0963b-124">在请求正文中，提供 [iosLobApp](../resources/intune_apps_ioslobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0963b-124">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune_apps_ioslobapp.md) object.</span></span>

<span data-ttu-id="0963b-125">下表显示了创建 [iosLobApp](../resources/intune_apps_ioslobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0963b-125">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune_apps_ioslobapp.md).</span></span>

|<span data-ttu-id="0963b-126">属性</span><span class="sxs-lookup"><span data-stu-id="0963b-126">Property</span></span>|<span data-ttu-id="0963b-127">类型</span><span class="sxs-lookup"><span data-stu-id="0963b-127">Type</span></span>|<span data-ttu-id="0963b-128">说明</span><span class="sxs-lookup"><span data-stu-id="0963b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0963b-129">id</span><span class="sxs-lookup"><span data-stu-id="0963b-129">id</span></span>|<span data-ttu-id="0963b-130">字符串</span><span class="sxs-lookup"><span data-stu-id="0963b-130">String</span></span>|<span data-ttu-id="0963b-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0963b-131">Key of the entity.</span></span> <span data-ttu-id="0963b-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0963b-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0963b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0963b-133">displayName</span></span>|<span data-ttu-id="0963b-134">字符串</span><span class="sxs-lookup"><span data-stu-id="0963b-134">String</span></span>|<span data-ttu-id="0963b-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="0963b-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0963b-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0963b-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0963b-137">description</span><span class="sxs-lookup"><span data-stu-id="0963b-137">description</span></span>|<span data-ttu-id="0963b-138">字符串</span><span class="sxs-lookup"><span data-stu-id="0963b-138">String</span></span>|<span data-ttu-id="0963b-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="0963b-139">The description of the app.</span></span> <span data-ttu-id="0963b-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0963b-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0963b-141">publisher</span><span class="sxs-lookup"><span data-stu-id="0963b-141">publisher</span></span>|<span data-ttu-id="0963b-142">字符串</span><span class="sxs-lookup"><span data-stu-id="0963b-142">String</span></span>|<span data-ttu-id="0963b-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="0963b-143">The publisher of the app.</span></span> <span data-ttu-id="0963b-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0963b-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0963b-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0963b-145">largeIcon</span></span>|[<span data-ttu-id="0963b-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0963b-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="0963b-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="0963b-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0963b-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0963b-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0963b-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0963b-149">createdDateTime</span></span>|<span data-ttu-id="0963b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0963b-150">DateTimeOffset</span></span>|<span data-ttu-id="0963b-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0963b-151">The date and time the app was created.</span></span> <span data-ttu-id="0963b-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0963b-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0963b-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0963b-153">lastModifiedDateTime</span></span>|<span data-ttu-id="0963b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0963b-154">DateTimeOffset</span></span>|<span data-ttu-id="0963b-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0963b-155">The date and time the app was last modified.</span></span> <span data-ttu-id="0963b-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0963b-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0963b-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0963b-157">isFeatured</span></span>|<span data-ttu-id="0963b-158">布尔值</span><span class="sxs-lookup"><span data-stu-id="0963b-158">Boolean</span></span>|<span data-ttu-id="0963b-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0963b-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0963b-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0963b-160">privacyInformationUrl</span></span>|<span data-ttu-id="0963b-161">字符串</span><span class="sxs-lookup"><span data-stu-id="0963b-161">String</span></span>|<span data-ttu-id="0963b-162">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="0963b-162">The privacy statement Url.</span></span> <span data-ttu-id="0963b-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0963b-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0963b-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0963b-164">informationUrl</span></span>|<span data-ttu-id="0963b-165">字符串</span><span class="sxs-lookup"><span data-stu-id="0963b-165">String</span></span>|<span data-ttu-id="0963b-166">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="0963b-166">The more information Url.</span></span> <span data-ttu-id="0963b-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0963b-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0963b-168">owner</span><span class="sxs-lookup"><span data-stu-id="0963b-168">owner</span></span>|<span data-ttu-id="0963b-169">字符串</span><span class="sxs-lookup"><span data-stu-id="0963b-169">String</span></span>|<span data-ttu-id="0963b-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="0963b-170">The owner of the app.</span></span> <span data-ttu-id="0963b-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0963b-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0963b-172">developer</span><span class="sxs-lookup"><span data-stu-id="0963b-172">developer</span></span>|<span data-ttu-id="0963b-173">字符串</span><span class="sxs-lookup"><span data-stu-id="0963b-173">String</span></span>|<span data-ttu-id="0963b-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="0963b-174">The developer of the app.</span></span> <span data-ttu-id="0963b-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0963b-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0963b-176">notes</span><span class="sxs-lookup"><span data-stu-id="0963b-176">notes</span></span>|<span data-ttu-id="0963b-177">字符串</span><span class="sxs-lookup"><span data-stu-id="0963b-177">String</span></span>|<span data-ttu-id="0963b-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="0963b-178">Notes for the app.</span></span> <span data-ttu-id="0963b-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0963b-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0963b-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="0963b-180">publishingState</span></span>|[<span data-ttu-id="0963b-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0963b-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="0963b-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="0963b-182">The publishing state for the app.</span></span> <span data-ttu-id="0963b-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="0963b-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0963b-184">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="0963b-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="0963b-185">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="0963b-185">The possible values are `notPublished`, `processing`, `published`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="0963b-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="0963b-186">committedContentVersion</span></span>|<span data-ttu-id="0963b-187">字符串</span><span class="sxs-lookup"><span data-stu-id="0963b-187">String</span></span>|<span data-ttu-id="0963b-188">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="0963b-188">The internal committed content version.</span></span> <span data-ttu-id="0963b-189">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0963b-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="0963b-190">fileName</span><span class="sxs-lookup"><span data-stu-id="0963b-190">fileName</span></span>|<span data-ttu-id="0963b-191">字符串</span><span class="sxs-lookup"><span data-stu-id="0963b-191">String</span></span>|<span data-ttu-id="0963b-192">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="0963b-192">The name of the main Lob application file.</span></span> <span data-ttu-id="0963b-193">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0963b-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="0963b-194">size</span><span class="sxs-lookup"><span data-stu-id="0963b-194">size</span></span>|<span data-ttu-id="0963b-195">Int64</span><span class="sxs-lookup"><span data-stu-id="0963b-195">Int64</span></span>|<span data-ttu-id="0963b-196">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="0963b-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="0963b-197">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0963b-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="0963b-198">bundleId</span><span class="sxs-lookup"><span data-stu-id="0963b-198">bundleId</span></span>|<span data-ttu-id="0963b-199">字符串</span><span class="sxs-lookup"><span data-stu-id="0963b-199">String</span></span>|<span data-ttu-id="0963b-200">标识名称。</span><span class="sxs-lookup"><span data-stu-id="0963b-200">The Identity Name.</span></span>|
|<span data-ttu-id="0963b-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="0963b-201">applicableDeviceType</span></span>|[<span data-ttu-id="0963b-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="0963b-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="0963b-203">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="0963b-203">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="0963b-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0963b-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0963b-205">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0963b-205">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="0963b-206">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="0963b-206">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="0963b-207">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0963b-207">expirationDateTime</span></span>|<span data-ttu-id="0963b-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0963b-208">DateTimeOffset</span></span>|<span data-ttu-id="0963b-209">过期时间。</span><span class="sxs-lookup"><span data-stu-id="0963b-209">The expiration time.</span></span>|
|<span data-ttu-id="0963b-210">versionNumber</span><span class="sxs-lookup"><span data-stu-id="0963b-210">versionNumber</span></span>|<span data-ttu-id="0963b-211">字符串</span><span class="sxs-lookup"><span data-stu-id="0963b-211">String</span></span>|<span data-ttu-id="0963b-212">iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="0963b-212">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="0963b-213">buildNumber</span><span class="sxs-lookup"><span data-stu-id="0963b-213">buildNumber</span></span>|<span data-ttu-id="0963b-214">字符串</span><span class="sxs-lookup"><span data-stu-id="0963b-214">String</span></span>|<span data-ttu-id="0963b-215">iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="0963b-215">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="0963b-216">响应</span><span class="sxs-lookup"><span data-stu-id="0963b-216">Response</span></span>
<span data-ttu-id="0963b-217">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosLobApp](../resources/intune_apps_ioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0963b-217">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune_apps_ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0963b-218">示例</span><span class="sxs-lookup"><span data-stu-id="0963b-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="0963b-219">请求</span><span class="sxs-lookup"><span data-stu-id="0963b-219">Request</span></span>
<span data-ttu-id="0963b-220">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0963b-220">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1205

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
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="0963b-221">响应</span><span class="sxs-lookup"><span data-stu-id="0963b-221">Response</span></span>
<span data-ttu-id="0963b-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0963b-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```



