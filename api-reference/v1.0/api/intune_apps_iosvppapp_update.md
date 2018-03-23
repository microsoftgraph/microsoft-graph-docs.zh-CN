# <a name="update-iosvppapp"></a><span data-ttu-id="be4c2-101">更新 iosVppApp</span><span class="sxs-lookup"><span data-stu-id="be4c2-101">Update iosVppApp</span></span>

> <span data-ttu-id="be4c2-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="be4c2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be4c2-103">更新 [iosVppApp](../resources/intune_apps_iosvppapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="be4c2-103">Update the properties of a [calendar](../resources/intune_apps_iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be4c2-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="be4c2-104">Prerequisites</span></span>
<span data-ttu-id="be4c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="be4c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="be4c2-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="be4c2-107">Permission type</span></span>|<span data-ttu-id="be4c2-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="be4c2-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be4c2-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be4c2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="be4c2-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4c2-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="be4c2-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be4c2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be4c2-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="be4c2-112">Not supported.</span></span>|
|<span data-ttu-id="be4c2-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="be4c2-113">Application</span></span>|<span data-ttu-id="be4c2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="be4c2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be4c2-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be4c2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="be4c2-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="be4c2-116">Request headers</span></span>
|<span data-ttu-id="be4c2-117">标头</span><span class="sxs-lookup"><span data-stu-id="be4c2-117">Header</span></span>|<span data-ttu-id="be4c2-118">值</span><span class="sxs-lookup"><span data-stu-id="be4c2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be4c2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="be4c2-119">Authorization</span></span>|<span data-ttu-id="be4c2-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="be4c2-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="be4c2-121">Accept</span><span class="sxs-lookup"><span data-stu-id="be4c2-121">Accept</span></span>|<span data-ttu-id="be4c2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="be4c2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be4c2-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="be4c2-123">Request body</span></span>
<span data-ttu-id="be4c2-124">在请求正文中，提供 [iosVppApp](../resources/intune_apps_iosvppapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be4c2-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_iosvppapp.md) object.</span></span>

