# <a name="update-iosvppebook"></a><span data-ttu-id="268fd-101">更新 iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="268fd-101">Update iosVppEBook</span></span>

> <span data-ttu-id="268fd-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="268fd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="268fd-103">更新 [iosVppEBook](../resources/intune_books_iosvppebook.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="268fd-103">Update the properties of a [iosVppEBook](../resources/intune_books_iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="268fd-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="268fd-104">Prerequisites</span></span>
<span data-ttu-id="268fd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="268fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="268fd-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="268fd-107">Permission type</span></span>|<span data-ttu-id="268fd-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="268fd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="268fd-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="268fd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="268fd-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="268fd-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="268fd-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="268fd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="268fd-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="268fd-112">Not supported.</span></span>|
|<span data-ttu-id="268fd-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="268fd-113">Application</span></span>|<span data-ttu-id="268fd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="268fd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="268fd-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="268fd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="268fd-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="268fd-116">Request headers</span></span>
|<span data-ttu-id="268fd-117">标头</span><span class="sxs-lookup"><span data-stu-id="268fd-117">Header</span></span>|<span data-ttu-id="268fd-118">值</span><span class="sxs-lookup"><span data-stu-id="268fd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="268fd-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="268fd-119">Authorization</span></span>|<span data-ttu-id="268fd-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="268fd-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="268fd-121">Accept</span><span class="sxs-lookup"><span data-stu-id="268fd-121">Accept</span></span>|<span data-ttu-id="268fd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="268fd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="268fd-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="268fd-123">Request body</span></span>
<span data-ttu-id="268fd-124">在请求正文中，提供 [iosVppEBook](../resources/intune_books_iosvppebook.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="268fd-124">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune_books_iosvppebook.md) object.</span></span>

<span data-ttu-id="268fd-125">下表显示了创建 [iosVppEBook](../resources/intune_books_iosvppebook.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="268fd-125">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune_books_iosvppebook.md).</span></span>

|<span data-ttu-id="268fd-126">属性</span><span class="sxs-lookup"><span data-stu-id="268fd-126">Property</span></span>|<span data-ttu-id="268fd-127">类型</span><span class="sxs-lookup"><span data-stu-id="268fd-127">Type</span></span>|<span data-ttu-id="268fd-128">说明</span><span class="sxs-lookup"><span data-stu-id="268fd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="268fd-129">id</span><span class="sxs-lookup"><span data-stu-id="268fd-129">id</span></span>|<span data-ttu-id="268fd-130">String</span><span class="sxs-lookup"><span data-stu-id="268fd-130">String</span></span>|<span data-ttu-id="268fd-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="268fd-131">Key of the entity.</span></span> <span data-ttu-id="268fd-132">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="268fd-132">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="268fd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="268fd-133">displayName</span></span>|<span data-ttu-id="268fd-134">String</span><span class="sxs-lookup"><span data-stu-id="268fd-134">String</span></span>|<span data-ttu-id="268fd-135">电子书的名称。</span><span class="sxs-lookup"><span data-stu-id="268fd-135">Name of the eBook.</span></span> <span data-ttu-id="268fd-136">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="268fd-136">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="268fd-137">description</span><span class="sxs-lookup"><span data-stu-id="268fd-137">description</span></span>|<span data-ttu-id="268fd-138">String</span><span class="sxs-lookup"><span data-stu-id="268fd-138">String</span></span>|<span data-ttu-id="268fd-139">说明。</span><span class="sxs-lookup"><span data-stu-id="268fd-139">Description.</span></span> <span data-ttu-id="268fd-140">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="268fd-140">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="268fd-141">publisher</span><span class="sxs-lookup"><span data-stu-id="268fd-141">publisher</span></span>|<span data-ttu-id="268fd-142">String</span><span class="sxs-lookup"><span data-stu-id="268fd-142">String</span></span>|<span data-ttu-id="268fd-143">发布者。</span><span class="sxs-lookup"><span data-stu-id="268fd-143">Publisher.</span></span> <span data-ttu-id="268fd-144">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="268fd-144">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="268fd-145">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="268fd-145">publishedDateTime</span></span>|<span data-ttu-id="268fd-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="268fd-146">DateTimeOffset</span></span>|<span data-ttu-id="268fd-147">电子书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="268fd-147">The date and time when the eBook was published.</span></span> <span data-ttu-id="268fd-148">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="268fd-148">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="268fd-149">largeCover</span><span class="sxs-lookup"><span data-stu-id="268fd-149">largeCover</span></span>|[<span data-ttu-id="268fd-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="268fd-150">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="268fd-151">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="268fd-151">Book cover.</span></span> <span data-ttu-id="268fd-152">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="268fd-152">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="268fd-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="268fd-153">createdDateTime</span></span>|<span data-ttu-id="268fd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="268fd-154">DateTimeOffset</span></span>|<span data-ttu-id="268fd-155">电子书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="268fd-155">The date and time when the eBook file was created.</span></span> <span data-ttu-id="268fd-156">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="268fd-156">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="268fd-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="268fd-157">lastModifiedDateTime</span></span>|<span data-ttu-id="268fd-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="268fd-158">DateTimeOffset</span></span>|<span data-ttu-id="268fd-159">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="268fd-159">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="268fd-160">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="268fd-160">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="268fd-161">informationUrl</span><span class="sxs-lookup"><span data-stu-id="268fd-161">informationUrl</span></span>|<span data-ttu-id="268fd-162">String</span><span class="sxs-lookup"><span data-stu-id="268fd-162">String</span></span>|<span data-ttu-id="268fd-163">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="268fd-163">The more information Url.</span></span> <span data-ttu-id="268fd-164">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="268fd-164">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="268fd-165">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="268fd-165">privacyInformationUrl</span></span>|<span data-ttu-id="268fd-166">String</span><span class="sxs-lookup"><span data-stu-id="268fd-166">String</span></span>|<span data-ttu-id="268fd-167">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="268fd-167">The privacy statement Url.</span></span> <span data-ttu-id="268fd-168">继承自 [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="268fd-168">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="268fd-169">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="268fd-169">vppTokenId</span></span>|<span data-ttu-id="268fd-170">Guid</span><span class="sxs-lookup"><span data-stu-id="268fd-170">Guid</span></span>|<span data-ttu-id="268fd-171">Vpp 令牌 ID。</span><span class="sxs-lookup"><span data-stu-id="268fd-171">The Vpp token ID.</span></span>|
|<span data-ttu-id="268fd-172">appleId</span><span class="sxs-lookup"><span data-stu-id="268fd-172">appleId</span></span>|<span data-ttu-id="268fd-173">String</span><span class="sxs-lookup"><span data-stu-id="268fd-173">String</span></span>|<span data-ttu-id="268fd-174">与 Vpp 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="268fd-174">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="268fd-175">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="268fd-175">vppOrganizationName</span></span>|<span data-ttu-id="268fd-176">String</span><span class="sxs-lookup"><span data-stu-id="268fd-176">String</span></span>|<span data-ttu-id="268fd-177">Vpp 令牌的组织名称。</span><span class="sxs-lookup"><span data-stu-id="268fd-177">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="268fd-178">genres</span><span class="sxs-lookup"><span data-stu-id="268fd-178">genres</span></span>|<span data-ttu-id="268fd-179">String 集合</span><span class="sxs-lookup"><span data-stu-id="268fd-179">String collection</span></span>|<span data-ttu-id="268fd-180">流派。</span><span class="sxs-lookup"><span data-stu-id="268fd-180">Genres.</span></span>|
|<span data-ttu-id="268fd-181">language</span><span class="sxs-lookup"><span data-stu-id="268fd-181">language</span></span>|<span data-ttu-id="268fd-182">String</span><span class="sxs-lookup"><span data-stu-id="268fd-182">String</span></span>|<span data-ttu-id="268fd-183">语言。</span><span class="sxs-lookup"><span data-stu-id="268fd-183">Language.</span></span>|
|<span data-ttu-id="268fd-184">seller</span><span class="sxs-lookup"><span data-stu-id="268fd-184">seller</span></span>|<span data-ttu-id="268fd-185">String</span><span class="sxs-lookup"><span data-stu-id="268fd-185">String</span></span>|<span data-ttu-id="268fd-186">经销商。</span><span class="sxs-lookup"><span data-stu-id="268fd-186">Seller.</span></span>|
|<span data-ttu-id="268fd-187">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="268fd-187">totalLicenseCount</span></span>|<span data-ttu-id="268fd-188">Int32</span><span class="sxs-lookup"><span data-stu-id="268fd-188">Int32</span></span>|<span data-ttu-id="268fd-189">许可证总数。</span><span class="sxs-lookup"><span data-stu-id="268fd-189">Total license count.</span></span>|
|<span data-ttu-id="268fd-190">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="268fd-190">usedLicenseCount</span></span>|<span data-ttu-id="268fd-191">Int32</span><span class="sxs-lookup"><span data-stu-id="268fd-191">Int32</span></span>|<span data-ttu-id="268fd-192">使用的许可证数。</span><span class="sxs-lookup"><span data-stu-id="268fd-192">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="268fd-193">响应</span><span class="sxs-lookup"><span data-stu-id="268fd-193">Response</span></span>
<span data-ttu-id="268fd-194">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppEBook](../resources/intune_books_iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="268fd-194">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune_books_iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="268fd-195">示例</span><span class="sxs-lookup"><span data-stu-id="268fd-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="268fd-196">请求</span><span class="sxs-lookup"><span data-stu-id="268fd-196">Request</span></span>
<span data-ttu-id="268fd-197">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="268fd-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
Content-type: application/json
Content-length: 803

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "<Unknown Primitive Type Edm.Guid>",
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

### <a name="response"></a><span data-ttu-id="268fd-198">响应</span><span class="sxs-lookup"><span data-stu-id="268fd-198">Response</span></span>
<span data-ttu-id="268fd-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="268fd-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 961

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
  "vppTokenId": "<Unknown Primitive Type Edm.Guid>",
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



