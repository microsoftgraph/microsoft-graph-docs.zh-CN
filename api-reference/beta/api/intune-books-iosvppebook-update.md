---
title: 更新 iosVppEBook
description: 更新 iosVppEBook 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1bbf07c5eefeca73ae69b7488f7cddf426ce06cd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43392718"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="a1cc0-103">更新 iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="a1cc0-103">Update iosVppEBook</span></span>

<span data-ttu-id="a1cc0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1cc0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1cc0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1cc0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1cc0-107">更新 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-107">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1cc0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1cc0-108">Prerequisites</span></span>
<span data-ttu-id="a1cc0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1cc0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1cc0-111">Permission type</span></span>|<span data-ttu-id="a1cc0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a1cc0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1cc0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1cc0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1cc0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1cc0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a1cc0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1cc0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1cc0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-116">Not supported.</span></span>|
|<span data-ttu-id="a1cc0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1cc0-117">Application</span></span>|<span data-ttu-id="a1cc0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1cc0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1cc0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1cc0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="a1cc0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1cc0-120">Request headers</span></span>
|<span data-ttu-id="a1cc0-121">标头</span><span class="sxs-lookup"><span data-stu-id="a1cc0-121">Header</span></span>|<span data-ttu-id="a1cc0-122">值</span><span class="sxs-lookup"><span data-stu-id="a1cc0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1cc0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1cc0-123">Authorization</span></span>|<span data-ttu-id="a1cc0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1cc0-125">接受</span><span class="sxs-lookup"><span data-stu-id="a1cc0-125">Accept</span></span>|<span data-ttu-id="a1cc0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1cc0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1cc0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1cc0-127">Request body</span></span>
<span data-ttu-id="a1cc0-128">在请求正文中，提供 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-128">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="a1cc0-129">下表显示了创建 [iosVppEBook](../resources/intune-books-iosvppebook.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-129">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="a1cc0-130">属性</span><span class="sxs-lookup"><span data-stu-id="a1cc0-130">Property</span></span>|<span data-ttu-id="a1cc0-131">类型</span><span class="sxs-lookup"><span data-stu-id="a1cc0-131">Type</span></span>|<span data-ttu-id="a1cc0-132">说明</span><span class="sxs-lookup"><span data-stu-id="a1cc0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1cc0-133">id</span><span class="sxs-lookup"><span data-stu-id="a1cc0-133">id</span></span>|<span data-ttu-id="a1cc0-134">字符串</span><span class="sxs-lookup"><span data-stu-id="a1cc0-134">String</span></span>|<span data-ttu-id="a1cc0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-135">Key of the entity.</span></span> <span data-ttu-id="a1cc0-136">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a1cc0-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a1cc0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a1cc0-137">displayName</span></span>|<span data-ttu-id="a1cc0-138">字符串</span><span class="sxs-lookup"><span data-stu-id="a1cc0-138">String</span></span>|<span data-ttu-id="a1cc0-139">电子图书的名称。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-139">Name of the eBook.</span></span> <span data-ttu-id="a1cc0-140">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a1cc0-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a1cc0-141">description</span><span class="sxs-lookup"><span data-stu-id="a1cc0-141">description</span></span>|<span data-ttu-id="a1cc0-142">String</span><span class="sxs-lookup"><span data-stu-id="a1cc0-142">String</span></span>|<span data-ttu-id="a1cc0-143">说明。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-143">Description.</span></span> <span data-ttu-id="a1cc0-144">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a1cc0-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a1cc0-145">publisher</span><span class="sxs-lookup"><span data-stu-id="a1cc0-145">publisher</span></span>|<span data-ttu-id="a1cc0-146">字符串</span><span class="sxs-lookup"><span data-stu-id="a1cc0-146">String</span></span>|<span data-ttu-id="a1cc0-147">发布者。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-147">Publisher.</span></span> <span data-ttu-id="a1cc0-148">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a1cc0-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a1cc0-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1cc0-149">publishedDateTime</span></span>|<span data-ttu-id="a1cc0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1cc0-150">DateTimeOffset</span></span>|<span data-ttu-id="a1cc0-151">电子图书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="a1cc0-152">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a1cc0-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a1cc0-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="a1cc0-153">largeCover</span></span>|[<span data-ttu-id="a1cc0-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a1cc0-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a1cc0-155">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-155">Book cover.</span></span> <span data-ttu-id="a1cc0-156">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a1cc0-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a1cc0-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1cc0-157">createdDateTime</span></span>|<span data-ttu-id="a1cc0-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1cc0-158">DateTimeOffset</span></span>|<span data-ttu-id="a1cc0-159">电子图书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="a1cc0-160">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a1cc0-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a1cc0-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1cc0-161">lastModifiedDateTime</span></span>|<span data-ttu-id="a1cc0-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1cc0-162">DateTimeOffset</span></span>|<span data-ttu-id="a1cc0-163">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="a1cc0-164">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a1cc0-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a1cc0-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a1cc0-165">informationUrl</span></span>|<span data-ttu-id="a1cc0-166">字符串</span><span class="sxs-lookup"><span data-stu-id="a1cc0-166">String</span></span>|<span data-ttu-id="a1cc0-167">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-167">The more information Url.</span></span> <span data-ttu-id="a1cc0-168">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a1cc0-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a1cc0-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a1cc0-169">privacyInformationUrl</span></span>|<span data-ttu-id="a1cc0-170">字符串</span><span class="sxs-lookup"><span data-stu-id="a1cc0-170">String</span></span>|<span data-ttu-id="a1cc0-171">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-171">The privacy statement Url.</span></span> <span data-ttu-id="a1cc0-172">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a1cc0-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="a1cc0-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="a1cc0-173">vppTokenId</span></span>|<span data-ttu-id="a1cc0-174">Guid</span><span class="sxs-lookup"><span data-stu-id="a1cc0-174">Guid</span></span>|<span data-ttu-id="a1cc0-175">Vpp 令牌 ID。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="a1cc0-176">appleId</span><span class="sxs-lookup"><span data-stu-id="a1cc0-176">appleId</span></span>|<span data-ttu-id="a1cc0-177">字符串</span><span class="sxs-lookup"><span data-stu-id="a1cc0-177">String</span></span>|<span data-ttu-id="a1cc0-178">与 Vpp 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="a1cc0-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="a1cc0-179">vppOrganizationName</span></span>|<span data-ttu-id="a1cc0-180">字符串</span><span class="sxs-lookup"><span data-stu-id="a1cc0-180">String</span></span>|<span data-ttu-id="a1cc0-181">Vpp 令牌的组织名称。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="a1cc0-182">genres</span><span class="sxs-lookup"><span data-stu-id="a1cc0-182">genres</span></span>|<span data-ttu-id="a1cc0-183">String 集合</span><span class="sxs-lookup"><span data-stu-id="a1cc0-183">String collection</span></span>|<span data-ttu-id="a1cc0-184">流派。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-184">Genres.</span></span>|
|<span data-ttu-id="a1cc0-185">language</span><span class="sxs-lookup"><span data-stu-id="a1cc0-185">language</span></span>|<span data-ttu-id="a1cc0-186">字符串</span><span class="sxs-lookup"><span data-stu-id="a1cc0-186">String</span></span>|<span data-ttu-id="a1cc0-187">语言。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-187">Language.</span></span>|
|<span data-ttu-id="a1cc0-188">seller</span><span class="sxs-lookup"><span data-stu-id="a1cc0-188">seller</span></span>|<span data-ttu-id="a1cc0-189">String</span><span class="sxs-lookup"><span data-stu-id="a1cc0-189">String</span></span>|<span data-ttu-id="a1cc0-190">经销商。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-190">Seller.</span></span>|
|<span data-ttu-id="a1cc0-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a1cc0-191">totalLicenseCount</span></span>|<span data-ttu-id="a1cc0-192">Int32</span><span class="sxs-lookup"><span data-stu-id="a1cc0-192">Int32</span></span>|<span data-ttu-id="a1cc0-193">许可证总数。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-193">Total license count.</span></span>|
|<span data-ttu-id="a1cc0-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a1cc0-194">usedLicenseCount</span></span>|<span data-ttu-id="a1cc0-195">Int32</span><span class="sxs-lookup"><span data-stu-id="a1cc0-195">Int32</span></span>|<span data-ttu-id="a1cc0-196">使用的许可证数。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-196">Used license count.</span></span>|
|<span data-ttu-id="a1cc0-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a1cc0-197">roleScopeTagIds</span></span>|<span data-ttu-id="a1cc0-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="a1cc0-198">String collection</span></span>|<span data-ttu-id="a1cc0-199">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-199">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="a1cc0-200">响应</span><span class="sxs-lookup"><span data-stu-id="a1cc0-200">Response</span></span>
<span data-ttu-id="a1cc0-201">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-201">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1cc0-202">示例</span><span class="sxs-lookup"><span data-stu-id="a1cc0-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1cc0-203">请求</span><span class="sxs-lookup"><span data-stu-id="a1cc0-203">Request</span></span>
<span data-ttu-id="a1cc0-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a1cc0-205">响应</span><span class="sxs-lookup"><span data-stu-id="a1cc0-205">Response</span></span>
<span data-ttu-id="a1cc0-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1cc0-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



