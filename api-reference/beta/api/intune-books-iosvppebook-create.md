---
title: 创建 iosVppEBook
description: 创建新的 iosVppEBook 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 45edcdc7a31a6840da0b7af2ae5cf5e9618ad5d8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49245436"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="e4e11-103">创建 iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="e4e11-103">Create iosVppEBook</span></span>

<span data-ttu-id="e4e11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4e11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4e11-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e4e11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4e11-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4e11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4e11-107">创建新的 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e4e11-107">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4e11-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e4e11-108">Prerequisites</span></span>
<span data-ttu-id="e4e11-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4e11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4e11-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4e11-111">Permission type</span></span>|<span data-ttu-id="e4e11-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e4e11-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4e11-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4e11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4e11-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4e11-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e4e11-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4e11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4e11-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4e11-116">Not supported.</span></span>|
|<span data-ttu-id="e4e11-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4e11-117">Application</span></span>|<span data-ttu-id="e4e11-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4e11-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4e11-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4e11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="e4e11-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4e11-120">Request headers</span></span>
|<span data-ttu-id="e4e11-121">标头</span><span class="sxs-lookup"><span data-stu-id="e4e11-121">Header</span></span>|<span data-ttu-id="e4e11-122">值</span><span class="sxs-lookup"><span data-stu-id="e4e11-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4e11-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4e11-123">Authorization</span></span>|<span data-ttu-id="e4e11-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e4e11-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4e11-125">接受</span><span class="sxs-lookup"><span data-stu-id="e4e11-125">Accept</span></span>|<span data-ttu-id="e4e11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4e11-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4e11-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4e11-127">Request body</span></span>
<span data-ttu-id="e4e11-128">在请求正文中，提供 iosVppEBook 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4e11-128">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="e4e11-129">下表显示了创建 iosVppEBook 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e4e11-129">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="e4e11-130">属性</span><span class="sxs-lookup"><span data-stu-id="e4e11-130">Property</span></span>|<span data-ttu-id="e4e11-131">类型</span><span class="sxs-lookup"><span data-stu-id="e4e11-131">Type</span></span>|<span data-ttu-id="e4e11-132">说明</span><span class="sxs-lookup"><span data-stu-id="e4e11-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4e11-133">id</span><span class="sxs-lookup"><span data-stu-id="e4e11-133">id</span></span>|<span data-ttu-id="e4e11-134">String</span><span class="sxs-lookup"><span data-stu-id="e4e11-134">String</span></span>|<span data-ttu-id="e4e11-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e4e11-135">Key of the entity.</span></span> <span data-ttu-id="e4e11-136">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e4e11-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e4e11-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e4e11-137">displayName</span></span>|<span data-ttu-id="e4e11-138">String</span><span class="sxs-lookup"><span data-stu-id="e4e11-138">String</span></span>|<span data-ttu-id="e4e11-139">电子图书的名称。</span><span class="sxs-lookup"><span data-stu-id="e4e11-139">Name of the eBook.</span></span> <span data-ttu-id="e4e11-140">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e4e11-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e4e11-141">description</span><span class="sxs-lookup"><span data-stu-id="e4e11-141">description</span></span>|<span data-ttu-id="e4e11-142">String</span><span class="sxs-lookup"><span data-stu-id="e4e11-142">String</span></span>|<span data-ttu-id="e4e11-143">说明。</span><span class="sxs-lookup"><span data-stu-id="e4e11-143">Description.</span></span> <span data-ttu-id="e4e11-144">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e4e11-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e4e11-145">publisher</span><span class="sxs-lookup"><span data-stu-id="e4e11-145">publisher</span></span>|<span data-ttu-id="e4e11-146">String</span><span class="sxs-lookup"><span data-stu-id="e4e11-146">String</span></span>|<span data-ttu-id="e4e11-147">发布者。</span><span class="sxs-lookup"><span data-stu-id="e4e11-147">Publisher.</span></span> <span data-ttu-id="e4e11-148">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e4e11-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e4e11-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4e11-149">publishedDateTime</span></span>|<span data-ttu-id="e4e11-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4e11-150">DateTimeOffset</span></span>|<span data-ttu-id="e4e11-151">电子图书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e4e11-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="e4e11-152">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e4e11-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e4e11-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="e4e11-153">largeCover</span></span>|[<span data-ttu-id="e4e11-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e4e11-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e4e11-155">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="e4e11-155">Book cover.</span></span> <span data-ttu-id="e4e11-156">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e4e11-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e4e11-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4e11-157">createdDateTime</span></span>|<span data-ttu-id="e4e11-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4e11-158">DateTimeOffset</span></span>|<span data-ttu-id="e4e11-159">电子图书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e4e11-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="e4e11-160">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e4e11-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e4e11-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4e11-161">lastModifiedDateTime</span></span>|<span data-ttu-id="e4e11-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4e11-162">DateTimeOffset</span></span>|<span data-ttu-id="e4e11-163">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e4e11-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="e4e11-164">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e4e11-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e4e11-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e4e11-165">informationUrl</span></span>|<span data-ttu-id="e4e11-166">String</span><span class="sxs-lookup"><span data-stu-id="e4e11-166">String</span></span>|<span data-ttu-id="e4e11-167">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="e4e11-167">The more information Url.</span></span> <span data-ttu-id="e4e11-168">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e4e11-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e4e11-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e4e11-169">privacyInformationUrl</span></span>|<span data-ttu-id="e4e11-170">String</span><span class="sxs-lookup"><span data-stu-id="e4e11-170">String</span></span>|<span data-ttu-id="e4e11-171">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="e4e11-171">The privacy statement Url.</span></span> <span data-ttu-id="e4e11-172">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e4e11-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e4e11-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="e4e11-173">vppTokenId</span></span>|<span data-ttu-id="e4e11-174">Guid</span><span class="sxs-lookup"><span data-stu-id="e4e11-174">Guid</span></span>|<span data-ttu-id="e4e11-175">Vpp 令牌 ID。</span><span class="sxs-lookup"><span data-stu-id="e4e11-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="e4e11-176">appleId</span><span class="sxs-lookup"><span data-stu-id="e4e11-176">appleId</span></span>|<span data-ttu-id="e4e11-177">String</span><span class="sxs-lookup"><span data-stu-id="e4e11-177">String</span></span>|<span data-ttu-id="e4e11-178">与 Vpp 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="e4e11-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="e4e11-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="e4e11-179">vppOrganizationName</span></span>|<span data-ttu-id="e4e11-180">String</span><span class="sxs-lookup"><span data-stu-id="e4e11-180">String</span></span>|<span data-ttu-id="e4e11-181">Vpp 令牌的组织名称。</span><span class="sxs-lookup"><span data-stu-id="e4e11-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="e4e11-182">genres</span><span class="sxs-lookup"><span data-stu-id="e4e11-182">genres</span></span>|<span data-ttu-id="e4e11-183">String 集合</span><span class="sxs-lookup"><span data-stu-id="e4e11-183">String collection</span></span>|<span data-ttu-id="e4e11-184">流派。</span><span class="sxs-lookup"><span data-stu-id="e4e11-184">Genres.</span></span>|
|<span data-ttu-id="e4e11-185">language</span><span class="sxs-lookup"><span data-stu-id="e4e11-185">language</span></span>|<span data-ttu-id="e4e11-186">String</span><span class="sxs-lookup"><span data-stu-id="e4e11-186">String</span></span>|<span data-ttu-id="e4e11-187">语言。</span><span class="sxs-lookup"><span data-stu-id="e4e11-187">Language.</span></span>|
|<span data-ttu-id="e4e11-188">seller</span><span class="sxs-lookup"><span data-stu-id="e4e11-188">seller</span></span>|<span data-ttu-id="e4e11-189">String</span><span class="sxs-lookup"><span data-stu-id="e4e11-189">String</span></span>|<span data-ttu-id="e4e11-190">经销商。</span><span class="sxs-lookup"><span data-stu-id="e4e11-190">Seller.</span></span>|
|<span data-ttu-id="e4e11-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e4e11-191">totalLicenseCount</span></span>|<span data-ttu-id="e4e11-192">Int32</span><span class="sxs-lookup"><span data-stu-id="e4e11-192">Int32</span></span>|<span data-ttu-id="e4e11-193">许可证总数。</span><span class="sxs-lookup"><span data-stu-id="e4e11-193">Total license count.</span></span>|
|<span data-ttu-id="e4e11-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e4e11-194">usedLicenseCount</span></span>|<span data-ttu-id="e4e11-195">Int32</span><span class="sxs-lookup"><span data-stu-id="e4e11-195">Int32</span></span>|<span data-ttu-id="e4e11-196">使用的许可证数。</span><span class="sxs-lookup"><span data-stu-id="e4e11-196">Used license count.</span></span>|
|<span data-ttu-id="e4e11-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e4e11-197">roleScopeTagIds</span></span>|<span data-ttu-id="e4e11-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="e4e11-198">String collection</span></span>|<span data-ttu-id="e4e11-199">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e4e11-199">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="e4e11-200">响应</span><span class="sxs-lookup"><span data-stu-id="e4e11-200">Response</span></span>
<span data-ttu-id="e4e11-201">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e4e11-201">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4e11-202">示例</span><span class="sxs-lookup"><span data-stu-id="e4e11-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4e11-203">请求</span><span class="sxs-lookup"><span data-stu-id="e4e11-203">Request</span></span>
<span data-ttu-id="e4e11-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e4e11-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e4e11-205">响应</span><span class="sxs-lookup"><span data-stu-id="e4e11-205">Response</span></span>
<span data-ttu-id="e4e11-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e4e11-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




