# <a name="create-managedioslobapp"></a><span data-ttu-id="2a707-101">创建 managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="2a707-101">Create managedIOSLobApp</span></span>

> <span data-ttu-id="2a707-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2a707-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a707-103">创建新的 [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2a707-103">Create a new [plannerBucket](../resources/intune_apps_managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a707-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="2a707-104">Prerequisites</span></span>
<span data-ttu-id="2a707-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2a707-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2a707-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a707-107">Permission type</span></span>|<span data-ttu-id="2a707-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2a707-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a707-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a707-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2a707-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a707-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2a707-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a707-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a707-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a707-112">Not supported.</span></span>|
|<span data-ttu-id="2a707-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a707-113">Application</span></span>|<span data-ttu-id="2a707-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a707-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a707-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a707-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2a707-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a707-116">Request headers</span></span>
|<span data-ttu-id="2a707-117">标头</span><span class="sxs-lookup"><span data-stu-id="2a707-117">Header</span></span>|<span data-ttu-id="2a707-118">值</span><span class="sxs-lookup"><span data-stu-id="2a707-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a707-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a707-119">Authorization</span></span>|<span data-ttu-id="2a707-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2a707-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2a707-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2a707-121">Accept</span></span>|<span data-ttu-id="2a707-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2a707-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a707-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a707-123">Request body</span></span>
<span data-ttu-id="2a707-124">在请求正文中，提供 managedIOSLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a707-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="2a707-125">下表显示创建 managedIOSLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2a707-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="2a707-126">属性</span><span class="sxs-lookup"><span data-stu-id="2a707-126">Property</span></span>|<span data-ttu-id="2a707-127">类型</span><span class="sxs-lookup"><span data-stu-id="2a707-127">Type</span></span>|<span data-ttu-id="2a707-128">说明</span><span class="sxs-lookup"><span data-stu-id="2a707-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a707-129">id</span><span class="sxs-lookup"><span data-stu-id="2a707-129">id</span></span>|<span data-ttu-id="2a707-130">String</span><span class="sxs-lookup"><span data-stu-id="2a707-130">String</span></span>|<span data-ttu-id="2a707-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2a707-131">Key of the setting.</span></span> <span data-ttu-id="2a707-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a707-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a707-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2a707-133">displayName</span></span>|<span data-ttu-id="2a707-134">String</span><span class="sxs-lookup"><span data-stu-id="2a707-134">String</span></span>|<span data-ttu-id="2a707-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="2a707-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2a707-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a707-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a707-137">description</span><span class="sxs-lookup"><span data-stu-id="2a707-137">description</span></span>|<span data-ttu-id="2a707-138">String</span><span class="sxs-lookup"><span data-stu-id="2a707-138">String</span></span>|<span data-ttu-id="2a707-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="2a707-139">The description of the app.</span></span> <span data-ttu-id="2a707-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a707-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a707-141">publisher</span><span class="sxs-lookup"><span data-stu-id="2a707-141">Publisher</span></span>|<span data-ttu-id="2a707-142">String</span><span class="sxs-lookup"><span data-stu-id="2a707-142">String</span></span>|<span data-ttu-id="2a707-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="2a707-143">The name of the app.</span></span> <span data-ttu-id="2a707-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a707-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a707-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2a707-145">largeIcon</span></span>|[<span data-ttu-id="2a707-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2a707-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="2a707-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="2a707-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2a707-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a707-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a707-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a707-149">createdDateTime</span></span>|<span data-ttu-id="2a707-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a707-150">DateTimeOffset</span></span>|<span data-ttu-id="2a707-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2a707-151">The date and time when the page was created.</span></span> <span data-ttu-id="2a707-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a707-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a707-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a707-153">lastModifiedDateTime</span></span>|<span data-ttu-id="2a707-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a707-154">DateTimeOffset</span></span>|<span data-ttu-id="2a707-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2a707-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="2a707-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a707-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a707-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2a707-157">isFeatured</span></span>|<span data-ttu-id="2a707-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a707-158">Boolean</span></span>|<span data-ttu-id="2a707-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a707-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a707-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2a707-160">privacyInformationUrl</span></span>|<span data-ttu-id="2a707-161">String</span><span class="sxs-lookup"><span data-stu-id="2a707-161">String</span></span>|<span data-ttu-id="2a707-162">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="2a707-162">The privacy statement Url.</span></span> <span data-ttu-id="2a707-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a707-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a707-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2a707-164">informationUrl</span></span>|<span data-ttu-id="2a707-165">String</span><span class="sxs-lookup"><span data-stu-id="2a707-165">String</span></span>|<span data-ttu-id="2a707-166">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="2a707-166">The more information Url.</span></span> <span data-ttu-id="2a707-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a707-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a707-168">owner</span><span class="sxs-lookup"><span data-stu-id="2a707-168">owner</span></span>|<span data-ttu-id="2a707-169">String</span><span class="sxs-lookup"><span data-stu-id="2a707-169">String</span></span>|<span data-ttu-id="2a707-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="2a707-170">The owner of the timesheet.</span></span> <span data-ttu-id="2a707-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a707-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a707-172">developer</span><span class="sxs-lookup"><span data-stu-id="2a707-172">developer</span></span>|<span data-ttu-id="2a707-173">String</span><span class="sxs-lookup"><span data-stu-id="2a707-173">String</span></span>|<span data-ttu-id="2a707-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="2a707-174">The name of the app.</span></span> <span data-ttu-id="2a707-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a707-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a707-176">notes</span><span class="sxs-lookup"><span data-stu-id="2a707-176">notes</span></span>|<span data-ttu-id="2a707-177">String</span><span class="sxs-lookup"><span data-stu-id="2a707-177">String</span></span>|<span data-ttu-id="2a707-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="2a707-178">Notes for the app.</span></span> <span data-ttu-id="2a707-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a707-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a707-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="2a707-180">publishingState</span></span>|<span data-ttu-id="2a707-181">String</span><span class="sxs-lookup"><span data-stu-id="2a707-181">String</span></span>|<span data-ttu-id="2a707-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="2a707-182">The publishing state for the app.</span></span> <span data-ttu-id="2a707-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="2a707-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2a707-184">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="2a707-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2a707-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="2a707-185">appAvailability</span></span>|<span data-ttu-id="2a707-186">String</span><span class="sxs-lookup"><span data-stu-id="2a707-186">String</span></span>|<span data-ttu-id="2a707-187">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="2a707-187">The Application's availability.</span></span> <span data-ttu-id="2a707-188">继承自 [managedApp](../resources/intune_apps_managedapp.md)。可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="2a707-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="2a707-189">version</span><span class="sxs-lookup"><span data-stu-id="2a707-189">version</span></span>|<span data-ttu-id="2a707-190">String</span><span class="sxs-lookup"><span data-stu-id="2a707-190">String</span></span>|<span data-ttu-id="2a707-191">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="2a707-191">The Application's version.</span></span> <span data-ttu-id="2a707-192">继承自 [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a707-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="2a707-193">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="2a707-193">committedContentVersion</span></span>|<span data-ttu-id="2a707-194">String</span><span class="sxs-lookup"><span data-stu-id="2a707-194">String</span></span>|<span data-ttu-id="2a707-195">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="2a707-195">The internal committed content version.</span></span> <span data-ttu-id="2a707-196">继承自 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a707-196">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="2a707-197">fileName</span><span class="sxs-lookup"><span data-stu-id="2a707-197">fileName</span></span>|<span data-ttu-id="2a707-198">String</span><span class="sxs-lookup"><span data-stu-id="2a707-198">String</span></span>|<span data-ttu-id="2a707-199">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="2a707-199">The name of the main Lob application file.</span></span> <span data-ttu-id="2a707-200">继承自 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a707-200">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="2a707-201">size</span><span class="sxs-lookup"><span data-stu-id="2a707-201">size</span></span>|<span data-ttu-id="2a707-202">Int64</span><span class="sxs-lookup"><span data-stu-id="2a707-202">Int64</span></span>|<span data-ttu-id="2a707-203">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="2a707-203">The total size, including all uploaded files.</span></span> <span data-ttu-id="2a707-204">继承自 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a707-204">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="2a707-205">bundleId</span><span class="sxs-lookup"><span data-stu-id="2a707-205">bundleId</span></span>|<span data-ttu-id="2a707-206">String</span><span class="sxs-lookup"><span data-stu-id="2a707-206">String</span></span>|<span data-ttu-id="2a707-207">标识名称。</span><span class="sxs-lookup"><span data-stu-id="2a707-207">The Identity Name.</span></span>|
|<span data-ttu-id="2a707-208">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="2a707-208">applicableDeviceType</span></span>|[<span data-ttu-id="2a707-209">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="2a707-209">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="2a707-210">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="2a707-210">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="2a707-211">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2a707-211">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2a707-212">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2a707-212">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="2a707-213">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="2a707-213">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="2a707-214">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2a707-214">expirationDateTime</span></span>|<span data-ttu-id="2a707-215">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a707-215">DateTimeOffset</span></span>|<span data-ttu-id="2a707-216">过期时间。</span><span class="sxs-lookup"><span data-stu-id="2a707-216">: The expiration time for the subscription.</span></span>|
|<span data-ttu-id="2a707-217">versionNumber</span><span class="sxs-lookup"><span data-stu-id="2a707-217">versionNumber</span></span>|<span data-ttu-id="2a707-218">String</span><span class="sxs-lookup"><span data-stu-id="2a707-218">String</span></span>|<span data-ttu-id="2a707-219">托管 iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="2a707-219">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="2a707-220">buildNumber</span><span class="sxs-lookup"><span data-stu-id="2a707-220">buildNumber</span></span>|<span data-ttu-id="2a707-221">String</span><span class="sxs-lookup"><span data-stu-id="2a707-221">String</span></span>|<span data-ttu-id="2a707-222">托管 iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="2a707-222">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="2a707-223">响应</span><span class="sxs-lookup"><span data-stu-id="2a707-223">Response</span></span>
<span data-ttu-id="2a707-224">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2a707-224">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_apps_managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a707-225">示例</span><span class="sxs-lookup"><span data-stu-id="2a707-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a707-226">请求</span><span class="sxs-lookup"><span data-stu-id="2a707-226">Request</span></span>
<span data-ttu-id="2a707-227">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a707-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1331

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="2a707-228">响应</span><span class="sxs-lookup"><span data-stu-id="2a707-228">Response</span></span>
<span data-ttu-id="2a707-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a707-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1439

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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



