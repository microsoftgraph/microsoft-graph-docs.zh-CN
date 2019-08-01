---
title: 更新 iosVppEBook
description: 更新 iosVppEBook 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d68b8ba149b4b5f8b63029df98769d37a5fdd8c7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001878"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="99e7d-103">更新 iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="99e7d-103">Update iosVppEBook</span></span>

> <span data-ttu-id="99e7d-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="99e7d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99e7d-105">更新 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="99e7d-105">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99e7d-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="99e7d-106">Prerequisites</span></span>
<span data-ttu-id="99e7d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99e7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99e7d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="99e7d-109">Permission type</span></span>|<span data-ttu-id="99e7d-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="99e7d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99e7d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99e7d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="99e7d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e7d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="99e7d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99e7d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99e7d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="99e7d-114">Not supported.</span></span>|
|<span data-ttu-id="99e7d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="99e7d-115">Application</span></span>|<span data-ttu-id="99e7d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="99e7d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99e7d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99e7d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="99e7d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="99e7d-118">Request headers</span></span>
|<span data-ttu-id="99e7d-119">标头</span><span class="sxs-lookup"><span data-stu-id="99e7d-119">Header</span></span>|<span data-ttu-id="99e7d-120">值</span><span class="sxs-lookup"><span data-stu-id="99e7d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99e7d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="99e7d-121">Authorization</span></span>|<span data-ttu-id="99e7d-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="99e7d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99e7d-123">接受</span><span class="sxs-lookup"><span data-stu-id="99e7d-123">Accept</span></span>|<span data-ttu-id="99e7d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="99e7d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99e7d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="99e7d-125">Request body</span></span>
<span data-ttu-id="99e7d-126">在请求正文中，提供 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99e7d-126">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="99e7d-127">下表显示了创建 [iosVppEBook](../resources/intune-books-iosvppebook.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="99e7d-127">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="99e7d-128">属性</span><span class="sxs-lookup"><span data-stu-id="99e7d-128">Property</span></span>|<span data-ttu-id="99e7d-129">类型</span><span class="sxs-lookup"><span data-stu-id="99e7d-129">Type</span></span>|<span data-ttu-id="99e7d-130">说明</span><span class="sxs-lookup"><span data-stu-id="99e7d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99e7d-131">id</span><span class="sxs-lookup"><span data-stu-id="99e7d-131">id</span></span>|<span data-ttu-id="99e7d-132">字符串</span><span class="sxs-lookup"><span data-stu-id="99e7d-132">String</span></span>|<span data-ttu-id="99e7d-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="99e7d-133">Key of the entity.</span></span> <span data-ttu-id="99e7d-134">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="99e7d-134">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="99e7d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="99e7d-135">displayName</span></span>|<span data-ttu-id="99e7d-136">字符串</span><span class="sxs-lookup"><span data-stu-id="99e7d-136">String</span></span>|<span data-ttu-id="99e7d-137">电子图书的名称。</span><span class="sxs-lookup"><span data-stu-id="99e7d-137">Name of the eBook.</span></span> <span data-ttu-id="99e7d-138">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="99e7d-138">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="99e7d-139">说明</span><span class="sxs-lookup"><span data-stu-id="99e7d-139">description</span></span>|<span data-ttu-id="99e7d-140">String</span><span class="sxs-lookup"><span data-stu-id="99e7d-140">String</span></span>|<span data-ttu-id="99e7d-141">说明。</span><span class="sxs-lookup"><span data-stu-id="99e7d-141">Description.</span></span> <span data-ttu-id="99e7d-142">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="99e7d-142">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="99e7d-143">publisher</span><span class="sxs-lookup"><span data-stu-id="99e7d-143">publisher</span></span>|<span data-ttu-id="99e7d-144">String</span><span class="sxs-lookup"><span data-stu-id="99e7d-144">String</span></span>|<span data-ttu-id="99e7d-145">发布者。</span><span class="sxs-lookup"><span data-stu-id="99e7d-145">Publisher.</span></span> <span data-ttu-id="99e7d-146">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="99e7d-146">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="99e7d-147">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="99e7d-147">publishedDateTime</span></span>|<span data-ttu-id="99e7d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99e7d-148">DateTimeOffset</span></span>|<span data-ttu-id="99e7d-149">电子图书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="99e7d-149">The date and time when the eBook was published.</span></span> <span data-ttu-id="99e7d-150">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="99e7d-150">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="99e7d-151">largeCover</span><span class="sxs-lookup"><span data-stu-id="99e7d-151">largeCover</span></span>|[<span data-ttu-id="99e7d-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="99e7d-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="99e7d-153">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="99e7d-153">Book cover.</span></span> <span data-ttu-id="99e7d-154">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="99e7d-154">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="99e7d-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99e7d-155">createdDateTime</span></span>|<span data-ttu-id="99e7d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99e7d-156">DateTimeOffset</span></span>|<span data-ttu-id="99e7d-157">电子图书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="99e7d-157">The date and time when the eBook file was created.</span></span> <span data-ttu-id="99e7d-158">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="99e7d-158">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="99e7d-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99e7d-159">lastModifiedDateTime</span></span>|<span data-ttu-id="99e7d-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99e7d-160">DateTimeOffset</span></span>|<span data-ttu-id="99e7d-161">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="99e7d-161">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="99e7d-162">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="99e7d-162">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="99e7d-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="99e7d-163">informationUrl</span></span>|<span data-ttu-id="99e7d-164">String</span><span class="sxs-lookup"><span data-stu-id="99e7d-164">String</span></span>|<span data-ttu-id="99e7d-165">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="99e7d-165">The more information Url.</span></span> <span data-ttu-id="99e7d-166">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="99e7d-166">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="99e7d-167">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="99e7d-167">privacyInformationUrl</span></span>|<span data-ttu-id="99e7d-168">String</span><span class="sxs-lookup"><span data-stu-id="99e7d-168">String</span></span>|<span data-ttu-id="99e7d-169">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="99e7d-169">The privacy statement Url.</span></span> <span data-ttu-id="99e7d-170">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="99e7d-170">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="99e7d-171">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="99e7d-171">vppTokenId</span></span>|<span data-ttu-id="99e7d-172">Guid</span><span class="sxs-lookup"><span data-stu-id="99e7d-172">Guid</span></span>|<span data-ttu-id="99e7d-173">Vpp 令牌 ID。</span><span class="sxs-lookup"><span data-stu-id="99e7d-173">The Vpp token ID.</span></span>|
|<span data-ttu-id="99e7d-174">appleId</span><span class="sxs-lookup"><span data-stu-id="99e7d-174">appleId</span></span>|<span data-ttu-id="99e7d-175">String</span><span class="sxs-lookup"><span data-stu-id="99e7d-175">String</span></span>|<span data-ttu-id="99e7d-176">与 Vpp 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="99e7d-176">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="99e7d-177">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="99e7d-177">vppOrganizationName</span></span>|<span data-ttu-id="99e7d-178">String</span><span class="sxs-lookup"><span data-stu-id="99e7d-178">String</span></span>|<span data-ttu-id="99e7d-179">Vpp 令牌的组织名称。</span><span class="sxs-lookup"><span data-stu-id="99e7d-179">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="99e7d-180">genres</span><span class="sxs-lookup"><span data-stu-id="99e7d-180">genres</span></span>|<span data-ttu-id="99e7d-181">String 集合</span><span class="sxs-lookup"><span data-stu-id="99e7d-181">String collection</span></span>|<span data-ttu-id="99e7d-182">流派。</span><span class="sxs-lookup"><span data-stu-id="99e7d-182">Genres.</span></span>|
|<span data-ttu-id="99e7d-183">language</span><span class="sxs-lookup"><span data-stu-id="99e7d-183">language</span></span>|<span data-ttu-id="99e7d-184">String</span><span class="sxs-lookup"><span data-stu-id="99e7d-184">String</span></span>|<span data-ttu-id="99e7d-185">语言。</span><span class="sxs-lookup"><span data-stu-id="99e7d-185">Language.</span></span>|
|<span data-ttu-id="99e7d-186">seller</span><span class="sxs-lookup"><span data-stu-id="99e7d-186">seller</span></span>|<span data-ttu-id="99e7d-187">String</span><span class="sxs-lookup"><span data-stu-id="99e7d-187">String</span></span>|<span data-ttu-id="99e7d-188">经销商。</span><span class="sxs-lookup"><span data-stu-id="99e7d-188">Seller.</span></span>|
|<span data-ttu-id="99e7d-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="99e7d-189">totalLicenseCount</span></span>|<span data-ttu-id="99e7d-190">Int32</span><span class="sxs-lookup"><span data-stu-id="99e7d-190">Int32</span></span>|<span data-ttu-id="99e7d-191">许可证总数。</span><span class="sxs-lookup"><span data-stu-id="99e7d-191">Total license count.</span></span>|
|<span data-ttu-id="99e7d-192">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="99e7d-192">usedLicenseCount</span></span>|<span data-ttu-id="99e7d-193">Int32</span><span class="sxs-lookup"><span data-stu-id="99e7d-193">Int32</span></span>|<span data-ttu-id="99e7d-194">使用的许可证数。</span><span class="sxs-lookup"><span data-stu-id="99e7d-194">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="99e7d-195">响应</span><span class="sxs-lookup"><span data-stu-id="99e7d-195">Response</span></span>
<span data-ttu-id="99e7d-196">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="99e7d-196">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99e7d-197">示例</span><span class="sxs-lookup"><span data-stu-id="99e7d-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="99e7d-198">请求</span><span class="sxs-lookup"><span data-stu-id="99e7d-198">Request</span></span>
<span data-ttu-id="99e7d-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99e7d-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="99e7d-200">响应</span><span class="sxs-lookup"><span data-stu-id="99e7d-200">Response</span></span>
<span data-ttu-id="99e7d-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="99e7d-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



