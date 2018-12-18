---
title: 更新 iosVppEBook
description: 更新 iosVppEBook 对象的属性。
author: tfitzmac
ms.openlocfilehash: d73542adf39948979e0287be6a566ae8ddb7f829
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309672"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="f3c47-103">更新 iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="f3c47-103">Update iosVppEBook</span></span>

> <span data-ttu-id="f3c47-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f3c47-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3c47-105">更新 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f3c47-105">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f3c47-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f3c47-106">Prerequisites</span></span>
<span data-ttu-id="f3c47-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f3c47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3c47-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3c47-109">Permission type</span></span>|<span data-ttu-id="f3c47-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f3c47-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3c47-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3c47-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f3c47-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3c47-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f3c47-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3c47-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3c47-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3c47-114">Not supported.</span></span>|
|<span data-ttu-id="f3c47-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3c47-115">Application</span></span>|<span data-ttu-id="f3c47-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3c47-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3c47-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3c47-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="f3c47-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f3c47-118">Request headers</span></span>
|<span data-ttu-id="f3c47-119">标头</span><span class="sxs-lookup"><span data-stu-id="f3c47-119">Header</span></span>|<span data-ttu-id="f3c47-120">值</span><span class="sxs-lookup"><span data-stu-id="f3c47-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3c47-121">授权</span><span class="sxs-lookup"><span data-stu-id="f3c47-121">Authorization</span></span>|<span data-ttu-id="f3c47-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f3c47-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3c47-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f3c47-123">Accept</span></span>|<span data-ttu-id="f3c47-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f3c47-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3c47-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3c47-125">Request body</span></span>
<span data-ttu-id="f3c47-126">在请求正文中，提供 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3c47-126">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="f3c47-127">下表显示了创建 [iosVppEBook](../resources/intune-books-iosvppebook.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f3c47-127">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="f3c47-128">属性</span><span class="sxs-lookup"><span data-stu-id="f3c47-128">Property</span></span>|<span data-ttu-id="f3c47-129">类型</span><span class="sxs-lookup"><span data-stu-id="f3c47-129">Type</span></span>|<span data-ttu-id="f3c47-130">说明</span><span class="sxs-lookup"><span data-stu-id="f3c47-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3c47-131">id</span><span class="sxs-lookup"><span data-stu-id="f3c47-131">id</span></span>|<span data-ttu-id="f3c47-132">String</span><span class="sxs-lookup"><span data-stu-id="f3c47-132">String</span></span>|<span data-ttu-id="f3c47-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f3c47-133">Key of the entity.</span></span> <span data-ttu-id="f3c47-134">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f3c47-134">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3c47-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f3c47-135">displayName</span></span>|<span data-ttu-id="f3c47-136">String</span><span class="sxs-lookup"><span data-stu-id="f3c47-136">String</span></span>|<span data-ttu-id="f3c47-137">电子书的名称。</span><span class="sxs-lookup"><span data-stu-id="f3c47-137">Name of the eBook.</span></span> <span data-ttu-id="f3c47-138">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f3c47-138">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3c47-139">description</span><span class="sxs-lookup"><span data-stu-id="f3c47-139">description</span></span>|<span data-ttu-id="f3c47-140">String</span><span class="sxs-lookup"><span data-stu-id="f3c47-140">String</span></span>|<span data-ttu-id="f3c47-141">说明。</span><span class="sxs-lookup"><span data-stu-id="f3c47-141">Description.</span></span> <span data-ttu-id="f3c47-142">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f3c47-142">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3c47-143">publisher</span><span class="sxs-lookup"><span data-stu-id="f3c47-143">publisher</span></span>|<span data-ttu-id="f3c47-144">String</span><span class="sxs-lookup"><span data-stu-id="f3c47-144">String</span></span>|<span data-ttu-id="f3c47-145">发布者。</span><span class="sxs-lookup"><span data-stu-id="f3c47-145">Publisher.</span></span> <span data-ttu-id="f3c47-146">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f3c47-146">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3c47-147">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3c47-147">publishedDateTime</span></span>|<span data-ttu-id="f3c47-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3c47-148">DateTimeOffset</span></span>|<span data-ttu-id="f3c47-149">电子书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f3c47-149">The date and time when the eBook was published.</span></span> <span data-ttu-id="f3c47-150">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f3c47-150">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3c47-151">largeCover</span><span class="sxs-lookup"><span data-stu-id="f3c47-151">largeCover</span></span>|[<span data-ttu-id="f3c47-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f3c47-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f3c47-153">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="f3c47-153">Book cover.</span></span> <span data-ttu-id="f3c47-154">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f3c47-154">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3c47-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3c47-155">createdDateTime</span></span>|<span data-ttu-id="f3c47-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3c47-156">DateTimeOffset</span></span>|<span data-ttu-id="f3c47-157">电子书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f3c47-157">The date and time when the eBook file was created.</span></span> <span data-ttu-id="f3c47-158">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f3c47-158">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3c47-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3c47-159">lastModifiedDateTime</span></span>|<span data-ttu-id="f3c47-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3c47-160">DateTimeOffset</span></span>|<span data-ttu-id="f3c47-161">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f3c47-161">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="f3c47-162">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f3c47-162">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3c47-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f3c47-163">informationUrl</span></span>|<span data-ttu-id="f3c47-164">String</span><span class="sxs-lookup"><span data-stu-id="f3c47-164">String</span></span>|<span data-ttu-id="f3c47-165">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="f3c47-165">The more information Url.</span></span> <span data-ttu-id="f3c47-166">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f3c47-166">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3c47-167">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f3c47-167">privacyInformationUrl</span></span>|<span data-ttu-id="f3c47-168">String</span><span class="sxs-lookup"><span data-stu-id="f3c47-168">String</span></span>|<span data-ttu-id="f3c47-169">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="f3c47-169">The privacy statement Url.</span></span> <span data-ttu-id="f3c47-170">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f3c47-170">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f3c47-171">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="f3c47-171">vppTokenId</span></span>|<span data-ttu-id="f3c47-172">Guid</span><span class="sxs-lookup"><span data-stu-id="f3c47-172">Guid</span></span>|<span data-ttu-id="f3c47-173">Vpp 令牌 ID。</span><span class="sxs-lookup"><span data-stu-id="f3c47-173">The Vpp token ID.</span></span>|
|<span data-ttu-id="f3c47-174">appleId</span><span class="sxs-lookup"><span data-stu-id="f3c47-174">appleId</span></span>|<span data-ttu-id="f3c47-175">String</span><span class="sxs-lookup"><span data-stu-id="f3c47-175">String</span></span>|<span data-ttu-id="f3c47-176">与 Vpp 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="f3c47-176">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="f3c47-177">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="f3c47-177">vppOrganizationName</span></span>|<span data-ttu-id="f3c47-178">String</span><span class="sxs-lookup"><span data-stu-id="f3c47-178">String</span></span>|<span data-ttu-id="f3c47-179">Vpp 令牌的组织名称。</span><span class="sxs-lookup"><span data-stu-id="f3c47-179">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="f3c47-180">genres</span><span class="sxs-lookup"><span data-stu-id="f3c47-180">genres</span></span>|<span data-ttu-id="f3c47-181">String 集合</span><span class="sxs-lookup"><span data-stu-id="f3c47-181">String collection</span></span>|<span data-ttu-id="f3c47-182">流派。</span><span class="sxs-lookup"><span data-stu-id="f3c47-182">Genres.</span></span>|
|<span data-ttu-id="f3c47-183">language</span><span class="sxs-lookup"><span data-stu-id="f3c47-183">language</span></span>|<span data-ttu-id="f3c47-184">String</span><span class="sxs-lookup"><span data-stu-id="f3c47-184">String</span></span>|<span data-ttu-id="f3c47-185">语言。</span><span class="sxs-lookup"><span data-stu-id="f3c47-185">Language.</span></span>|
|<span data-ttu-id="f3c47-186">seller</span><span class="sxs-lookup"><span data-stu-id="f3c47-186">seller</span></span>|<span data-ttu-id="f3c47-187">String</span><span class="sxs-lookup"><span data-stu-id="f3c47-187">String</span></span>|<span data-ttu-id="f3c47-188">经销商。</span><span class="sxs-lookup"><span data-stu-id="f3c47-188">Seller.</span></span>|
|<span data-ttu-id="f3c47-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f3c47-189">totalLicenseCount</span></span>|<span data-ttu-id="f3c47-190">Int32</span><span class="sxs-lookup"><span data-stu-id="f3c47-190">Int32</span></span>|<span data-ttu-id="f3c47-191">许可证总数。</span><span class="sxs-lookup"><span data-stu-id="f3c47-191">Total license count.</span></span>|
|<span data-ttu-id="f3c47-192">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f3c47-192">usedLicenseCount</span></span>|<span data-ttu-id="f3c47-193">Int32</span><span class="sxs-lookup"><span data-stu-id="f3c47-193">Int32</span></span>|<span data-ttu-id="f3c47-194">使用的许可证数。</span><span class="sxs-lookup"><span data-stu-id="f3c47-194">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="f3c47-195">响应</span><span class="sxs-lookup"><span data-stu-id="f3c47-195">Response</span></span>
<span data-ttu-id="f3c47-196">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f3c47-196">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3c47-197">示例</span><span class="sxs-lookup"><span data-stu-id="f3c47-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="f3c47-198">请求</span><span class="sxs-lookup"><span data-stu-id="f3c47-198">Request</span></span>
<span data-ttu-id="f3c47-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f3c47-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
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

### <a name="response"></a><span data-ttu-id="f3c47-200">响应</span><span class="sxs-lookup"><span data-stu-id="f3c47-200">Response</span></span>
<span data-ttu-id="f3c47-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f3c47-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



