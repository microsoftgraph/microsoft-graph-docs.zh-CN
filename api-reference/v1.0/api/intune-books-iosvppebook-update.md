---
title: 更新 iosVppEBook
description: 更新 iosVppEBook 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cba3e1eb6fa3b6398006fb9db3c50f8c644b93da
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515635"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="f38dc-103">更新 iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="f38dc-103">Update iosVppEBook</span></span>

<span data-ttu-id="f38dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f38dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f38dc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f38dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f38dc-106">更新 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f38dc-106">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f38dc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f38dc-107">Prerequisites</span></span>
<span data-ttu-id="f38dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f38dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f38dc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f38dc-110">Permission type</span></span>|<span data-ttu-id="f38dc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f38dc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f38dc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f38dc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f38dc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f38dc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f38dc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f38dc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f38dc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f38dc-115">Not supported.</span></span>|
|<span data-ttu-id="f38dc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f38dc-116">Application</span></span>|<span data-ttu-id="f38dc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f38dc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f38dc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f38dc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="f38dc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f38dc-119">Request headers</span></span>
|<span data-ttu-id="f38dc-120">标头</span><span class="sxs-lookup"><span data-stu-id="f38dc-120">Header</span></span>|<span data-ttu-id="f38dc-121">值</span><span class="sxs-lookup"><span data-stu-id="f38dc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f38dc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f38dc-122">Authorization</span></span>|<span data-ttu-id="f38dc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f38dc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f38dc-124">接受</span><span class="sxs-lookup"><span data-stu-id="f38dc-124">Accept</span></span>|<span data-ttu-id="f38dc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f38dc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f38dc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f38dc-126">Request body</span></span>
<span data-ttu-id="f38dc-127">在请求正文中，提供 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f38dc-127">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="f38dc-128">下表显示了创建 [iosVppEBook](../resources/intune-books-iosvppebook.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f38dc-128">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="f38dc-129">属性</span><span class="sxs-lookup"><span data-stu-id="f38dc-129">Property</span></span>|<span data-ttu-id="f38dc-130">类型</span><span class="sxs-lookup"><span data-stu-id="f38dc-130">Type</span></span>|<span data-ttu-id="f38dc-131">说明</span><span class="sxs-lookup"><span data-stu-id="f38dc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f38dc-132">id</span><span class="sxs-lookup"><span data-stu-id="f38dc-132">id</span></span>|<span data-ttu-id="f38dc-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f38dc-133">String</span></span>|<span data-ttu-id="f38dc-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f38dc-134">Key of the entity.</span></span> <span data-ttu-id="f38dc-135">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f38dc-135">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f38dc-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f38dc-136">displayName</span></span>|<span data-ttu-id="f38dc-137">字符串</span><span class="sxs-lookup"><span data-stu-id="f38dc-137">String</span></span>|<span data-ttu-id="f38dc-138">电子图书的名称。</span><span class="sxs-lookup"><span data-stu-id="f38dc-138">Name of the eBook.</span></span> <span data-ttu-id="f38dc-139">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f38dc-139">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f38dc-140">说明</span><span class="sxs-lookup"><span data-stu-id="f38dc-140">description</span></span>|<span data-ttu-id="f38dc-141">String</span><span class="sxs-lookup"><span data-stu-id="f38dc-141">String</span></span>|<span data-ttu-id="f38dc-142">说明。</span><span class="sxs-lookup"><span data-stu-id="f38dc-142">Description.</span></span> <span data-ttu-id="f38dc-143">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f38dc-143">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f38dc-144">publisher</span><span class="sxs-lookup"><span data-stu-id="f38dc-144">publisher</span></span>|<span data-ttu-id="f38dc-145">字符串</span><span class="sxs-lookup"><span data-stu-id="f38dc-145">String</span></span>|<span data-ttu-id="f38dc-146">发布者。</span><span class="sxs-lookup"><span data-stu-id="f38dc-146">Publisher.</span></span> <span data-ttu-id="f38dc-147">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f38dc-147">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f38dc-148">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="f38dc-148">publishedDateTime</span></span>|<span data-ttu-id="f38dc-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f38dc-149">DateTimeOffset</span></span>|<span data-ttu-id="f38dc-150">电子图书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f38dc-150">The date and time when the eBook was published.</span></span> <span data-ttu-id="f38dc-151">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f38dc-151">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f38dc-152">largeCover</span><span class="sxs-lookup"><span data-stu-id="f38dc-152">largeCover</span></span>|[<span data-ttu-id="f38dc-153">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f38dc-153">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f38dc-154">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="f38dc-154">Book cover.</span></span> <span data-ttu-id="f38dc-155">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f38dc-155">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f38dc-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f38dc-156">createdDateTime</span></span>|<span data-ttu-id="f38dc-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f38dc-157">DateTimeOffset</span></span>|<span data-ttu-id="f38dc-158">电子图书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f38dc-158">The date and time when the eBook file was created.</span></span> <span data-ttu-id="f38dc-159">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f38dc-159">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f38dc-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f38dc-160">lastModifiedDateTime</span></span>|<span data-ttu-id="f38dc-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f38dc-161">DateTimeOffset</span></span>|<span data-ttu-id="f38dc-162">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f38dc-162">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="f38dc-163">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f38dc-163">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f38dc-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f38dc-164">informationUrl</span></span>|<span data-ttu-id="f38dc-165">字符串</span><span class="sxs-lookup"><span data-stu-id="f38dc-165">String</span></span>|<span data-ttu-id="f38dc-166">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="f38dc-166">The more information Url.</span></span> <span data-ttu-id="f38dc-167">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f38dc-167">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f38dc-168">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f38dc-168">privacyInformationUrl</span></span>|<span data-ttu-id="f38dc-169">字符串</span><span class="sxs-lookup"><span data-stu-id="f38dc-169">String</span></span>|<span data-ttu-id="f38dc-170">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="f38dc-170">The privacy statement Url.</span></span> <span data-ttu-id="f38dc-171">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f38dc-171">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="f38dc-172">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="f38dc-172">vppTokenId</span></span>|<span data-ttu-id="f38dc-173">Guid</span><span class="sxs-lookup"><span data-stu-id="f38dc-173">Guid</span></span>|<span data-ttu-id="f38dc-174">Vpp 令牌 ID。</span><span class="sxs-lookup"><span data-stu-id="f38dc-174">The Vpp token ID.</span></span>|
|<span data-ttu-id="f38dc-175">appleId</span><span class="sxs-lookup"><span data-stu-id="f38dc-175">appleId</span></span>|<span data-ttu-id="f38dc-176">字符串</span><span class="sxs-lookup"><span data-stu-id="f38dc-176">String</span></span>|<span data-ttu-id="f38dc-177">与 Vpp 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="f38dc-177">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="f38dc-178">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="f38dc-178">vppOrganizationName</span></span>|<span data-ttu-id="f38dc-179">字符串</span><span class="sxs-lookup"><span data-stu-id="f38dc-179">String</span></span>|<span data-ttu-id="f38dc-180">Vpp 令牌的组织名称。</span><span class="sxs-lookup"><span data-stu-id="f38dc-180">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="f38dc-181">genres</span><span class="sxs-lookup"><span data-stu-id="f38dc-181">genres</span></span>|<span data-ttu-id="f38dc-182">String 集合</span><span class="sxs-lookup"><span data-stu-id="f38dc-182">String collection</span></span>|<span data-ttu-id="f38dc-183">流派。</span><span class="sxs-lookup"><span data-stu-id="f38dc-183">Genres.</span></span>|
|<span data-ttu-id="f38dc-184">language</span><span class="sxs-lookup"><span data-stu-id="f38dc-184">language</span></span>|<span data-ttu-id="f38dc-185">字符串</span><span class="sxs-lookup"><span data-stu-id="f38dc-185">String</span></span>|<span data-ttu-id="f38dc-186">语言。</span><span class="sxs-lookup"><span data-stu-id="f38dc-186">Language.</span></span>|
|<span data-ttu-id="f38dc-187">seller</span><span class="sxs-lookup"><span data-stu-id="f38dc-187">seller</span></span>|<span data-ttu-id="f38dc-188">String</span><span class="sxs-lookup"><span data-stu-id="f38dc-188">String</span></span>|<span data-ttu-id="f38dc-189">经销商。</span><span class="sxs-lookup"><span data-stu-id="f38dc-189">Seller.</span></span>|
|<span data-ttu-id="f38dc-190">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f38dc-190">totalLicenseCount</span></span>|<span data-ttu-id="f38dc-191">Int32</span><span class="sxs-lookup"><span data-stu-id="f38dc-191">Int32</span></span>|<span data-ttu-id="f38dc-192">许可证总数。</span><span class="sxs-lookup"><span data-stu-id="f38dc-192">Total license count.</span></span>|
|<span data-ttu-id="f38dc-193">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f38dc-193">usedLicenseCount</span></span>|<span data-ttu-id="f38dc-194">Int32</span><span class="sxs-lookup"><span data-stu-id="f38dc-194">Int32</span></span>|<span data-ttu-id="f38dc-195">使用的许可证数。</span><span class="sxs-lookup"><span data-stu-id="f38dc-195">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="f38dc-196">响应</span><span class="sxs-lookup"><span data-stu-id="f38dc-196">Response</span></span>
<span data-ttu-id="f38dc-197">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f38dc-197">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f38dc-198">示例</span><span class="sxs-lookup"><span data-stu-id="f38dc-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="f38dc-199">请求</span><span class="sxs-lookup"><span data-stu-id="f38dc-199">Request</span></span>
<span data-ttu-id="f38dc-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f38dc-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f38dc-201">响应</span><span class="sxs-lookup"><span data-stu-id="f38dc-201">Response</span></span>
<span data-ttu-id="f38dc-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f38dc-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




