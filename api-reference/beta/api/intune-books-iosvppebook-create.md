---
title: 创建 iosVppEBook
description: 创建新的 iosVppEBook 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bb641714a4ffbdb304ba3a95bb7078d9bc223696
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450361"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="cbddb-103">创建 iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="cbddb-103">Create iosVppEBook</span></span>

<span data-ttu-id="cbddb-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="cbddb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cbddb-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cbddb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbddb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cbddb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbddb-107">创建新的 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cbddb-107">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbddb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cbddb-108">Prerequisites</span></span>
<span data-ttu-id="cbddb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cbddb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbddb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cbddb-111">Permission type</span></span>|<span data-ttu-id="cbddb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cbddb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbddb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cbddb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cbddb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbddb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cbddb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cbddb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbddb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbddb-116">Not supported.</span></span>|
|<span data-ttu-id="cbddb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cbddb-117">Application</span></span>|<span data-ttu-id="cbddb-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbddb-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbddb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cbddb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="cbddb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cbddb-120">Request headers</span></span>
|<span data-ttu-id="cbddb-121">标头</span><span class="sxs-lookup"><span data-stu-id="cbddb-121">Header</span></span>|<span data-ttu-id="cbddb-122">值</span><span class="sxs-lookup"><span data-stu-id="cbddb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbddb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbddb-123">Authorization</span></span>|<span data-ttu-id="cbddb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cbddb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbddb-125">接受</span><span class="sxs-lookup"><span data-stu-id="cbddb-125">Accept</span></span>|<span data-ttu-id="cbddb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cbddb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbddb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cbddb-127">Request body</span></span>
<span data-ttu-id="cbddb-128">在请求正文中，提供 iosVppEBook 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cbddb-128">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="cbddb-129">下表显示了创建 iosVppEBook 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cbddb-129">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="cbddb-130">属性</span><span class="sxs-lookup"><span data-stu-id="cbddb-130">Property</span></span>|<span data-ttu-id="cbddb-131">类型</span><span class="sxs-lookup"><span data-stu-id="cbddb-131">Type</span></span>|<span data-ttu-id="cbddb-132">说明</span><span class="sxs-lookup"><span data-stu-id="cbddb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbddb-133">id</span><span class="sxs-lookup"><span data-stu-id="cbddb-133">id</span></span>|<span data-ttu-id="cbddb-134">字符串</span><span class="sxs-lookup"><span data-stu-id="cbddb-134">String</span></span>|<span data-ttu-id="cbddb-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cbddb-135">Key of the entity.</span></span> <span data-ttu-id="cbddb-136">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cbddb-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cbddb-137">displayName</span><span class="sxs-lookup"><span data-stu-id="cbddb-137">displayName</span></span>|<span data-ttu-id="cbddb-138">字符串</span><span class="sxs-lookup"><span data-stu-id="cbddb-138">String</span></span>|<span data-ttu-id="cbddb-139">电子图书的名称。</span><span class="sxs-lookup"><span data-stu-id="cbddb-139">Name of the eBook.</span></span> <span data-ttu-id="cbddb-140">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cbddb-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cbddb-141">说明</span><span class="sxs-lookup"><span data-stu-id="cbddb-141">description</span></span>|<span data-ttu-id="cbddb-142">String</span><span class="sxs-lookup"><span data-stu-id="cbddb-142">String</span></span>|<span data-ttu-id="cbddb-143">说明。</span><span class="sxs-lookup"><span data-stu-id="cbddb-143">Description.</span></span> <span data-ttu-id="cbddb-144">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cbddb-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cbddb-145">publisher</span><span class="sxs-lookup"><span data-stu-id="cbddb-145">publisher</span></span>|<span data-ttu-id="cbddb-146">String</span><span class="sxs-lookup"><span data-stu-id="cbddb-146">String</span></span>|<span data-ttu-id="cbddb-147">发布者。</span><span class="sxs-lookup"><span data-stu-id="cbddb-147">Publisher.</span></span> <span data-ttu-id="cbddb-148">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cbddb-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cbddb-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="cbddb-149">publishedDateTime</span></span>|<span data-ttu-id="cbddb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbddb-150">DateTimeOffset</span></span>|<span data-ttu-id="cbddb-151">电子图书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cbddb-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="cbddb-152">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cbddb-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cbddb-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="cbddb-153">largeCover</span></span>|[<span data-ttu-id="cbddb-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cbddb-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cbddb-155">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="cbddb-155">Book cover.</span></span> <span data-ttu-id="cbddb-156">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cbddb-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cbddb-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cbddb-157">createdDateTime</span></span>|<span data-ttu-id="cbddb-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbddb-158">DateTimeOffset</span></span>|<span data-ttu-id="cbddb-159">电子图书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cbddb-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="cbddb-160">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cbddb-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cbddb-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cbddb-161">lastModifiedDateTime</span></span>|<span data-ttu-id="cbddb-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbddb-162">DateTimeOffset</span></span>|<span data-ttu-id="cbddb-163">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cbddb-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="cbddb-164">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cbddb-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cbddb-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cbddb-165">informationUrl</span></span>|<span data-ttu-id="cbddb-166">String</span><span class="sxs-lookup"><span data-stu-id="cbddb-166">String</span></span>|<span data-ttu-id="cbddb-167">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="cbddb-167">The more information Url.</span></span> <span data-ttu-id="cbddb-168">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cbddb-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cbddb-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cbddb-169">privacyInformationUrl</span></span>|<span data-ttu-id="cbddb-170">String</span><span class="sxs-lookup"><span data-stu-id="cbddb-170">String</span></span>|<span data-ttu-id="cbddb-171">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="cbddb-171">The privacy statement Url.</span></span> <span data-ttu-id="cbddb-172">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cbddb-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cbddb-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="cbddb-173">vppTokenId</span></span>|<span data-ttu-id="cbddb-174">Guid</span><span class="sxs-lookup"><span data-stu-id="cbddb-174">Guid</span></span>|<span data-ttu-id="cbddb-175">Vpp 令牌 ID。</span><span class="sxs-lookup"><span data-stu-id="cbddb-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="cbddb-176">appleId</span><span class="sxs-lookup"><span data-stu-id="cbddb-176">appleId</span></span>|<span data-ttu-id="cbddb-177">String</span><span class="sxs-lookup"><span data-stu-id="cbddb-177">String</span></span>|<span data-ttu-id="cbddb-178">与 Vpp 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="cbddb-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="cbddb-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="cbddb-179">vppOrganizationName</span></span>|<span data-ttu-id="cbddb-180">String</span><span class="sxs-lookup"><span data-stu-id="cbddb-180">String</span></span>|<span data-ttu-id="cbddb-181">Vpp 令牌的组织名称。</span><span class="sxs-lookup"><span data-stu-id="cbddb-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="cbddb-182">genres</span><span class="sxs-lookup"><span data-stu-id="cbddb-182">genres</span></span>|<span data-ttu-id="cbddb-183">String 集合</span><span class="sxs-lookup"><span data-stu-id="cbddb-183">String collection</span></span>|<span data-ttu-id="cbddb-184">流派。</span><span class="sxs-lookup"><span data-stu-id="cbddb-184">Genres.</span></span>|
|<span data-ttu-id="cbddb-185">language</span><span class="sxs-lookup"><span data-stu-id="cbddb-185">language</span></span>|<span data-ttu-id="cbddb-186">String</span><span class="sxs-lookup"><span data-stu-id="cbddb-186">String</span></span>|<span data-ttu-id="cbddb-187">语言。</span><span class="sxs-lookup"><span data-stu-id="cbddb-187">Language.</span></span>|
|<span data-ttu-id="cbddb-188">seller</span><span class="sxs-lookup"><span data-stu-id="cbddb-188">seller</span></span>|<span data-ttu-id="cbddb-189">String</span><span class="sxs-lookup"><span data-stu-id="cbddb-189">String</span></span>|<span data-ttu-id="cbddb-190">经销商。</span><span class="sxs-lookup"><span data-stu-id="cbddb-190">Seller.</span></span>|
|<span data-ttu-id="cbddb-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="cbddb-191">totalLicenseCount</span></span>|<span data-ttu-id="cbddb-192">Int32</span><span class="sxs-lookup"><span data-stu-id="cbddb-192">Int32</span></span>|<span data-ttu-id="cbddb-193">许可证总数。</span><span class="sxs-lookup"><span data-stu-id="cbddb-193">Total license count.</span></span>|
|<span data-ttu-id="cbddb-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="cbddb-194">usedLicenseCount</span></span>|<span data-ttu-id="cbddb-195">Int32</span><span class="sxs-lookup"><span data-stu-id="cbddb-195">Int32</span></span>|<span data-ttu-id="cbddb-196">使用的许可证数。</span><span class="sxs-lookup"><span data-stu-id="cbddb-196">Used license count.</span></span>|
|<span data-ttu-id="cbddb-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cbddb-197">roleScopeTagIds</span></span>|<span data-ttu-id="cbddb-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="cbddb-198">String collection</span></span>|<span data-ttu-id="cbddb-199">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="cbddb-199">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="cbddb-200">响应</span><span class="sxs-lookup"><span data-stu-id="cbddb-200">Response</span></span>
<span data-ttu-id="cbddb-201">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cbddb-201">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbddb-202">示例</span><span class="sxs-lookup"><span data-stu-id="cbddb-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbddb-203">请求</span><span class="sxs-lookup"><span data-stu-id="cbddb-203">Request</span></span>
<span data-ttu-id="cbddb-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cbddb-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cbddb-205">响应</span><span class="sxs-lookup"><span data-stu-id="cbddb-205">Response</span></span>
<span data-ttu-id="cbddb-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cbddb-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





