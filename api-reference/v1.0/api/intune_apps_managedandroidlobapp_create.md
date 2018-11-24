# <a name="create-managedandroidlobapp"></a><span data-ttu-id="e6748-101">创建 managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="e6748-101">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="e6748-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e6748-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6748-103">创建新的 [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e6748-103">Create a new [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e6748-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="e6748-104">Prerequisites</span></span>
<span data-ttu-id="e6748-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e6748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e6748-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6748-107">Permission type</span></span>|<span data-ttu-id="e6748-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e6748-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6748-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6748-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e6748-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6748-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e6748-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6748-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6748-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6748-112">Not supported.</span></span>|
|<span data-ttu-id="e6748-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6748-113">Application</span></span>|<span data-ttu-id="e6748-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6748-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6748-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6748-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e6748-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6748-116">Request headers</span></span>
|<span data-ttu-id="e6748-117">标头</span><span class="sxs-lookup"><span data-stu-id="e6748-117">Header</span></span>|<span data-ttu-id="e6748-118">值</span><span class="sxs-lookup"><span data-stu-id="e6748-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6748-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6748-119">Authorization</span></span>|<span data-ttu-id="e6748-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e6748-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6748-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e6748-121">Accept</span></span>|<span data-ttu-id="e6748-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e6748-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6748-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6748-123">Request body</span></span>
<span data-ttu-id="e6748-124">在请求正文中，提供 managedAndroidLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6748-124">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="e6748-125">下表显示了创建 managedAndroidLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e6748-125">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="e6748-126">属性</span><span class="sxs-lookup"><span data-stu-id="e6748-126">Property</span></span>|<span data-ttu-id="e6748-127">类型</span><span class="sxs-lookup"><span data-stu-id="e6748-127">Type</span></span>|<span data-ttu-id="e6748-128">说明</span><span class="sxs-lookup"><span data-stu-id="e6748-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6748-129">id</span><span class="sxs-lookup"><span data-stu-id="e6748-129">id</span></span>|<span data-ttu-id="e6748-130">String</span><span class="sxs-lookup"><span data-stu-id="e6748-130">String</span></span>|<span data-ttu-id="e6748-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e6748-131">Key of the entity.</span></span> <span data-ttu-id="e6748-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6748-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e6748-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e6748-133">displayName</span></span>|<span data-ttu-id="e6748-134">String</span><span class="sxs-lookup"><span data-stu-id="e6748-134">String</span></span>|<span data-ttu-id="e6748-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="e6748-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e6748-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6748-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e6748-137">description</span><span class="sxs-lookup"><span data-stu-id="e6748-137">description</span></span>|<span data-ttu-id="e6748-138">String</span><span class="sxs-lookup"><span data-stu-id="e6748-138">String</span></span>|<span data-ttu-id="e6748-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="e6748-139">The description of the app.</span></span> <span data-ttu-id="e6748-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6748-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e6748-141">publisher</span><span class="sxs-lookup"><span data-stu-id="e6748-141">publisher</span></span>|<span data-ttu-id="e6748-142">String</span><span class="sxs-lookup"><span data-stu-id="e6748-142">String</span></span>|<span data-ttu-id="e6748-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="e6748-143">The publisher of the app.</span></span> <span data-ttu-id="e6748-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6748-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e6748-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e6748-145">largeIcon</span></span>|[<span data-ttu-id="e6748-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e6748-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="e6748-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="e6748-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e6748-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6748-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e6748-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6748-149">createdDateTime</span></span>|<span data-ttu-id="e6748-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6748-150">DateTimeOffset</span></span>|<span data-ttu-id="e6748-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e6748-151">The date and time the app was created.</span></span> <span data-ttu-id="e6748-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6748-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e6748-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6748-153">lastModifiedDateTime</span></span>|<span data-ttu-id="e6748-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6748-154">DateTimeOffset</span></span>|<span data-ttu-id="e6748-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e6748-155">The date and time the app was last modified.</span></span> <span data-ttu-id="e6748-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6748-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e6748-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e6748-157">isFeatured</span></span>|<span data-ttu-id="e6748-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6748-158">Boolean</span></span>|<span data-ttu-id="e6748-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6748-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e6748-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e6748-160">privacyInformationUrl</span></span>|<span data-ttu-id="e6748-161">String</span><span class="sxs-lookup"><span data-stu-id="e6748-161">String</span></span>|<span data-ttu-id="e6748-162">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="e6748-162">The privacy statement Url.</span></span> <span data-ttu-id="e6748-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6748-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e6748-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e6748-164">informationUrl</span></span>|<span data-ttu-id="e6748-165">String</span><span class="sxs-lookup"><span data-stu-id="e6748-165">String</span></span>|<span data-ttu-id="e6748-166">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="e6748-166">The more information Url.</span></span> <span data-ttu-id="e6748-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6748-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e6748-168">owner</span><span class="sxs-lookup"><span data-stu-id="e6748-168">owner</span></span>|<span data-ttu-id="e6748-169">String</span><span class="sxs-lookup"><span data-stu-id="e6748-169">String</span></span>|<span data-ttu-id="e6748-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="e6748-170">The owner of the app.</span></span> <span data-ttu-id="e6748-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6748-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e6748-172">developer</span><span class="sxs-lookup"><span data-stu-id="e6748-172">developer</span></span>|<span data-ttu-id="e6748-173">String</span><span class="sxs-lookup"><span data-stu-id="e6748-173">String</span></span>|<span data-ttu-id="e6748-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="e6748-174">The developer of the app.</span></span> <span data-ttu-id="e6748-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6748-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e6748-176">notes</span><span class="sxs-lookup"><span data-stu-id="e6748-176">notes</span></span>|<span data-ttu-id="e6748-177">String</span><span class="sxs-lookup"><span data-stu-id="e6748-177">String</span></span>|<span data-ttu-id="e6748-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="e6748-178">Notes for the app.</span></span> <span data-ttu-id="e6748-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6748-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e6748-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="e6748-180">publishingState</span></span>|[<span data-ttu-id="e6748-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e6748-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="e6748-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="e6748-182">The publishing state for the app.</span></span> <span data-ttu-id="e6748-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="e6748-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e6748-184">继承自[mobileApp](../resources/intune_apps_mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="e6748-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="e6748-185">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="e6748-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e6748-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="e6748-186">appAvailability</span></span>|[<span data-ttu-id="e6748-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="e6748-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="e6748-188">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="e6748-188">The Application's availability.</span></span> <span data-ttu-id="e6748-189">继承自[managedApp](../resources/intune_apps_managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="e6748-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md).</span></span> <span data-ttu-id="e6748-190">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="e6748-190">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="e6748-191">version</span><span class="sxs-lookup"><span data-stu-id="e6748-191">version</span></span>|<span data-ttu-id="e6748-192">String</span><span class="sxs-lookup"><span data-stu-id="e6748-192">String</span></span>|<span data-ttu-id="e6748-193">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="e6748-193">The Application's version.</span></span> <span data-ttu-id="e6748-194">继承自 [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6748-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="e6748-195">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e6748-195">committedContentVersion</span></span>|<span data-ttu-id="e6748-196">String</span><span class="sxs-lookup"><span data-stu-id="e6748-196">String</span></span>|<span data-ttu-id="e6748-197">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="e6748-197">The internal committed content version.</span></span> <span data-ttu-id="e6748-198">继承自 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6748-198">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e6748-199">fileName</span><span class="sxs-lookup"><span data-stu-id="e6748-199">fileName</span></span>|<span data-ttu-id="e6748-200">String</span><span class="sxs-lookup"><span data-stu-id="e6748-200">String</span></span>|<span data-ttu-id="e6748-201">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="e6748-201">The name of the main Lob application file.</span></span> <span data-ttu-id="e6748-202">继承自 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6748-202">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e6748-203">size</span><span class="sxs-lookup"><span data-stu-id="e6748-203">size</span></span>|<span data-ttu-id="e6748-204">Int64</span><span class="sxs-lookup"><span data-stu-id="e6748-204">Int64</span></span>|<span data-ttu-id="e6748-205">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="e6748-205">The total size, including all uploaded files.</span></span> <span data-ttu-id="e6748-206">继承自 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6748-206">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e6748-207">packageId</span><span class="sxs-lookup"><span data-stu-id="e6748-207">packageId</span></span>|<span data-ttu-id="e6748-208">String</span><span class="sxs-lookup"><span data-stu-id="e6748-208">String</span></span>|<span data-ttu-id="e6748-209">包标识符。</span><span class="sxs-lookup"><span data-stu-id="e6748-209">The package identifier.</span></span>|
|<span data-ttu-id="e6748-210">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e6748-210">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e6748-211">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e6748-211">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="e6748-212">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="e6748-212">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e6748-213">versionName</span><span class="sxs-lookup"><span data-stu-id="e6748-213">versionName</span></span>|<span data-ttu-id="e6748-214">String</span><span class="sxs-lookup"><span data-stu-id="e6748-214">String</span></span>|<span data-ttu-id="e6748-215">托管 Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="e6748-215">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e6748-216">versionCode</span><span class="sxs-lookup"><span data-stu-id="e6748-216">versionCode</span></span>|<span data-ttu-id="e6748-217">String</span><span class="sxs-lookup"><span data-stu-id="e6748-217">String</span></span>|<span data-ttu-id="e6748-218">托管 Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="e6748-218">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="e6748-219">响应</span><span class="sxs-lookup"><span data-stu-id="e6748-219">Response</span></span>
<span data-ttu-id="e6748-220">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e6748-220">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6748-221">示例</span><span class="sxs-lookup"><span data-stu-id="e6748-221">Example</span></span>
### <a name="request"></a><span data-ttu-id="e6748-222">请求</span><span class="sxs-lookup"><span data-stu-id="e6748-222">Request</span></span>
<span data-ttu-id="e6748-223">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6748-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1153

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="e6748-224">响应</span><span class="sxs-lookup"><span data-stu-id="e6748-224">Response</span></span>
<span data-ttu-id="e6748-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6748-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1325

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "packageId": "Package Id value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```



