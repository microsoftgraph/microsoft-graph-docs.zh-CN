---
title: 更新 iosVppEBook
description: 更新 iosVppEBook 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7279b8da1ffe159dba56f4a5a10345243703da1c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393744"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="cec95-103">更新 iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="cec95-103">Update iosVppEBook</span></span>

> <span data-ttu-id="cec95-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="cec95-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cec95-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cec95-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cec95-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cec95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cec95-107">更新 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cec95-107">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cec95-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cec95-108">Prerequisites</span></span>
<span data-ttu-id="cec95-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cec95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cec95-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cec95-111">Permission type</span></span>|<span data-ttu-id="cec95-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cec95-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cec95-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cec95-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cec95-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cec95-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cec95-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cec95-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cec95-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cec95-116">Not supported.</span></span>|
|<span data-ttu-id="cec95-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cec95-117">Application</span></span>|<span data-ttu-id="cec95-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cec95-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cec95-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cec95-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="cec95-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cec95-120">Request headers</span></span>
|<span data-ttu-id="cec95-121">标头</span><span class="sxs-lookup"><span data-stu-id="cec95-121">Header</span></span>|<span data-ttu-id="cec95-122">值</span><span class="sxs-lookup"><span data-stu-id="cec95-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cec95-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cec95-123">Authorization</span></span>|<span data-ttu-id="cec95-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cec95-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cec95-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cec95-125">Accept</span></span>|<span data-ttu-id="cec95-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cec95-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cec95-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cec95-127">Request body</span></span>
<span data-ttu-id="cec95-128">在请求正文中，提供 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cec95-128">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="cec95-129">下表显示了创建 [iosVppEBook](../resources/intune-books-iosvppebook.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cec95-129">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="cec95-130">属性</span><span class="sxs-lookup"><span data-stu-id="cec95-130">Property</span></span>|<span data-ttu-id="cec95-131">类型</span><span class="sxs-lookup"><span data-stu-id="cec95-131">Type</span></span>|<span data-ttu-id="cec95-132">说明</span><span class="sxs-lookup"><span data-stu-id="cec95-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cec95-133">id</span><span class="sxs-lookup"><span data-stu-id="cec95-133">id</span></span>|<span data-ttu-id="cec95-134">String</span><span class="sxs-lookup"><span data-stu-id="cec95-134">String</span></span>|<span data-ttu-id="cec95-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cec95-135">Key of the entity.</span></span> <span data-ttu-id="cec95-136">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cec95-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cec95-137">displayName</span><span class="sxs-lookup"><span data-stu-id="cec95-137">displayName</span></span>|<span data-ttu-id="cec95-138">String</span><span class="sxs-lookup"><span data-stu-id="cec95-138">String</span></span>|<span data-ttu-id="cec95-139">电子书的名称。</span><span class="sxs-lookup"><span data-stu-id="cec95-139">Name of the eBook.</span></span> <span data-ttu-id="cec95-140">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cec95-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cec95-141">description</span><span class="sxs-lookup"><span data-stu-id="cec95-141">description</span></span>|<span data-ttu-id="cec95-142">String</span><span class="sxs-lookup"><span data-stu-id="cec95-142">String</span></span>|<span data-ttu-id="cec95-143">说明。</span><span class="sxs-lookup"><span data-stu-id="cec95-143">Description.</span></span> <span data-ttu-id="cec95-144">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cec95-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cec95-145">publisher</span><span class="sxs-lookup"><span data-stu-id="cec95-145">publisher</span></span>|<span data-ttu-id="cec95-146">String</span><span class="sxs-lookup"><span data-stu-id="cec95-146">String</span></span>|<span data-ttu-id="cec95-147">发布者。</span><span class="sxs-lookup"><span data-stu-id="cec95-147">Publisher.</span></span> <span data-ttu-id="cec95-148">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cec95-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cec95-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="cec95-149">publishedDateTime</span></span>|<span data-ttu-id="cec95-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cec95-150">DateTimeOffset</span></span>|<span data-ttu-id="cec95-151">电子书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cec95-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="cec95-152">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cec95-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cec95-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="cec95-153">largeCover</span></span>|[<span data-ttu-id="cec95-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cec95-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cec95-155">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="cec95-155">Book cover.</span></span> <span data-ttu-id="cec95-156">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cec95-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cec95-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cec95-157">createdDateTime</span></span>|<span data-ttu-id="cec95-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cec95-158">DateTimeOffset</span></span>|<span data-ttu-id="cec95-159">电子书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cec95-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="cec95-160">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cec95-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cec95-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cec95-161">lastModifiedDateTime</span></span>|<span data-ttu-id="cec95-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cec95-162">DateTimeOffset</span></span>|<span data-ttu-id="cec95-163">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cec95-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="cec95-164">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cec95-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cec95-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cec95-165">informationUrl</span></span>|<span data-ttu-id="cec95-166">String</span><span class="sxs-lookup"><span data-stu-id="cec95-166">String</span></span>|<span data-ttu-id="cec95-167">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="cec95-167">The more information Url.</span></span> <span data-ttu-id="cec95-168">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cec95-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cec95-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cec95-169">privacyInformationUrl</span></span>|<span data-ttu-id="cec95-170">String</span><span class="sxs-lookup"><span data-stu-id="cec95-170">String</span></span>|<span data-ttu-id="cec95-171">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="cec95-171">The privacy statement Url.</span></span> <span data-ttu-id="cec95-172">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cec95-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="cec95-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="cec95-173">vppTokenId</span></span>|<span data-ttu-id="cec95-174">Guid</span><span class="sxs-lookup"><span data-stu-id="cec95-174">Guid</span></span>|<span data-ttu-id="cec95-175">Vpp 令牌 ID。</span><span class="sxs-lookup"><span data-stu-id="cec95-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="cec95-176">appleId</span><span class="sxs-lookup"><span data-stu-id="cec95-176">appleId</span></span>|<span data-ttu-id="cec95-177">String</span><span class="sxs-lookup"><span data-stu-id="cec95-177">String</span></span>|<span data-ttu-id="cec95-178">与 Vpp 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="cec95-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="cec95-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="cec95-179">vppOrganizationName</span></span>|<span data-ttu-id="cec95-180">String</span><span class="sxs-lookup"><span data-stu-id="cec95-180">String</span></span>|<span data-ttu-id="cec95-181">Vpp 令牌的组织名称。</span><span class="sxs-lookup"><span data-stu-id="cec95-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="cec95-182">genres</span><span class="sxs-lookup"><span data-stu-id="cec95-182">genres</span></span>|<span data-ttu-id="cec95-183">String 集合</span><span class="sxs-lookup"><span data-stu-id="cec95-183">String collection</span></span>|<span data-ttu-id="cec95-184">流派。</span><span class="sxs-lookup"><span data-stu-id="cec95-184">Genres.</span></span>|
|<span data-ttu-id="cec95-185">language</span><span class="sxs-lookup"><span data-stu-id="cec95-185">language</span></span>|<span data-ttu-id="cec95-186">String</span><span class="sxs-lookup"><span data-stu-id="cec95-186">String</span></span>|<span data-ttu-id="cec95-187">语言。</span><span class="sxs-lookup"><span data-stu-id="cec95-187">Language.</span></span>|
|<span data-ttu-id="cec95-188">seller</span><span class="sxs-lookup"><span data-stu-id="cec95-188">seller</span></span>|<span data-ttu-id="cec95-189">String</span><span class="sxs-lookup"><span data-stu-id="cec95-189">String</span></span>|<span data-ttu-id="cec95-190">经销商。</span><span class="sxs-lookup"><span data-stu-id="cec95-190">Seller.</span></span>|
|<span data-ttu-id="cec95-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="cec95-191">totalLicenseCount</span></span>|<span data-ttu-id="cec95-192">Int32</span><span class="sxs-lookup"><span data-stu-id="cec95-192">Int32</span></span>|<span data-ttu-id="cec95-193">许可证总数。</span><span class="sxs-lookup"><span data-stu-id="cec95-193">Total license count.</span></span>|
|<span data-ttu-id="cec95-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="cec95-194">usedLicenseCount</span></span>|<span data-ttu-id="cec95-195">Int32</span><span class="sxs-lookup"><span data-stu-id="cec95-195">Int32</span></span>|<span data-ttu-id="cec95-196">使用的许可证数。</span><span class="sxs-lookup"><span data-stu-id="cec95-196">Used license count.</span></span>|
|<span data-ttu-id="cec95-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cec95-197">roleScopeTagIds</span></span>|<span data-ttu-id="cec95-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="cec95-198">String collection</span></span>|<span data-ttu-id="cec95-199">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="cec95-199">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="cec95-200">响应</span><span class="sxs-lookup"><span data-stu-id="cec95-200">Response</span></span>
<span data-ttu-id="cec95-201">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cec95-201">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cec95-202">示例</span><span class="sxs-lookup"><span data-stu-id="cec95-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="cec95-203">请求</span><span class="sxs-lookup"><span data-stu-id="cec95-203">Request</span></span>
<span data-ttu-id="cec95-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cec95-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cec95-205">响应</span><span class="sxs-lookup"><span data-stu-id="cec95-205">Response</span></span>
<span data-ttu-id="cec95-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cec95-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




