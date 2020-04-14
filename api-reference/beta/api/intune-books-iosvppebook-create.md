---
title: 创建 iosVppEBook
description: 创建新的 iosVppEBook 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 03e88512487a6ab4c5e948f1c240f47403b2583c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43423172"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="70796-103">创建 iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="70796-103">Create iosVppEBook</span></span>

<span data-ttu-id="70796-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70796-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70796-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="70796-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70796-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="70796-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70796-107">创建新的 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="70796-107">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70796-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="70796-108">Prerequisites</span></span>
<span data-ttu-id="70796-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70796-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70796-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="70796-111">Permission type</span></span>|<span data-ttu-id="70796-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="70796-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70796-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70796-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70796-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70796-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="70796-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70796-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70796-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="70796-116">Not supported.</span></span>|
|<span data-ttu-id="70796-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="70796-117">Application</span></span>|<span data-ttu-id="70796-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70796-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="70796-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70796-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="70796-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="70796-120">Request headers</span></span>
|<span data-ttu-id="70796-121">标头</span><span class="sxs-lookup"><span data-stu-id="70796-121">Header</span></span>|<span data-ttu-id="70796-122">值</span><span class="sxs-lookup"><span data-stu-id="70796-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70796-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="70796-123">Authorization</span></span>|<span data-ttu-id="70796-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="70796-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70796-125">接受</span><span class="sxs-lookup"><span data-stu-id="70796-125">Accept</span></span>|<span data-ttu-id="70796-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70796-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70796-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="70796-127">Request body</span></span>
<span data-ttu-id="70796-128">在请求正文中，提供 iosVppEBook 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70796-128">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="70796-129">下表显示了创建 iosVppEBook 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="70796-129">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="70796-130">属性</span><span class="sxs-lookup"><span data-stu-id="70796-130">Property</span></span>|<span data-ttu-id="70796-131">类型</span><span class="sxs-lookup"><span data-stu-id="70796-131">Type</span></span>|<span data-ttu-id="70796-132">说明</span><span class="sxs-lookup"><span data-stu-id="70796-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70796-133">id</span><span class="sxs-lookup"><span data-stu-id="70796-133">id</span></span>|<span data-ttu-id="70796-134">字符串</span><span class="sxs-lookup"><span data-stu-id="70796-134">String</span></span>|<span data-ttu-id="70796-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="70796-135">Key of the entity.</span></span> <span data-ttu-id="70796-136">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="70796-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="70796-137">displayName</span><span class="sxs-lookup"><span data-stu-id="70796-137">displayName</span></span>|<span data-ttu-id="70796-138">字符串</span><span class="sxs-lookup"><span data-stu-id="70796-138">String</span></span>|<span data-ttu-id="70796-139">电子图书的名称。</span><span class="sxs-lookup"><span data-stu-id="70796-139">Name of the eBook.</span></span> <span data-ttu-id="70796-140">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="70796-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="70796-141">description</span><span class="sxs-lookup"><span data-stu-id="70796-141">description</span></span>|<span data-ttu-id="70796-142">String</span><span class="sxs-lookup"><span data-stu-id="70796-142">String</span></span>|<span data-ttu-id="70796-143">说明。</span><span class="sxs-lookup"><span data-stu-id="70796-143">Description.</span></span> <span data-ttu-id="70796-144">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="70796-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="70796-145">publisher</span><span class="sxs-lookup"><span data-stu-id="70796-145">publisher</span></span>|<span data-ttu-id="70796-146">String</span><span class="sxs-lookup"><span data-stu-id="70796-146">String</span></span>|<span data-ttu-id="70796-147">发布者。</span><span class="sxs-lookup"><span data-stu-id="70796-147">Publisher.</span></span> <span data-ttu-id="70796-148">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="70796-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="70796-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="70796-149">publishedDateTime</span></span>|<span data-ttu-id="70796-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70796-150">DateTimeOffset</span></span>|<span data-ttu-id="70796-151">电子图书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="70796-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="70796-152">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="70796-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="70796-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="70796-153">largeCover</span></span>|[<span data-ttu-id="70796-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="70796-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="70796-155">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="70796-155">Book cover.</span></span> <span data-ttu-id="70796-156">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="70796-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="70796-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70796-157">createdDateTime</span></span>|<span data-ttu-id="70796-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70796-158">DateTimeOffset</span></span>|<span data-ttu-id="70796-159">电子图书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="70796-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="70796-160">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="70796-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="70796-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70796-161">lastModifiedDateTime</span></span>|<span data-ttu-id="70796-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70796-162">DateTimeOffset</span></span>|<span data-ttu-id="70796-163">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="70796-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="70796-164">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="70796-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="70796-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="70796-165">informationUrl</span></span>|<span data-ttu-id="70796-166">String</span><span class="sxs-lookup"><span data-stu-id="70796-166">String</span></span>|<span data-ttu-id="70796-167">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="70796-167">The more information Url.</span></span> <span data-ttu-id="70796-168">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="70796-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="70796-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="70796-169">privacyInformationUrl</span></span>|<span data-ttu-id="70796-170">String</span><span class="sxs-lookup"><span data-stu-id="70796-170">String</span></span>|<span data-ttu-id="70796-171">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="70796-171">The privacy statement Url.</span></span> <span data-ttu-id="70796-172">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="70796-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="70796-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="70796-173">vppTokenId</span></span>|<span data-ttu-id="70796-174">Guid</span><span class="sxs-lookup"><span data-stu-id="70796-174">Guid</span></span>|<span data-ttu-id="70796-175">Vpp 令牌 ID。</span><span class="sxs-lookup"><span data-stu-id="70796-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="70796-176">appleId</span><span class="sxs-lookup"><span data-stu-id="70796-176">appleId</span></span>|<span data-ttu-id="70796-177">String</span><span class="sxs-lookup"><span data-stu-id="70796-177">String</span></span>|<span data-ttu-id="70796-178">与 Vpp 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="70796-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="70796-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="70796-179">vppOrganizationName</span></span>|<span data-ttu-id="70796-180">String</span><span class="sxs-lookup"><span data-stu-id="70796-180">String</span></span>|<span data-ttu-id="70796-181">Vpp 令牌的组织名称。</span><span class="sxs-lookup"><span data-stu-id="70796-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="70796-182">genres</span><span class="sxs-lookup"><span data-stu-id="70796-182">genres</span></span>|<span data-ttu-id="70796-183">String 集合</span><span class="sxs-lookup"><span data-stu-id="70796-183">String collection</span></span>|<span data-ttu-id="70796-184">流派。</span><span class="sxs-lookup"><span data-stu-id="70796-184">Genres.</span></span>|
|<span data-ttu-id="70796-185">language</span><span class="sxs-lookup"><span data-stu-id="70796-185">language</span></span>|<span data-ttu-id="70796-186">String</span><span class="sxs-lookup"><span data-stu-id="70796-186">String</span></span>|<span data-ttu-id="70796-187">语言。</span><span class="sxs-lookup"><span data-stu-id="70796-187">Language.</span></span>|
|<span data-ttu-id="70796-188">seller</span><span class="sxs-lookup"><span data-stu-id="70796-188">seller</span></span>|<span data-ttu-id="70796-189">String</span><span class="sxs-lookup"><span data-stu-id="70796-189">String</span></span>|<span data-ttu-id="70796-190">经销商。</span><span class="sxs-lookup"><span data-stu-id="70796-190">Seller.</span></span>|
|<span data-ttu-id="70796-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="70796-191">totalLicenseCount</span></span>|<span data-ttu-id="70796-192">Int32</span><span class="sxs-lookup"><span data-stu-id="70796-192">Int32</span></span>|<span data-ttu-id="70796-193">许可证总数。</span><span class="sxs-lookup"><span data-stu-id="70796-193">Total license count.</span></span>|
|<span data-ttu-id="70796-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="70796-194">usedLicenseCount</span></span>|<span data-ttu-id="70796-195">Int32</span><span class="sxs-lookup"><span data-stu-id="70796-195">Int32</span></span>|<span data-ttu-id="70796-196">使用的许可证数。</span><span class="sxs-lookup"><span data-stu-id="70796-196">Used license count.</span></span>|
|<span data-ttu-id="70796-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="70796-197">roleScopeTagIds</span></span>|<span data-ttu-id="70796-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="70796-198">String collection</span></span>|<span data-ttu-id="70796-199">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="70796-199">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="70796-200">响应</span><span class="sxs-lookup"><span data-stu-id="70796-200">Response</span></span>
<span data-ttu-id="70796-201">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="70796-201">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70796-202">示例</span><span class="sxs-lookup"><span data-stu-id="70796-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="70796-203">请求</span><span class="sxs-lookup"><span data-stu-id="70796-203">Request</span></span>
<span data-ttu-id="70796-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="70796-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
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

### <a name="response"></a><span data-ttu-id="70796-205">响应</span><span class="sxs-lookup"><span data-stu-id="70796-205">Response</span></span>
<span data-ttu-id="70796-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="70796-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



