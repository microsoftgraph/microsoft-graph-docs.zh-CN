---
title: 创建 iosVppEBook
description: 创建新的 iosVppEBook 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 267ee13b37657d18a3123cec15eb3ea88d70a47d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015836"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="a69cb-103">创建 iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="a69cb-103">Create iosVppEBook</span></span>

> <span data-ttu-id="a69cb-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a69cb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a69cb-105">创建新的 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a69cb-105">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a69cb-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a69cb-106">Prerequisites</span></span>
<span data-ttu-id="a69cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a69cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a69cb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a69cb-109">Permission type</span></span>|<span data-ttu-id="a69cb-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a69cb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a69cb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a69cb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a69cb-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a69cb-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a69cb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a69cb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a69cb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a69cb-114">Not supported.</span></span>|
|<span data-ttu-id="a69cb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a69cb-115">Application</span></span>|<span data-ttu-id="a69cb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a69cb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a69cb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a69cb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="a69cb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a69cb-118">Request headers</span></span>
|<span data-ttu-id="a69cb-119">标头</span><span class="sxs-lookup"><span data-stu-id="a69cb-119">Header</span></span>|<span data-ttu-id="a69cb-120">值</span><span class="sxs-lookup"><span data-stu-id="a69cb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a69cb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a69cb-121">Authorization</span></span>|<span data-ttu-id="a69cb-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a69cb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a69cb-123">接受</span><span class="sxs-lookup"><span data-stu-id="a69cb-123">Accept</span></span>|<span data-ttu-id="a69cb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a69cb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a69cb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a69cb-125">Request body</span></span>
<span data-ttu-id="a69cb-126">在请求正文中，提供 iosVppEBook 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a69cb-126">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="a69cb-127">下表显示了创建 iosVppEBook 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a69cb-127">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="a69cb-128">属性</span><span class="sxs-lookup"><span data-stu-id="a69cb-128">Property</span></span>|<span data-ttu-id="a69cb-129">类型</span><span class="sxs-lookup"><span data-stu-id="a69cb-129">Type</span></span>|<span data-ttu-id="a69cb-130">说明</span><span class="sxs-lookup"><span data-stu-id="a69cb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a69cb-131">id</span><span class="sxs-lookup"><span data-stu-id="a69cb-131">id</span></span>|<span data-ttu-id="a69cb-132">字符串</span><span class="sxs-lookup"><span data-stu-id="a69cb-132">String</span></span>|<span data-ttu-id="a69cb-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a69cb-133">Key of the entity.</span></span> <span data-ttu-id="a69cb-134">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a69cb-134">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a69cb-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a69cb-135">displayName</span></span>|<span data-ttu-id="a69cb-136">字符串</span><span class="sxs-lookup"><span data-stu-id="a69cb-136">String</span></span>|<span data-ttu-id="a69cb-137">电子图书的名称。</span><span class="sxs-lookup"><span data-stu-id="a69cb-137">Name of the eBook.</span></span> <span data-ttu-id="a69cb-138">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a69cb-138">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a69cb-139">说明</span><span class="sxs-lookup"><span data-stu-id="a69cb-139">description</span></span>|<span data-ttu-id="a69cb-140">String</span><span class="sxs-lookup"><span data-stu-id="a69cb-140">String</span></span>|<span data-ttu-id="a69cb-141">说明。</span><span class="sxs-lookup"><span data-stu-id="a69cb-141">Description.</span></span> <span data-ttu-id="a69cb-142">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a69cb-142">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a69cb-143">publisher</span><span class="sxs-lookup"><span data-stu-id="a69cb-143">publisher</span></span>|<span data-ttu-id="a69cb-144">String</span><span class="sxs-lookup"><span data-stu-id="a69cb-144">String</span></span>|<span data-ttu-id="a69cb-145">发布者。</span><span class="sxs-lookup"><span data-stu-id="a69cb-145">Publisher.</span></span> <span data-ttu-id="a69cb-146">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a69cb-146">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a69cb-147">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="a69cb-147">publishedDateTime</span></span>|<span data-ttu-id="a69cb-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a69cb-148">DateTimeOffset</span></span>|<span data-ttu-id="a69cb-149">电子图书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a69cb-149">The date and time when the eBook was published.</span></span> <span data-ttu-id="a69cb-150">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a69cb-150">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a69cb-151">largeCover</span><span class="sxs-lookup"><span data-stu-id="a69cb-151">largeCover</span></span>|[<span data-ttu-id="a69cb-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a69cb-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a69cb-153">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="a69cb-153">Book cover.</span></span> <span data-ttu-id="a69cb-154">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a69cb-154">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a69cb-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a69cb-155">createdDateTime</span></span>|<span data-ttu-id="a69cb-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a69cb-156">DateTimeOffset</span></span>|<span data-ttu-id="a69cb-157">电子图书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a69cb-157">The date and time when the eBook file was created.</span></span> <span data-ttu-id="a69cb-158">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a69cb-158">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a69cb-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a69cb-159">lastModifiedDateTime</span></span>|<span data-ttu-id="a69cb-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a69cb-160">DateTimeOffset</span></span>|<span data-ttu-id="a69cb-161">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a69cb-161">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="a69cb-162">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a69cb-162">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a69cb-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a69cb-163">informationUrl</span></span>|<span data-ttu-id="a69cb-164">String</span><span class="sxs-lookup"><span data-stu-id="a69cb-164">String</span></span>|<span data-ttu-id="a69cb-165">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="a69cb-165">The more information Url.</span></span> <span data-ttu-id="a69cb-166">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a69cb-166">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a69cb-167">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a69cb-167">privacyInformationUrl</span></span>|<span data-ttu-id="a69cb-168">String</span><span class="sxs-lookup"><span data-stu-id="a69cb-168">String</span></span>|<span data-ttu-id="a69cb-169">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="a69cb-169">The privacy statement Url.</span></span> <span data-ttu-id="a69cb-170">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a69cb-170">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a69cb-171">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="a69cb-171">vppTokenId</span></span>|<span data-ttu-id="a69cb-172">Guid</span><span class="sxs-lookup"><span data-stu-id="a69cb-172">Guid</span></span>|<span data-ttu-id="a69cb-173">Vpp 令牌 ID。</span><span class="sxs-lookup"><span data-stu-id="a69cb-173">The Vpp token ID.</span></span>|
|<span data-ttu-id="a69cb-174">appleId</span><span class="sxs-lookup"><span data-stu-id="a69cb-174">appleId</span></span>|<span data-ttu-id="a69cb-175">String</span><span class="sxs-lookup"><span data-stu-id="a69cb-175">String</span></span>|<span data-ttu-id="a69cb-176">与 Vpp 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="a69cb-176">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="a69cb-177">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="a69cb-177">vppOrganizationName</span></span>|<span data-ttu-id="a69cb-178">String</span><span class="sxs-lookup"><span data-stu-id="a69cb-178">String</span></span>|<span data-ttu-id="a69cb-179">Vpp 令牌的组织名称。</span><span class="sxs-lookup"><span data-stu-id="a69cb-179">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="a69cb-180">genres</span><span class="sxs-lookup"><span data-stu-id="a69cb-180">genres</span></span>|<span data-ttu-id="a69cb-181">String 集合</span><span class="sxs-lookup"><span data-stu-id="a69cb-181">String collection</span></span>|<span data-ttu-id="a69cb-182">流派。</span><span class="sxs-lookup"><span data-stu-id="a69cb-182">Genres.</span></span>|
|<span data-ttu-id="a69cb-183">language</span><span class="sxs-lookup"><span data-stu-id="a69cb-183">language</span></span>|<span data-ttu-id="a69cb-184">String</span><span class="sxs-lookup"><span data-stu-id="a69cb-184">String</span></span>|<span data-ttu-id="a69cb-185">语言。</span><span class="sxs-lookup"><span data-stu-id="a69cb-185">Language.</span></span>|
|<span data-ttu-id="a69cb-186">seller</span><span class="sxs-lookup"><span data-stu-id="a69cb-186">seller</span></span>|<span data-ttu-id="a69cb-187">String</span><span class="sxs-lookup"><span data-stu-id="a69cb-187">String</span></span>|<span data-ttu-id="a69cb-188">经销商。</span><span class="sxs-lookup"><span data-stu-id="a69cb-188">Seller.</span></span>|
|<span data-ttu-id="a69cb-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a69cb-189">totalLicenseCount</span></span>|<span data-ttu-id="a69cb-190">Int32</span><span class="sxs-lookup"><span data-stu-id="a69cb-190">Int32</span></span>|<span data-ttu-id="a69cb-191">许可证总数。</span><span class="sxs-lookup"><span data-stu-id="a69cb-191">Total license count.</span></span>|
|<span data-ttu-id="a69cb-192">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a69cb-192">usedLicenseCount</span></span>|<span data-ttu-id="a69cb-193">Int32</span><span class="sxs-lookup"><span data-stu-id="a69cb-193">Int32</span></span>|<span data-ttu-id="a69cb-194">使用的许可证数。</span><span class="sxs-lookup"><span data-stu-id="a69cb-194">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="a69cb-195">响应</span><span class="sxs-lookup"><span data-stu-id="a69cb-195">Response</span></span>
<span data-ttu-id="a69cb-196">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a69cb-196">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a69cb-197">示例</span><span class="sxs-lookup"><span data-stu-id="a69cb-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="a69cb-198">请求</span><span class="sxs-lookup"><span data-stu-id="a69cb-198">Request</span></span>
<span data-ttu-id="a69cb-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a69cb-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a69cb-200">响应</span><span class="sxs-lookup"><span data-stu-id="a69cb-200">Response</span></span>
<span data-ttu-id="a69cb-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a69cb-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