<span data-ttu-id="be4c2-125">下表显示了创建 [iosVppApp](../resources/intune_apps_iosvppapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="be4c2-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="be4c2-126">属性</span><span class="sxs-lookup"><span data-stu-id="be4c2-126">Property</span></span>|<span data-ttu-id="be4c2-127">类型</span><span class="sxs-lookup"><span data-stu-id="be4c2-127">Type</span></span>|<span data-ttu-id="be4c2-128">说明</span><span class="sxs-lookup"><span data-stu-id="be4c2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be4c2-129">id</span><span class="sxs-lookup"><span data-stu-id="be4c2-129">id</span></span>|<span data-ttu-id="be4c2-130">String</span><span class="sxs-lookup"><span data-stu-id="be4c2-130">String</span></span>|<span data-ttu-id="be4c2-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="be4c2-131">Key of the setting.</span></span> <span data-ttu-id="be4c2-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="be4c2-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="be4c2-133">displayName</span><span class="sxs-lookup"><span data-stu-id="be4c2-133">displayName</span></span>|<span data-ttu-id="be4c2-134">String</span><span class="sxs-lookup"><span data-stu-id="be4c2-134">String</span></span>|<span data-ttu-id="be4c2-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="be4c2-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="be4c2-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="be4c2-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="be4c2-137">description</span><span class="sxs-lookup"><span data-stu-id="be4c2-137">description</span></span>|<span data-ttu-id="be4c2-138">String</span><span class="sxs-lookup"><span data-stu-id="be4c2-138">String</span></span>|<span data-ttu-id="be4c2-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="be4c2-139">The description of the app.</span></span> <span data-ttu-id="be4c2-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="be4c2-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="be4c2-141">publisher</span><span class="sxs-lookup"><span data-stu-id="be4c2-141">Publisher</span></span>|<span data-ttu-id="be4c2-142">String</span><span class="sxs-lookup"><span data-stu-id="be4c2-142">String</span></span>|<span data-ttu-id="be4c2-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="be4c2-143">The name of the app.</span></span> <span data-ttu-id="be4c2-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="be4c2-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="be4c2-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="be4c2-145">largeIcon</span></span>|[<span data-ttu-id="be4c2-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="be4c2-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="be4c2-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="be4c2-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="be4c2-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="be4c2-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="be4c2-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be4c2-149">createdDateTime</span></span>|<span data-ttu-id="be4c2-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be4c2-150">DateTimeOffset</span></span>|<span data-ttu-id="be4c2-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="be4c2-151">The date and time when the page was created.</span></span> <span data-ttu-id="be4c2-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="be4c2-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="be4c2-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be4c2-153">lastModifiedDateTime</span></span>|<span data-ttu-id="be4c2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be4c2-154">DateTimeOffset</span></span>|<span data-ttu-id="be4c2-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="be4c2-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="be4c2-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="be4c2-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="be4c2-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="be4c2-157">isFeatured</span></span>|<span data-ttu-id="be4c2-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="be4c2-158">Boolean</span></span>|<span data-ttu-id="be4c2-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="be4c2-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="be4c2-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="be4c2-160">privacyInformationUrl</span></span>|<span data-ttu-id="be4c2-161">String</span><span class="sxs-lookup"><span data-stu-id="be4c2-161">String</span></span>|<span data-ttu-id="be4c2-162">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="be4c2-162">The privacy statement Url.</span></span> <span data-ttu-id="be4c2-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="be4c2-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="be4c2-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="be4c2-164">informationUrl</span></span>|<span data-ttu-id="be4c2-165">String</span><span class="sxs-lookup"><span data-stu-id="be4c2-165">String</span></span>|<span data-ttu-id="be4c2-166">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="be4c2-166">The more information Url.</span></span> <span data-ttu-id="be4c2-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="be4c2-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="be4c2-168">owner</span><span class="sxs-lookup"><span data-stu-id="be4c2-168">owner</span></span>|<span data-ttu-id="be4c2-169">String</span><span class="sxs-lookup"><span data-stu-id="be4c2-169">String</span></span>|<span data-ttu-id="be4c2-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="be4c2-170">The owner of the timesheet.</span></span> <span data-ttu-id="be4c2-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="be4c2-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="be4c2-172">developer</span><span class="sxs-lookup"><span data-stu-id="be4c2-172">developer</span></span>|<span data-ttu-id="be4c2-173">String</span><span class="sxs-lookup"><span data-stu-id="be4c2-173">String</span></span>|<span data-ttu-id="be4c2-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="be4c2-174">The name of the app.</span></span> <span data-ttu-id="be4c2-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="be4c2-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="be4c2-176">notes</span><span class="sxs-lookup"><span data-stu-id="be4c2-176">notes</span></span>|<span data-ttu-id="be4c2-177">String</span><span class="sxs-lookup"><span data-stu-id="be4c2-177">String</span></span>|<span data-ttu-id="be4c2-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="be4c2-178">Notes for the app.</span></span> <span data-ttu-id="be4c2-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="be4c2-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="be4c2-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="be4c2-180">publishingState</span></span>|<span data-ttu-id="be4c2-181">String</span><span class="sxs-lookup"><span data-stu-id="be4c2-181">String</span></span>|<span data-ttu-id="be4c2-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="be4c2-182">The publishing state for the app.</span></span> <span data-ttu-id="be4c2-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="be4c2-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="be4c2-184">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="be4c2-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="be4c2-185">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="be4c2-185">usedLicenseCount</span></span>|<span data-ttu-id="be4c2-186">Int32</span><span class="sxs-lookup"><span data-stu-id="be4c2-186">Int32</span></span>|<span data-ttu-id="be4c2-187">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="be4c2-187">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="be4c2-188">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="be4c2-188">totalLicenseCount</span></span>|<span data-ttu-id="be4c2-189">Int32</span><span class="sxs-lookup"><span data-stu-id="be4c2-189">Int32</span></span>|<span data-ttu-id="be4c2-190">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="be4c2-190">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="be4c2-191">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="be4c2-191">releaseDateTime</span></span>|<span data-ttu-id="be4c2-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be4c2-192">DateTimeOffset</span></span>|<span data-ttu-id="be4c2-193">VPP 应用程序的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="be4c2-193">The VPP application release date and time.</span></span>|
|<span data-ttu-id="be4c2-194">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="be4c2-194">appStoreUrl</span></span>|<span data-ttu-id="be4c2-195">String</span><span class="sxs-lookup"><span data-stu-id="be4c2-195">String</span></span>|<span data-ttu-id="be4c2-196">存储 URL。</span><span class="sxs-lookup"><span data-stu-id="be4c2-196">The store URL.</span></span>|
|<span data-ttu-id="be4c2-197">licensingType</span><span class="sxs-lookup"><span data-stu-id="be4c2-197">licensingType</span></span>|[<span data-ttu-id="be4c2-198">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="be4c2-198">vppLicensingType</span></span>](../resources/intune_apps_vpplicensingtype.md)|<span data-ttu-id="be4c2-199">受支持的许可证类型。</span><span class="sxs-lookup"><span data-stu-id="be4c2-199">The supported License Type.</span></span>|
|<span data-ttu-id="be4c2-200">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="be4c2-200">applicableDeviceType</span></span>|[<span data-ttu-id="be4c2-201">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="be4c2-201">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="be4c2-202">适用的 iOS 设备类型。</span><span class="sxs-lookup"><span data-stu-id="be4c2-202">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="be4c2-203">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="be4c2-203">vppTokenOrganizationName</span></span>|<span data-ttu-id="be4c2-204">String</span><span class="sxs-lookup"><span data-stu-id="be4c2-204">String</span></span>|<span data-ttu-id="be4c2-205">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="be4c2-205">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="be4c2-206">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="be4c2-206">vppTokenAccountType</span></span>|<span data-ttu-id="be4c2-207">String</span><span class="sxs-lookup"><span data-stu-id="be4c2-207">String</span></span>|<span data-ttu-id="be4c2-208">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="be4c2-208">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="be4c2-209">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="be4c2-209">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="be4c2-210">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="be4c2-210">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="be4c2-211">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="be4c2-211">vppTokenAppleId</span></span>|<span data-ttu-id="be4c2-212">String</span><span class="sxs-lookup"><span data-stu-id="be4c2-212">String</span></span>|<span data-ttu-id="be4c2-213">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="be4c2-213">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="be4c2-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="be4c2-214">bundleId</span></span>|<span data-ttu-id="be4c2-215">String</span><span class="sxs-lookup"><span data-stu-id="be4c2-215">String</span></span>|<span data-ttu-id="be4c2-216">标识名称。</span><span class="sxs-lookup"><span data-stu-id="be4c2-216">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="be4c2-217">响应</span><span class="sxs-lookup"><span data-stu-id="be4c2-217">Response</span></span>
<span data-ttu-id="be4c2-218">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppApp](../resources/intune_apps_iosvppapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be4c2-218">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be4c2-219">示例</span><span class="sxs-lookup"><span data-stu-id="be4c2-219">Example</span></span>
### <a name="request"></a><span data-ttu-id="be4c2-220">请求</span><span class="sxs-lookup"><span data-stu-id="be4c2-220">Request</span></span>
<span data-ttu-id="be4c2-221">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="be4c2-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1238

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

### <a name="response"></a><span data-ttu-id="be4c2-222">响应</span><span class="sxs-lookup"><span data-stu-id="be4c2-222">Response</span></span>
<span data-ttu-id="be4c2-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="be4c2-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



