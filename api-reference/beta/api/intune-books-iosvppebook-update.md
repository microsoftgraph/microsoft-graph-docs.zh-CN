---
title: 更新 iosVppEBook
description: 更新 iosVppEBook 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f5129eba23f8e86af9f7cc41fef666702b5089cc
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934262"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="8a4e0-103">更新 iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="8a4e0-103">Update iosVppEBook</span></span>

> <span data-ttu-id="8a4e0-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a4e0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a4e0-106">更新 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-106">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a4e0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8a4e0-107">Prerequisites</span></span>
<span data-ttu-id="8a4e0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a4e0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a4e0-110">Permission type</span></span>|<span data-ttu-id="8a4e0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8a4e0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a4e0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a4e0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8a4e0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a4e0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8a4e0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a4e0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a4e0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-115">Not supported.</span></span>|
|<span data-ttu-id="8a4e0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a4e0-116">Application</span></span>|<span data-ttu-id="8a4e0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a4e0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a4e0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="8a4e0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a4e0-119">Request headers</span></span>
|<span data-ttu-id="8a4e0-120">标头</span><span class="sxs-lookup"><span data-stu-id="8a4e0-120">Header</span></span>|<span data-ttu-id="8a4e0-121">值</span><span class="sxs-lookup"><span data-stu-id="8a4e0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a4e0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a4e0-122">Authorization</span></span>|<span data-ttu-id="8a4e0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a4e0-124">接受</span><span class="sxs-lookup"><span data-stu-id="8a4e0-124">Accept</span></span>|<span data-ttu-id="8a4e0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8a4e0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a4e0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a4e0-126">Request body</span></span>
<span data-ttu-id="8a4e0-127">在请求正文中，提供 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-127">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="8a4e0-128">下表显示了创建 [iosVppEBook](../resources/intune-books-iosvppebook.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-128">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="8a4e0-129">属性</span><span class="sxs-lookup"><span data-stu-id="8a4e0-129">Property</span></span>|<span data-ttu-id="8a4e0-130">类型</span><span class="sxs-lookup"><span data-stu-id="8a4e0-130">Type</span></span>|<span data-ttu-id="8a4e0-131">说明</span><span class="sxs-lookup"><span data-stu-id="8a4e0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a4e0-132">id</span><span class="sxs-lookup"><span data-stu-id="8a4e0-132">id</span></span>|<span data-ttu-id="8a4e0-133">字符串</span><span class="sxs-lookup"><span data-stu-id="8a4e0-133">String</span></span>|<span data-ttu-id="8a4e0-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-134">Key of the entity.</span></span> <span data-ttu-id="8a4e0-135">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="8a4e0-135">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="8a4e0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8a4e0-136">displayName</span></span>|<span data-ttu-id="8a4e0-137">字符串</span><span class="sxs-lookup"><span data-stu-id="8a4e0-137">String</span></span>|<span data-ttu-id="8a4e0-138">电子图书的名称。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-138">Name of the eBook.</span></span> <span data-ttu-id="8a4e0-139">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="8a4e0-139">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="8a4e0-140">说明</span><span class="sxs-lookup"><span data-stu-id="8a4e0-140">description</span></span>|<span data-ttu-id="8a4e0-141">String</span><span class="sxs-lookup"><span data-stu-id="8a4e0-141">String</span></span>|<span data-ttu-id="8a4e0-142">说明。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-142">Description.</span></span> <span data-ttu-id="8a4e0-143">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="8a4e0-143">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="8a4e0-144">publisher</span><span class="sxs-lookup"><span data-stu-id="8a4e0-144">publisher</span></span>|<span data-ttu-id="8a4e0-145">String</span><span class="sxs-lookup"><span data-stu-id="8a4e0-145">String</span></span>|<span data-ttu-id="8a4e0-146">发布者。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-146">Publisher.</span></span> <span data-ttu-id="8a4e0-147">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="8a4e0-147">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="8a4e0-148">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a4e0-148">publishedDateTime</span></span>|<span data-ttu-id="8a4e0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a4e0-149">DateTimeOffset</span></span>|<span data-ttu-id="8a4e0-150">电子图书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-150">The date and time when the eBook was published.</span></span> <span data-ttu-id="8a4e0-151">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="8a4e0-151">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="8a4e0-152">largeCover</span><span class="sxs-lookup"><span data-stu-id="8a4e0-152">largeCover</span></span>|[<span data-ttu-id="8a4e0-153">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8a4e0-153">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8a4e0-154">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-154">Book cover.</span></span> <span data-ttu-id="8a4e0-155">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="8a4e0-155">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="8a4e0-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a4e0-156">createdDateTime</span></span>|<span data-ttu-id="8a4e0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a4e0-157">DateTimeOffset</span></span>|<span data-ttu-id="8a4e0-158">电子图书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-158">The date and time when the eBook file was created.</span></span> <span data-ttu-id="8a4e0-159">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="8a4e0-159">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="8a4e0-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a4e0-160">lastModifiedDateTime</span></span>|<span data-ttu-id="8a4e0-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a4e0-161">DateTimeOffset</span></span>|<span data-ttu-id="8a4e0-162">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-162">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="8a4e0-163">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="8a4e0-163">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="8a4e0-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8a4e0-164">informationUrl</span></span>|<span data-ttu-id="8a4e0-165">String</span><span class="sxs-lookup"><span data-stu-id="8a4e0-165">String</span></span>|<span data-ttu-id="8a4e0-166">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-166">The more information Url.</span></span> <span data-ttu-id="8a4e0-167">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="8a4e0-167">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="8a4e0-168">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8a4e0-168">privacyInformationUrl</span></span>|<span data-ttu-id="8a4e0-169">String</span><span class="sxs-lookup"><span data-stu-id="8a4e0-169">String</span></span>|<span data-ttu-id="8a4e0-170">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-170">The privacy statement Url.</span></span> <span data-ttu-id="8a4e0-171">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="8a4e0-171">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="8a4e0-172">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="8a4e0-172">vppTokenId</span></span>|<span data-ttu-id="8a4e0-173">Guid</span><span class="sxs-lookup"><span data-stu-id="8a4e0-173">Guid</span></span>|<span data-ttu-id="8a4e0-174">Vpp 令牌 ID。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-174">The Vpp token ID.</span></span>|
|<span data-ttu-id="8a4e0-175">appleId</span><span class="sxs-lookup"><span data-stu-id="8a4e0-175">appleId</span></span>|<span data-ttu-id="8a4e0-176">String</span><span class="sxs-lookup"><span data-stu-id="8a4e0-176">String</span></span>|<span data-ttu-id="8a4e0-177">与 Vpp 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-177">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="8a4e0-178">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="8a4e0-178">vppOrganizationName</span></span>|<span data-ttu-id="8a4e0-179">String</span><span class="sxs-lookup"><span data-stu-id="8a4e0-179">String</span></span>|<span data-ttu-id="8a4e0-180">Vpp 令牌的组织名称。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-180">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="8a4e0-181">genres</span><span class="sxs-lookup"><span data-stu-id="8a4e0-181">genres</span></span>|<span data-ttu-id="8a4e0-182">String 集合</span><span class="sxs-lookup"><span data-stu-id="8a4e0-182">String collection</span></span>|<span data-ttu-id="8a4e0-183">流派。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-183">Genres.</span></span>|
|<span data-ttu-id="8a4e0-184">language</span><span class="sxs-lookup"><span data-stu-id="8a4e0-184">language</span></span>|<span data-ttu-id="8a4e0-185">String</span><span class="sxs-lookup"><span data-stu-id="8a4e0-185">String</span></span>|<span data-ttu-id="8a4e0-186">语言。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-186">Language.</span></span>|
|<span data-ttu-id="8a4e0-187">seller</span><span class="sxs-lookup"><span data-stu-id="8a4e0-187">seller</span></span>|<span data-ttu-id="8a4e0-188">String</span><span class="sxs-lookup"><span data-stu-id="8a4e0-188">String</span></span>|<span data-ttu-id="8a4e0-189">经销商。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-189">Seller.</span></span>|
|<span data-ttu-id="8a4e0-190">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8a4e0-190">totalLicenseCount</span></span>|<span data-ttu-id="8a4e0-191">Int32</span><span class="sxs-lookup"><span data-stu-id="8a4e0-191">Int32</span></span>|<span data-ttu-id="8a4e0-192">许可证总数。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-192">Total license count.</span></span>|
|<span data-ttu-id="8a4e0-193">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8a4e0-193">usedLicenseCount</span></span>|<span data-ttu-id="8a4e0-194">Int32</span><span class="sxs-lookup"><span data-stu-id="8a4e0-194">Int32</span></span>|<span data-ttu-id="8a4e0-195">使用的许可证数。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-195">Used license count.</span></span>|
|<span data-ttu-id="8a4e0-196">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8a4e0-196">roleScopeTagIds</span></span>|<span data-ttu-id="8a4e0-197">String collection</span><span class="sxs-lookup"><span data-stu-id="8a4e0-197">String collection</span></span>|<span data-ttu-id="8a4e0-198">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-198">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="8a4e0-199">响应</span><span class="sxs-lookup"><span data-stu-id="8a4e0-199">Response</span></span>
<span data-ttu-id="8a4e0-200">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-200">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a4e0-201">示例</span><span class="sxs-lookup"><span data-stu-id="8a4e0-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a4e0-202">请求</span><span class="sxs-lookup"><span data-stu-id="8a4e0-202">Request</span></span>
<span data-ttu-id="8a4e0-203">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}
Content-type: application/json
Content-length: 854

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
  "usedLicenseCount": 0,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="8a4e0-204">响应</span><span class="sxs-lookup"><span data-stu-id="8a4e0-204">Response</span></span>
<span data-ttu-id="8a4e0-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8a4e0-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1026

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
  "usedLicenseCount": 0,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




