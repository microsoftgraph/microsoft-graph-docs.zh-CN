# <a name="create-iosvppebook"></a><span data-ttu-id="78029-101">创建 iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="78029-101">Create iosVppEBook</span></span>

> <span data-ttu-id="78029-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="78029-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78029-103">创建新的 [iosVppEBook](../resources/intune_books_iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78029-103">Create a new [iosVppEBook](../resources/intune_books_iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="78029-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="78029-104">Prerequisites</span></span>
<span data-ttu-id="78029-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="78029-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="78029-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="78029-107">Permission type</span></span>|<span data-ttu-id="78029-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="78029-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78029-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78029-109">Delegated (work or school account)</span></span>|<span data-ttu-id="78029-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78029-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="78029-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78029-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78029-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="78029-112">Not supported.</span></span>|
|<span data-ttu-id="78029-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="78029-113">Application</span></span>|<span data-ttu-id="78029-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="78029-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78029-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78029-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="78029-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="78029-116">Request headers</span></span>
|<span data-ttu-id="78029-117">标头</span><span class="sxs-lookup"><span data-stu-id="78029-117">Header</span></span>|<span data-ttu-id="78029-118">值</span><span class="sxs-lookup"><span data-stu-id="78029-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78029-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="78029-119">Authorization</span></span>|<span data-ttu-id="78029-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="78029-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78029-121">Accept</span><span class="sxs-lookup"><span data-stu-id="78029-121">Accept</span></span>|<span data-ttu-id="78029-122">application/json</span><span class="sxs-lookup"><span data-stu-id="78029-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78029-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="78029-123">Request body</span></span>
<span data-ttu-id="78029-124">在请求正文中，提供 iosVppEBook 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78029-124">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="78029-125">下表显示了创建 iosVppEBook 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="78029-125">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="78029-126">属性</span><span class="sxs-lookup"><span data-stu-id="78029-126">Property</span></span>|<span data-ttu-id="78029-127">类型</span><span class="sxs-lookup"><span data-stu-id="78029-127">Type</span></span>|<span data-ttu-id="78029-128">说明</span><span class="sxs-lookup"><span data-stu-id="78029-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78029-129">id</span><span class="sxs-lookup"><span data-stu-id="78029-129">id</span></span>|<span data-ttu-id="78029-130">String</span><span class="sxs-lookup"><span data-stu-id="78029-130">String</span></span>|<span data-ttu-id="78029-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="78029-131">Key of the entity.</span></span> <span data-ttu-id="78029-132">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="78029-132">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="78029-133">displayName</span><span class="sxs-lookup"><span data-stu-id="78029-133">displayName</span></span>|<span data-ttu-id="78029-134">String</span><span class="sxs-lookup"><span data-stu-id="78029-134">String</span></span>|<span data-ttu-id="78029-135">电子图书的名称。</span><span class="sxs-lookup"><span data-stu-id="78029-135">Name of the eBook.</span></span> <span data-ttu-id="78029-136">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="78029-136">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="78029-137">description</span><span class="sxs-lookup"><span data-stu-id="78029-137">description</span></span>|<span data-ttu-id="78029-138">String</span><span class="sxs-lookup"><span data-stu-id="78029-138">String</span></span>|<span data-ttu-id="78029-139">说明。</span><span class="sxs-lookup"><span data-stu-id="78029-139">Description.</span></span> <span data-ttu-id="78029-140">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="78029-140">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="78029-141">publisher</span><span class="sxs-lookup"><span data-stu-id="78029-141">publisher</span></span>|<span data-ttu-id="78029-142">String</span><span class="sxs-lookup"><span data-stu-id="78029-142">String</span></span>|<span data-ttu-id="78029-143">发布者。</span><span class="sxs-lookup"><span data-stu-id="78029-143">Publisher.</span></span> <span data-ttu-id="78029-144">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="78029-144">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="78029-145">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="78029-145">publishedDateTime</span></span>|<span data-ttu-id="78029-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78029-146">DateTimeOffset</span></span>|<span data-ttu-id="78029-147">电子图书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="78029-147">The date and time when the eBook was published.</span></span> <span data-ttu-id="78029-148">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="78029-148">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="78029-149">largeCover</span><span class="sxs-lookup"><span data-stu-id="78029-149">largeCover</span></span>|[<span data-ttu-id="78029-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="78029-150">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="78029-151">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="78029-151">Book cover.</span></span> <span data-ttu-id="78029-152">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="78029-152">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="78029-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78029-153">createdDateTime</span></span>|<span data-ttu-id="78029-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78029-154">DateTimeOffset</span></span>|<span data-ttu-id="78029-155">电子图书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="78029-155">The date and time when the eBook file was created.</span></span> <span data-ttu-id="78029-156">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="78029-156">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="78029-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78029-157">lastModifiedDateTime</span></span>|<span data-ttu-id="78029-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78029-158">DateTimeOffset</span></span>|<span data-ttu-id="78029-159">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="78029-159">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="78029-160">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="78029-160">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="78029-161">informationUrl</span><span class="sxs-lookup"><span data-stu-id="78029-161">informationUrl</span></span>|<span data-ttu-id="78029-162">String</span><span class="sxs-lookup"><span data-stu-id="78029-162">String</span></span>|<span data-ttu-id="78029-163">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="78029-163">The more information Url.</span></span> <span data-ttu-id="78029-164">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="78029-164">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="78029-165">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="78029-165">privacyInformationUrl</span></span>|<span data-ttu-id="78029-166">String</span><span class="sxs-lookup"><span data-stu-id="78029-166">String</span></span>|<span data-ttu-id="78029-167">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="78029-167">The privacy statement Url.</span></span> <span data-ttu-id="78029-168">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="78029-168">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="78029-169">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="78029-169">vppTokenId</span></span>|<span data-ttu-id="78029-170">Guid</span><span class="sxs-lookup"><span data-stu-id="78029-170">Guid</span></span>|<span data-ttu-id="78029-171">Vpp 令牌 ID。</span><span class="sxs-lookup"><span data-stu-id="78029-171">The Vpp token ID.</span></span>|
|<span data-ttu-id="78029-172">appleId</span><span class="sxs-lookup"><span data-stu-id="78029-172">appleId</span></span>|<span data-ttu-id="78029-173">String</span><span class="sxs-lookup"><span data-stu-id="78029-173">String</span></span>|<span data-ttu-id="78029-174">与 Vpp 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="78029-174">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="78029-175">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="78029-175">vppOrganizationName</span></span>|<span data-ttu-id="78029-176">String</span><span class="sxs-lookup"><span data-stu-id="78029-176">String</span></span>|<span data-ttu-id="78029-177">Vpp 令牌的组织名称。</span><span class="sxs-lookup"><span data-stu-id="78029-177">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="78029-178">genres</span><span class="sxs-lookup"><span data-stu-id="78029-178">genres</span></span>|<span data-ttu-id="78029-179">String 集合</span><span class="sxs-lookup"><span data-stu-id="78029-179">String collection</span></span>|<span data-ttu-id="78029-180">流派。</span><span class="sxs-lookup"><span data-stu-id="78029-180">Genres.</span></span>|
|<span data-ttu-id="78029-181">language</span><span class="sxs-lookup"><span data-stu-id="78029-181">language</span></span>|<span data-ttu-id="78029-182">String</span><span class="sxs-lookup"><span data-stu-id="78029-182">String</span></span>|<span data-ttu-id="78029-183">语言。</span><span class="sxs-lookup"><span data-stu-id="78029-183">Language.</span></span>|
|<span data-ttu-id="78029-184">seller</span><span class="sxs-lookup"><span data-stu-id="78029-184">seller</span></span>|<span data-ttu-id="78029-185">String</span><span class="sxs-lookup"><span data-stu-id="78029-185">String</span></span>|<span data-ttu-id="78029-186">经销商。</span><span class="sxs-lookup"><span data-stu-id="78029-186">Seller.</span></span>|
|<span data-ttu-id="78029-187">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="78029-187">totalLicenseCount</span></span>|<span data-ttu-id="78029-188">Int32</span><span class="sxs-lookup"><span data-stu-id="78029-188">Int32</span></span>|<span data-ttu-id="78029-189">许可证总数。</span><span class="sxs-lookup"><span data-stu-id="78029-189">Total license count.</span></span>|
|<span data-ttu-id="78029-190">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="78029-190">usedLicenseCount</span></span>|<span data-ttu-id="78029-191">Int32</span><span class="sxs-lookup"><span data-stu-id="78029-191">Int32</span></span>|<span data-ttu-id="78029-192">使用的许可证数。</span><span class="sxs-lookup"><span data-stu-id="78029-192">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="78029-193">响应</span><span class="sxs-lookup"><span data-stu-id="78029-193">Response</span></span>
<span data-ttu-id="78029-194">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosVppEBook](../resources/intune_books_iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78029-194">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune_books_iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78029-195">示例</span><span class="sxs-lookup"><span data-stu-id="78029-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="78029-196">请求</span><span class="sxs-lookup"><span data-stu-id="78029-196">Request</span></span>
<span data-ttu-id="78029-197">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="78029-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
Content-type: application/json
Content-length: 792

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```

### <a name="response"></a><span data-ttu-id="78029-198">响应</span><span class="sxs-lookup"><span data-stu-id="78029-198">Response</span></span>
<span data-ttu-id="78029-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="78029-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 964

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```



