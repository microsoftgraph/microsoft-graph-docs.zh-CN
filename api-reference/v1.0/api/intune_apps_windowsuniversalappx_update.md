# <a name="update-windowsuniversalappx"></a><span data-ttu-id="da7e6-101">更新 windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="da7e6-101">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="da7e6-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="da7e6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da7e6-103">更新 [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="da7e6-103">Update the properties of a [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da7e6-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="da7e6-104">Prerequisites</span></span>
<span data-ttu-id="da7e6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="da7e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="da7e6-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="da7e6-107">Permission type</span></span>|<span data-ttu-id="da7e6-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="da7e6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da7e6-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da7e6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="da7e6-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da7e6-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="da7e6-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da7e6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da7e6-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="da7e6-112">Not supported.</span></span>|
|<span data-ttu-id="da7e6-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="da7e6-113">Application</span></span>|<span data-ttu-id="da7e6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="da7e6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da7e6-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da7e6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="da7e6-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="da7e6-116">Request headers</span></span>
|<span data-ttu-id="da7e6-117">标头</span><span class="sxs-lookup"><span data-stu-id="da7e6-117">Header</span></span>|<span data-ttu-id="da7e6-118">值</span><span class="sxs-lookup"><span data-stu-id="da7e6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da7e6-119">授权</span><span class="sxs-lookup"><span data-stu-id="da7e6-119">Authorization</span></span>|<span data-ttu-id="da7e6-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da7e6-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da7e6-121">接受</span><span class="sxs-lookup"><span data-stu-id="da7e6-121">Accept</span></span>|<span data-ttu-id="da7e6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="da7e6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da7e6-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="da7e6-123">Request body</span></span>
<span data-ttu-id="da7e6-124">在请求正文中，提供 [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da7e6-124">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="da7e6-125">下表显示创建 [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="da7e6-125">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span></span>

|<span data-ttu-id="da7e6-126">属性</span><span class="sxs-lookup"><span data-stu-id="da7e6-126">Property</span></span>|<span data-ttu-id="da7e6-127">类型</span><span class="sxs-lookup"><span data-stu-id="da7e6-127">Type</span></span>|<span data-ttu-id="da7e6-128">说明</span><span class="sxs-lookup"><span data-stu-id="da7e6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da7e6-129">id</span><span class="sxs-lookup"><span data-stu-id="da7e6-129">id</span></span>|<span data-ttu-id="da7e6-130">字符串</span><span class="sxs-lookup"><span data-stu-id="da7e6-130">String</span></span>|<span data-ttu-id="da7e6-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="da7e6-131">Key of the entity.</span></span> <span data-ttu-id="da7e6-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da7e6-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da7e6-133">displayName</span><span class="sxs-lookup"><span data-stu-id="da7e6-133">displayName</span></span>|<span data-ttu-id="da7e6-134">String</span><span class="sxs-lookup"><span data-stu-id="da7e6-134">String</span></span>|<span data-ttu-id="da7e6-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="da7e6-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="da7e6-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da7e6-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da7e6-137">description</span><span class="sxs-lookup"><span data-stu-id="da7e6-137">description</span></span>|<span data-ttu-id="da7e6-138">String</span><span class="sxs-lookup"><span data-stu-id="da7e6-138">String</span></span>|<span data-ttu-id="da7e6-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="da7e6-139">The description of the app.</span></span> <span data-ttu-id="da7e6-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da7e6-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da7e6-141">publisher</span><span class="sxs-lookup"><span data-stu-id="da7e6-141">publisher</span></span>|<span data-ttu-id="da7e6-142">String</span><span class="sxs-lookup"><span data-stu-id="da7e6-142">String</span></span>|<span data-ttu-id="da7e6-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="da7e6-143">The publisher of the app.</span></span> <span data-ttu-id="da7e6-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da7e6-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da7e6-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="da7e6-145">largeIcon</span></span>|[<span data-ttu-id="da7e6-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="da7e6-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="da7e6-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="da7e6-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="da7e6-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da7e6-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da7e6-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da7e6-149">createdDateTime</span></span>|<span data-ttu-id="da7e6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da7e6-150">DateTimeOffset</span></span>|<span data-ttu-id="da7e6-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="da7e6-151">The date and time the app was created.</span></span> <span data-ttu-id="da7e6-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da7e6-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da7e6-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da7e6-153">lastModifiedDateTime</span></span>|<span data-ttu-id="da7e6-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da7e6-154">DateTimeOffset</span></span>|<span data-ttu-id="da7e6-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="da7e6-155">The date and time the app was last modified.</span></span> <span data-ttu-id="da7e6-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da7e6-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da7e6-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="da7e6-157">isFeatured</span></span>|<span data-ttu-id="da7e6-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="da7e6-158">Boolean</span></span>|<span data-ttu-id="da7e6-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da7e6-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da7e6-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="da7e6-160">privacyInformationUrl</span></span>|<span data-ttu-id="da7e6-161">String</span><span class="sxs-lookup"><span data-stu-id="da7e6-161">String</span></span>|<span data-ttu-id="da7e6-162">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="da7e6-162">The privacy statement Url.</span></span> <span data-ttu-id="da7e6-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da7e6-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da7e6-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="da7e6-164">informationUrl</span></span>|<span data-ttu-id="da7e6-165">String</span><span class="sxs-lookup"><span data-stu-id="da7e6-165">String</span></span>|<span data-ttu-id="da7e6-166">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="da7e6-166">The more information Url.</span></span> <span data-ttu-id="da7e6-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da7e6-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da7e6-168">owner</span><span class="sxs-lookup"><span data-stu-id="da7e6-168">owner</span></span>|<span data-ttu-id="da7e6-169">String</span><span class="sxs-lookup"><span data-stu-id="da7e6-169">String</span></span>|<span data-ttu-id="da7e6-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="da7e6-170">The owner of the app.</span></span> <span data-ttu-id="da7e6-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da7e6-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da7e6-172">developer</span><span class="sxs-lookup"><span data-stu-id="da7e6-172">developer</span></span>|<span data-ttu-id="da7e6-173">String</span><span class="sxs-lookup"><span data-stu-id="da7e6-173">String</span></span>|<span data-ttu-id="da7e6-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="da7e6-174">The developer of the app.</span></span> <span data-ttu-id="da7e6-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da7e6-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da7e6-176">notes</span><span class="sxs-lookup"><span data-stu-id="da7e6-176">notes</span></span>|<span data-ttu-id="da7e6-177">String</span><span class="sxs-lookup"><span data-stu-id="da7e6-177">String</span></span>|<span data-ttu-id="da7e6-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="da7e6-178">Notes for the app.</span></span> <span data-ttu-id="da7e6-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da7e6-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="da7e6-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="da7e6-180">publishingState</span></span>|[<span data-ttu-id="da7e6-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="da7e6-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="da7e6-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="da7e6-182">The publishing state for the app.</span></span> <span data-ttu-id="da7e6-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="da7e6-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="da7e6-184">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="da7e6-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="da7e6-185">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="da7e6-185">The possible values are `notPublished`, `processing`, `published`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="da7e6-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="da7e6-186">committedContentVersion</span></span>|<span data-ttu-id="da7e6-187">String</span><span class="sxs-lookup"><span data-stu-id="da7e6-187">String</span></span>|<span data-ttu-id="da7e6-188">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="da7e6-188">The internal committed content version.</span></span> <span data-ttu-id="da7e6-189">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="da7e6-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="da7e6-190">fileName</span><span class="sxs-lookup"><span data-stu-id="da7e6-190">fileName</span></span>|<span data-ttu-id="da7e6-191">String</span><span class="sxs-lookup"><span data-stu-id="da7e6-191">String</span></span>|<span data-ttu-id="da7e6-192">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="da7e6-192">The name of the main Lob application file.</span></span> <span data-ttu-id="da7e6-193">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="da7e6-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="da7e6-194">size</span><span class="sxs-lookup"><span data-stu-id="da7e6-194">size</span></span>|<span data-ttu-id="da7e6-195">Int64</span><span class="sxs-lookup"><span data-stu-id="da7e6-195">Int64</span></span>|<span data-ttu-id="da7e6-196">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="da7e6-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="da7e6-197">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="da7e6-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="da7e6-198">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="da7e6-198">applicableArchitectures</span></span>|[<span data-ttu-id="da7e6-199">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="da7e6-199">windowsArchitecture</span></span>](../resources/intune_apps_windowsarchitecture.md)|<span data-ttu-id="da7e6-200">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="da7e6-200">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="da7e6-201">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。</span><span class="sxs-lookup"><span data-stu-id="da7e6-201">The possible values are `none`, `x86`, `x64`, `arm`, `neutral`, , , , , , , or .</span></span>|
|<span data-ttu-id="da7e6-202">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="da7e6-202">applicableDeviceTypes</span></span>|[<span data-ttu-id="da7e6-203">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="da7e6-203">windowsDeviceType</span></span>](../resources/intune_apps_windowsdevicetype.md)|<span data-ttu-id="da7e6-204">可运行此应用的 Windows 设备类型。</span><span class="sxs-lookup"><span data-stu-id="da7e6-204">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="da7e6-205">可取值为：`none`、`desktop`、`mobile`、`holographic`、`team`。</span><span class="sxs-lookup"><span data-stu-id="da7e6-205">The possible values are `none`, `desktop`, `mobile`, `holographic`, `team`, , , , , , , or .</span></span>|
|<span data-ttu-id="da7e6-206">identityName</span><span class="sxs-lookup"><span data-stu-id="da7e6-206">identityName</span></span>|<span data-ttu-id="da7e6-207">String</span><span class="sxs-lookup"><span data-stu-id="da7e6-207">String</span></span>|<span data-ttu-id="da7e6-208">标识名称。</span><span class="sxs-lookup"><span data-stu-id="da7e6-208">The Identity Name.</span></span>|
|<span data-ttu-id="da7e6-209">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="da7e6-209">identityPublisherHash</span></span>|<span data-ttu-id="da7e6-210">String</span><span class="sxs-lookup"><span data-stu-id="da7e6-210">String</span></span>|<span data-ttu-id="da7e6-211">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="da7e6-211">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="da7e6-212">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="da7e6-212">identityResourceIdentifier</span></span>|<span data-ttu-id="da7e6-213">String</span><span class="sxs-lookup"><span data-stu-id="da7e6-213">String</span></span>|<span data-ttu-id="da7e6-214">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="da7e6-214">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="da7e6-215">isBundle</span><span class="sxs-lookup"><span data-stu-id="da7e6-215">isBundle</span></span>|<span data-ttu-id="da7e6-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="da7e6-216">Boolean</span></span>|<span data-ttu-id="da7e6-217">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="da7e6-217">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="da7e6-218">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="da7e6-218">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="da7e6-219">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="da7e6-219">windowsMinimumOperatingSystem</span></span>](../resources/intune_apps_windowsminimumoperatingsystem.md)|<span data-ttu-id="da7e6-220">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="da7e6-220">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="da7e6-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="da7e6-221">identityVersion</span></span>|<span data-ttu-id="da7e6-222">String</span><span class="sxs-lookup"><span data-stu-id="da7e6-222">String</span></span>|<span data-ttu-id="da7e6-223">标识版本。</span><span class="sxs-lookup"><span data-stu-id="da7e6-223">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="da7e6-224">响应</span><span class="sxs-lookup"><span data-stu-id="da7e6-224">Response</span></span>
<span data-ttu-id="da7e6-225">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="da7e6-225">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da7e6-226">示例</span><span class="sxs-lookup"><span data-stu-id="da7e6-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="da7e6-227">请求</span><span class="sxs-lookup"><span data-stu-id="da7e6-227">Request</span></span>
<span data-ttu-id="da7e6-228">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da7e6-228">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="da7e6-229">响应</span><span class="sxs-lookup"><span data-stu-id="da7e6-229">Response</span></span>
<span data-ttu-id="da7e6-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da7e6-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



