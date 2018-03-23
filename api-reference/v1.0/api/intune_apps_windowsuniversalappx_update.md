# <a name="update-windowsuniversalappx"></a><span data-ttu-id="c59d2-101">更新 windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="c59d2-101">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="c59d2-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c59d2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c59d2-103">更新 [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c59d2-103">Update the properties of a [calendar](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c59d2-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="c59d2-104">Prerequisites</span></span>
<span data-ttu-id="c59d2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c59d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c59d2-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="c59d2-107">Permission type</span></span>|<span data-ttu-id="c59d2-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c59d2-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c59d2-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c59d2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c59d2-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c59d2-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c59d2-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c59d2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c59d2-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="c59d2-112">Not supported.</span></span>|
|<span data-ttu-id="c59d2-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="c59d2-113">Application</span></span>|<span data-ttu-id="c59d2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c59d2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c59d2-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c59d2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="c59d2-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="c59d2-116">Request headers</span></span>
|<span data-ttu-id="c59d2-117">标头</span><span class="sxs-lookup"><span data-stu-id="c59d2-117">Header</span></span>|<span data-ttu-id="c59d2-118">值</span><span class="sxs-lookup"><span data-stu-id="c59d2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c59d2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c59d2-119">Authorization</span></span>|<span data-ttu-id="c59d2-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c59d2-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c59d2-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c59d2-121">Accept</span></span>|<span data-ttu-id="c59d2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c59d2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c59d2-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c59d2-123">Request body</span></span>
<span data-ttu-id="c59d2-124">在请求正文中，提供 [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c59d2-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="c59d2-125">下表显示创建 [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c59d2-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="c59d2-126">属性</span><span class="sxs-lookup"><span data-stu-id="c59d2-126">Property</span></span>|<span data-ttu-id="c59d2-127">类型</span><span class="sxs-lookup"><span data-stu-id="c59d2-127">Type</span></span>|<span data-ttu-id="c59d2-128">说明</span><span class="sxs-lookup"><span data-stu-id="c59d2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c59d2-129">id</span><span class="sxs-lookup"><span data-stu-id="c59d2-129">id</span></span>|<span data-ttu-id="c59d2-130">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-130">String</span></span>|<span data-ttu-id="c59d2-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c59d2-131">Key of the setting.</span></span> <span data-ttu-id="c59d2-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c59d2-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c59d2-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c59d2-133">displayName</span></span>|<span data-ttu-id="c59d2-134">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-134">String</span></span>|<span data-ttu-id="c59d2-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="c59d2-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c59d2-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c59d2-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c59d2-137">description</span><span class="sxs-lookup"><span data-stu-id="c59d2-137">description</span></span>|<span data-ttu-id="c59d2-138">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-138">String</span></span>|<span data-ttu-id="c59d2-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="c59d2-139">The description of the app.</span></span> <span data-ttu-id="c59d2-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c59d2-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c59d2-141">publisher</span><span class="sxs-lookup"><span data-stu-id="c59d2-141">Publisher</span></span>|<span data-ttu-id="c59d2-142">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-142">String</span></span>|<span data-ttu-id="c59d2-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="c59d2-143">The name of the app.</span></span> <span data-ttu-id="c59d2-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c59d2-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c59d2-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c59d2-145">largeIcon</span></span>|[<span data-ttu-id="c59d2-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c59d2-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="c59d2-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="c59d2-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c59d2-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c59d2-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c59d2-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c59d2-149">createdDateTime</span></span>|<span data-ttu-id="c59d2-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c59d2-150">DateTimeOffset</span></span>|<span data-ttu-id="c59d2-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c59d2-151">The date and time when the page was created.</span></span> <span data-ttu-id="c59d2-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c59d2-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c59d2-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c59d2-153">lastModifiedDateTime</span></span>|<span data-ttu-id="c59d2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c59d2-154">DateTimeOffset</span></span>|<span data-ttu-id="c59d2-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c59d2-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="c59d2-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c59d2-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c59d2-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c59d2-157">isFeatured</span></span>|<span data-ttu-id="c59d2-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="c59d2-158">Boolean</span></span>|<span data-ttu-id="c59d2-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c59d2-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c59d2-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c59d2-160">privacyInformationUrl</span></span>|<span data-ttu-id="c59d2-161">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-161">String</span></span>|<span data-ttu-id="c59d2-162">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="c59d2-162">The privacy statement Url.</span></span> <span data-ttu-id="c59d2-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c59d2-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c59d2-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c59d2-164">informationUrl</span></span>|<span data-ttu-id="c59d2-165">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-165">String</span></span>|<span data-ttu-id="c59d2-166">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="c59d2-166">The more information Url.</span></span> <span data-ttu-id="c59d2-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c59d2-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c59d2-168">owner</span><span class="sxs-lookup"><span data-stu-id="c59d2-168">owner</span></span>|<span data-ttu-id="c59d2-169">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-169">String</span></span>|<span data-ttu-id="c59d2-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="c59d2-170">The owner of the timesheet.</span></span> <span data-ttu-id="c59d2-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c59d2-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c59d2-172">developer</span><span class="sxs-lookup"><span data-stu-id="c59d2-172">developer</span></span>|<span data-ttu-id="c59d2-173">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-173">String</span></span>|<span data-ttu-id="c59d2-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="c59d2-174">The name of the app.</span></span> <span data-ttu-id="c59d2-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c59d2-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c59d2-176">notes</span><span class="sxs-lookup"><span data-stu-id="c59d2-176">notes</span></span>|<span data-ttu-id="c59d2-177">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-177">String</span></span>|<span data-ttu-id="c59d2-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="c59d2-178">Notes for the app.</span></span> <span data-ttu-id="c59d2-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c59d2-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c59d2-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="c59d2-180">publishingState</span></span>|<span data-ttu-id="c59d2-181">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-181">String</span></span>|<span data-ttu-id="c59d2-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="c59d2-182">The publishing state for the app.</span></span> <span data-ttu-id="c59d2-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="c59d2-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c59d2-184">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="c59d2-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c59d2-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="c59d2-185">committedContentVersion</span></span>|<span data-ttu-id="c59d2-186">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-186">String</span></span>|<span data-ttu-id="c59d2-187">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="c59d2-187">The internal committed content version.</span></span> <span data-ttu-id="c59d2-188">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c59d2-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="c59d2-189">fileName</span><span class="sxs-lookup"><span data-stu-id="c59d2-189">fileName</span></span>|<span data-ttu-id="c59d2-190">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-190">String</span></span>|<span data-ttu-id="c59d2-191">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="c59d2-191">The name of the main Lob application file.</span></span> <span data-ttu-id="c59d2-192">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c59d2-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="c59d2-193">size</span><span class="sxs-lookup"><span data-stu-id="c59d2-193">size</span></span>|<span data-ttu-id="c59d2-194">Int64</span><span class="sxs-lookup"><span data-stu-id="c59d2-194">Int64</span></span>|<span data-ttu-id="c59d2-195">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="c59d2-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="c59d2-196">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c59d2-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="c59d2-197">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="c59d2-197">applicableArchitectures</span></span>|<span data-ttu-id="c59d2-198">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-198">String</span></span>|<span data-ttu-id="c59d2-199">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="c59d2-199">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="c59d2-200">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。</span><span class="sxs-lookup"><span data-stu-id="c59d2-200">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="c59d2-201">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="c59d2-201">applicableDeviceTypes</span></span>|<span data-ttu-id="c59d2-202">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-202">String</span></span>|<span data-ttu-id="c59d2-203">可运行此应用的 Windows 设备类型。</span><span class="sxs-lookup"><span data-stu-id="c59d2-203">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="c59d2-204">可取值为：`none`、`desktop`、`mobile`、`holographic`、`team`。</span><span class="sxs-lookup"><span data-stu-id="c59d2-204">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="c59d2-205">identityName</span><span class="sxs-lookup"><span data-stu-id="c59d2-205">identityName</span></span>|<span data-ttu-id="c59d2-206">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-206">String</span></span>|<span data-ttu-id="c59d2-207">标识名称。</span><span class="sxs-lookup"><span data-stu-id="c59d2-207">The Identity Name.</span></span>|
|<span data-ttu-id="c59d2-208">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="c59d2-208">identityPublisherHash</span></span>|<span data-ttu-id="c59d2-209">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-209">String</span></span>|<span data-ttu-id="c59d2-210">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="c59d2-210">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="c59d2-211">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="c59d2-211">identityResourceIdentifier</span></span>|<span data-ttu-id="c59d2-212">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-212">String</span></span>|<span data-ttu-id="c59d2-213">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="c59d2-213">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="c59d2-214">isBundle</span><span class="sxs-lookup"><span data-stu-id="c59d2-214">isBundle</span></span>|<span data-ttu-id="c59d2-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="c59d2-215">Boolean</span></span>|<span data-ttu-id="c59d2-216">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="c59d2-216">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="c59d2-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c59d2-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c59d2-218">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c59d2-218">windowsMinimumOperatingSystem</span></span>](../resources/intune_apps_windowsminimumoperatingsystem.md)|<span data-ttu-id="c59d2-219">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="c59d2-219">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="c59d2-220">identityVersion</span><span class="sxs-lookup"><span data-stu-id="c59d2-220">identityVersion</span></span>|<span data-ttu-id="c59d2-221">String</span><span class="sxs-lookup"><span data-stu-id="c59d2-221">String</span></span>|<span data-ttu-id="c59d2-222">标识版本。</span><span class="sxs-lookup"><span data-stu-id="c59d2-222">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="c59d2-223">响应</span><span class="sxs-lookup"><span data-stu-id="c59d2-223">Response</span></span>
<span data-ttu-id="c59d2-224">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c59d2-224">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c59d2-225">示例</span><span class="sxs-lookup"><span data-stu-id="c59d2-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="c59d2-226">请求</span><span class="sxs-lookup"><span data-stu-id="c59d2-226">Request</span></span>
<span data-ttu-id="c59d2-227">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c59d2-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1194

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
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="c59d2-228">响应</span><span class="sxs-lookup"><span data-stu-id="c59d2-228">Response</span></span>
<span data-ttu-id="c59d2-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c59d2-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```



