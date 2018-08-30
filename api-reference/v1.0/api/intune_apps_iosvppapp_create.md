# <a name="create-iosvppapp"></a><span data-ttu-id="1627a-101">创建 iosVppApp</span><span class="sxs-lookup"><span data-stu-id="1627a-101">Create iosVppApp</span></span>

> <span data-ttu-id="1627a-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1627a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1627a-103">创建新的 [iosVppApp](../resources/intune_apps_iosvppapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1627a-103">Create a new [iosVppApp](../resources/intune_apps_iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1627a-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="1627a-104">Prerequisites</span></span>
<span data-ttu-id="1627a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1627a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1627a-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="1627a-107">Permission type</span></span>|<span data-ttu-id="1627a-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1627a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1627a-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1627a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1627a-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1627a-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1627a-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1627a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1627a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="1627a-112">Not supported.</span></span>|
|<span data-ttu-id="1627a-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="1627a-113">Application</span></span>|<span data-ttu-id="1627a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1627a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1627a-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1627a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1627a-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="1627a-116">Request headers</span></span>
|<span data-ttu-id="1627a-117">标头</span><span class="sxs-lookup"><span data-stu-id="1627a-117">Header</span></span>|<span data-ttu-id="1627a-118">值</span><span class="sxs-lookup"><span data-stu-id="1627a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1627a-119">授权</span><span class="sxs-lookup"><span data-stu-id="1627a-119">Authorization</span></span>|<span data-ttu-id="1627a-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1627a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1627a-121">接受</span><span class="sxs-lookup"><span data-stu-id="1627a-121">Accept</span></span>|<span data-ttu-id="1627a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1627a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1627a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1627a-123">Request body</span></span>
<span data-ttu-id="1627a-124">在请求正文中，提供 iosVppApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1627a-124">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="1627a-125">下表显示了创建 iosVppApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1627a-125">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="1627a-126">属性</span><span class="sxs-lookup"><span data-stu-id="1627a-126">Property</span></span>|<span data-ttu-id="1627a-127">类型</span><span class="sxs-lookup"><span data-stu-id="1627a-127">Type</span></span>|<span data-ttu-id="1627a-128">说明</span><span class="sxs-lookup"><span data-stu-id="1627a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1627a-129">id</span><span class="sxs-lookup"><span data-stu-id="1627a-129">id</span></span>|<span data-ttu-id="1627a-130">String</span><span class="sxs-lookup"><span data-stu-id="1627a-130">String</span></span>|<span data-ttu-id="1627a-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1627a-131">Key of the entity.</span></span> <span data-ttu-id="1627a-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1627a-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1627a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1627a-133">displayName</span></span>|<span data-ttu-id="1627a-134">String</span><span class="sxs-lookup"><span data-stu-id="1627a-134">String</span></span>|<span data-ttu-id="1627a-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="1627a-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1627a-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1627a-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1627a-137">description</span><span class="sxs-lookup"><span data-stu-id="1627a-137">description</span></span>|<span data-ttu-id="1627a-138">String</span><span class="sxs-lookup"><span data-stu-id="1627a-138">String</span></span>|<span data-ttu-id="1627a-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="1627a-139">The description of the app.</span></span> <span data-ttu-id="1627a-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1627a-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1627a-141">publisher</span><span class="sxs-lookup"><span data-stu-id="1627a-141">publisher</span></span>|<span data-ttu-id="1627a-142">String</span><span class="sxs-lookup"><span data-stu-id="1627a-142">String</span></span>|<span data-ttu-id="1627a-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="1627a-143">The publisher of the app.</span></span> <span data-ttu-id="1627a-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1627a-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1627a-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1627a-145">largeIcon</span></span>|[<span data-ttu-id="1627a-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1627a-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="1627a-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="1627a-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1627a-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1627a-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1627a-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1627a-149">createdDateTime</span></span>|<span data-ttu-id="1627a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1627a-150">DateTimeOffset</span></span>|<span data-ttu-id="1627a-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1627a-151">The date and time the app was created.</span></span> <span data-ttu-id="1627a-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1627a-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1627a-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1627a-153">lastModifiedDateTime</span></span>|<span data-ttu-id="1627a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1627a-154">DateTimeOffset</span></span>|<span data-ttu-id="1627a-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1627a-155">The date and time the app was last modified.</span></span> <span data-ttu-id="1627a-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1627a-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1627a-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1627a-157">isFeatured</span></span>|<span data-ttu-id="1627a-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="1627a-158">Boolean</span></span>|<span data-ttu-id="1627a-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1627a-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1627a-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1627a-160">privacyInformationUrl</span></span>|<span data-ttu-id="1627a-161">String</span><span class="sxs-lookup"><span data-stu-id="1627a-161">String</span></span>|<span data-ttu-id="1627a-162">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="1627a-162">The privacy statement Url.</span></span> <span data-ttu-id="1627a-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1627a-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1627a-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1627a-164">informationUrl</span></span>|<span data-ttu-id="1627a-165">String</span><span class="sxs-lookup"><span data-stu-id="1627a-165">String</span></span>|<span data-ttu-id="1627a-166">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="1627a-166">The more information Url.</span></span> <span data-ttu-id="1627a-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1627a-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1627a-168">owner</span><span class="sxs-lookup"><span data-stu-id="1627a-168">owner</span></span>|<span data-ttu-id="1627a-169">String</span><span class="sxs-lookup"><span data-stu-id="1627a-169">String</span></span>|<span data-ttu-id="1627a-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="1627a-170">The owner of the app.</span></span> <span data-ttu-id="1627a-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1627a-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1627a-172">developer</span><span class="sxs-lookup"><span data-stu-id="1627a-172">developer</span></span>|<span data-ttu-id="1627a-173">String</span><span class="sxs-lookup"><span data-stu-id="1627a-173">String</span></span>|<span data-ttu-id="1627a-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="1627a-174">The developer of the app.</span></span> <span data-ttu-id="1627a-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1627a-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1627a-176">notes</span><span class="sxs-lookup"><span data-stu-id="1627a-176">notes</span></span>|<span data-ttu-id="1627a-177">String</span><span class="sxs-lookup"><span data-stu-id="1627a-177">String</span></span>|<span data-ttu-id="1627a-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="1627a-178">Notes for the app.</span></span> <span data-ttu-id="1627a-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1627a-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1627a-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="1627a-180">publishingState</span></span>|[<span data-ttu-id="1627a-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1627a-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="1627a-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="1627a-182">The publishing state for the app.</span></span> <span data-ttu-id="1627a-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="1627a-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1627a-184">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="1627a-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="1627a-185">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="1627a-185">The possible values are `notPublished`, `processing`, `published`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="1627a-186">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1627a-186">usedLicenseCount</span></span>|<span data-ttu-id="1627a-187">Int32</span><span class="sxs-lookup"><span data-stu-id="1627a-187">Int32</span></span>|<span data-ttu-id="1627a-188">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="1627a-188">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="1627a-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1627a-189">totalLicenseCount</span></span>|<span data-ttu-id="1627a-190">Int32</span><span class="sxs-lookup"><span data-stu-id="1627a-190">Int32</span></span>|<span data-ttu-id="1627a-191">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="1627a-191">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="1627a-192">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="1627a-192">releaseDateTime</span></span>|<span data-ttu-id="1627a-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1627a-193">DateTimeOffset</span></span>|<span data-ttu-id="1627a-194">VPP 应用程序的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1627a-194">The VPP application release date and time.</span></span>|
|<span data-ttu-id="1627a-195">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1627a-195">appStoreUrl</span></span>|<span data-ttu-id="1627a-196">String</span><span class="sxs-lookup"><span data-stu-id="1627a-196">String</span></span>|<span data-ttu-id="1627a-197">存储 URL。</span><span class="sxs-lookup"><span data-stu-id="1627a-197">The store URL.</span></span>|
|<span data-ttu-id="1627a-198">licensingType</span><span class="sxs-lookup"><span data-stu-id="1627a-198">licensingType</span></span>|[<span data-ttu-id="1627a-199">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="1627a-199">vppLicensingType</span></span>](../resources/intune_apps_vpplicensingtype.md)|<span data-ttu-id="1627a-200">受支持的许可证类型。</span><span class="sxs-lookup"><span data-stu-id="1627a-200">The supported License Type.</span></span>|
|<span data-ttu-id="1627a-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="1627a-201">applicableDeviceType</span></span>|[<span data-ttu-id="1627a-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="1627a-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="1627a-203">适用的 iOS 设备类型。</span><span class="sxs-lookup"><span data-stu-id="1627a-203">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="1627a-204">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="1627a-204">vppTokenOrganizationName</span></span>|<span data-ttu-id="1627a-205">String</span><span class="sxs-lookup"><span data-stu-id="1627a-205">String</span></span>|<span data-ttu-id="1627a-206">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="1627a-206">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="1627a-207">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="1627a-207">vppTokenAccountType</span></span>|[<span data-ttu-id="1627a-208">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="1627a-208">vppTokenAccountType</span></span>](../resources/intune_shared_vpptokenaccounttype.md)|<span data-ttu-id="1627a-209">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="1627a-209">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="1627a-210">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="1627a-210">The possible values are:</span></span> <span data-ttu-id="1627a-211">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="1627a-211">The possible values are:</span></span>|
|<span data-ttu-id="1627a-212">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="1627a-212">vppTokenAppleId</span></span>|<span data-ttu-id="1627a-213">String</span><span class="sxs-lookup"><span data-stu-id="1627a-213">String</span></span>|<span data-ttu-id="1627a-214">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="1627a-214">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="1627a-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="1627a-215">bundleId</span></span>|<span data-ttu-id="1627a-216">String</span><span class="sxs-lookup"><span data-stu-id="1627a-216">String</span></span>|<span data-ttu-id="1627a-217">标识名称。</span><span class="sxs-lookup"><span data-stu-id="1627a-217">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="1627a-218">响应</span><span class="sxs-lookup"><span data-stu-id="1627a-218">Response</span></span>
<span data-ttu-id="1627a-219">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [iosVppApp](../resources/intune_apps_iosvppapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1627a-219">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune_apps_iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1627a-220">示例</span><span class="sxs-lookup"><span data-stu-id="1627a-220">Example</span></span>
### <a name="request"></a><span data-ttu-id="1627a-221">请求</span><span class="sxs-lookup"><span data-stu-id="1627a-221">Request</span></span>
<span data-ttu-id="1627a-222">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1627a-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1286

{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```

### <a name="response"></a><span data-ttu-id="1627a-223">响应</span><span class="sxs-lookup"><span data-stu-id="1627a-223">Response</span></span>
<span data-ttu-id="1627a-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1627a-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1394

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```



