---
title: 更新 iosVppEBook
description: 更新 iosVppEBook 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b8af46ca4e5e75e362043cfc74fc2745072ac033
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823378"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="e8407-103">更新 iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="e8407-103">Update iosVppEBook</span></span>

> <span data-ttu-id="e8407-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e8407-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8407-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e8407-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8407-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e8407-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8407-107">更新 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e8407-107">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8407-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e8407-108">Prerequisites</span></span>
<span data-ttu-id="e8407-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e8407-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8407-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8407-111">Permission type</span></span>|<span data-ttu-id="e8407-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e8407-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8407-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8407-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8407-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8407-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e8407-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8407-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8407-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8407-116">Not supported.</span></span>|
|<span data-ttu-id="e8407-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8407-117">Application</span></span>|<span data-ttu-id="e8407-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8407-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8407-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8407-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="e8407-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8407-120">Request headers</span></span>
|<span data-ttu-id="e8407-121">标头</span><span class="sxs-lookup"><span data-stu-id="e8407-121">Header</span></span>|<span data-ttu-id="e8407-122">值</span><span class="sxs-lookup"><span data-stu-id="e8407-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8407-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8407-123">Authorization</span></span>|<span data-ttu-id="e8407-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e8407-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8407-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e8407-125">Accept</span></span>|<span data-ttu-id="e8407-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8407-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8407-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8407-127">Request body</span></span>
<span data-ttu-id="e8407-128">在请求正文中，提供 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8407-128">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="e8407-129">下表显示了创建 [iosVppEBook](../resources/intune-books-iosvppebook.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e8407-129">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="e8407-130">属性</span><span class="sxs-lookup"><span data-stu-id="e8407-130">Property</span></span>|<span data-ttu-id="e8407-131">类型</span><span class="sxs-lookup"><span data-stu-id="e8407-131">Type</span></span>|<span data-ttu-id="e8407-132">说明</span><span class="sxs-lookup"><span data-stu-id="e8407-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8407-133">id</span><span class="sxs-lookup"><span data-stu-id="e8407-133">id</span></span>|<span data-ttu-id="e8407-134">String</span><span class="sxs-lookup"><span data-stu-id="e8407-134">String</span></span>|<span data-ttu-id="e8407-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e8407-135">Key of the entity.</span></span> <span data-ttu-id="e8407-136">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e8407-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e8407-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e8407-137">displayName</span></span>|<span data-ttu-id="e8407-138">String</span><span class="sxs-lookup"><span data-stu-id="e8407-138">String</span></span>|<span data-ttu-id="e8407-139">电子书的名称。</span><span class="sxs-lookup"><span data-stu-id="e8407-139">Name of the eBook.</span></span> <span data-ttu-id="e8407-140">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e8407-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e8407-141">description</span><span class="sxs-lookup"><span data-stu-id="e8407-141">description</span></span>|<span data-ttu-id="e8407-142">String</span><span class="sxs-lookup"><span data-stu-id="e8407-142">String</span></span>|<span data-ttu-id="e8407-143">说明。</span><span class="sxs-lookup"><span data-stu-id="e8407-143">Description.</span></span> <span data-ttu-id="e8407-144">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e8407-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e8407-145">publisher</span><span class="sxs-lookup"><span data-stu-id="e8407-145">publisher</span></span>|<span data-ttu-id="e8407-146">String</span><span class="sxs-lookup"><span data-stu-id="e8407-146">String</span></span>|<span data-ttu-id="e8407-147">发布者。</span><span class="sxs-lookup"><span data-stu-id="e8407-147">Publisher.</span></span> <span data-ttu-id="e8407-148">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e8407-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e8407-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8407-149">publishedDateTime</span></span>|<span data-ttu-id="e8407-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8407-150">DateTimeOffset</span></span>|<span data-ttu-id="e8407-151">电子书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e8407-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="e8407-152">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e8407-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e8407-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="e8407-153">largeCover</span></span>|[<span data-ttu-id="e8407-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e8407-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e8407-155">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="e8407-155">Book cover.</span></span> <span data-ttu-id="e8407-156">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e8407-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e8407-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8407-157">createdDateTime</span></span>|<span data-ttu-id="e8407-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8407-158">DateTimeOffset</span></span>|<span data-ttu-id="e8407-159">电子书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e8407-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="e8407-160">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e8407-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e8407-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8407-161">lastModifiedDateTime</span></span>|<span data-ttu-id="e8407-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8407-162">DateTimeOffset</span></span>|<span data-ttu-id="e8407-163">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e8407-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="e8407-164">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e8407-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e8407-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e8407-165">informationUrl</span></span>|<span data-ttu-id="e8407-166">String</span><span class="sxs-lookup"><span data-stu-id="e8407-166">String</span></span>|<span data-ttu-id="e8407-167">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="e8407-167">The more information Url.</span></span> <span data-ttu-id="e8407-168">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e8407-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e8407-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e8407-169">privacyInformationUrl</span></span>|<span data-ttu-id="e8407-170">String</span><span class="sxs-lookup"><span data-stu-id="e8407-170">String</span></span>|<span data-ttu-id="e8407-171">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="e8407-171">The privacy statement Url.</span></span> <span data-ttu-id="e8407-172">继承自 [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e8407-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e8407-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="e8407-173">vppTokenId</span></span>|<span data-ttu-id="e8407-174">Guid</span><span class="sxs-lookup"><span data-stu-id="e8407-174">Guid</span></span>|<span data-ttu-id="e8407-175">Vpp 令牌 ID。</span><span class="sxs-lookup"><span data-stu-id="e8407-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="e8407-176">appleId</span><span class="sxs-lookup"><span data-stu-id="e8407-176">appleId</span></span>|<span data-ttu-id="e8407-177">String</span><span class="sxs-lookup"><span data-stu-id="e8407-177">String</span></span>|<span data-ttu-id="e8407-178">与 Vpp 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="e8407-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="e8407-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="e8407-179">vppOrganizationName</span></span>|<span data-ttu-id="e8407-180">String</span><span class="sxs-lookup"><span data-stu-id="e8407-180">String</span></span>|<span data-ttu-id="e8407-181">Vpp 令牌的组织名称。</span><span class="sxs-lookup"><span data-stu-id="e8407-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="e8407-182">genres</span><span class="sxs-lookup"><span data-stu-id="e8407-182">genres</span></span>|<span data-ttu-id="e8407-183">String 集合</span><span class="sxs-lookup"><span data-stu-id="e8407-183">String collection</span></span>|<span data-ttu-id="e8407-184">流派。</span><span class="sxs-lookup"><span data-stu-id="e8407-184">Genres.</span></span>|
|<span data-ttu-id="e8407-185">language</span><span class="sxs-lookup"><span data-stu-id="e8407-185">language</span></span>|<span data-ttu-id="e8407-186">String</span><span class="sxs-lookup"><span data-stu-id="e8407-186">String</span></span>|<span data-ttu-id="e8407-187">语言。</span><span class="sxs-lookup"><span data-stu-id="e8407-187">Language.</span></span>|
|<span data-ttu-id="e8407-188">seller</span><span class="sxs-lookup"><span data-stu-id="e8407-188">seller</span></span>|<span data-ttu-id="e8407-189">String</span><span class="sxs-lookup"><span data-stu-id="e8407-189">String</span></span>|<span data-ttu-id="e8407-190">经销商。</span><span class="sxs-lookup"><span data-stu-id="e8407-190">Seller.</span></span>|
|<span data-ttu-id="e8407-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e8407-191">totalLicenseCount</span></span>|<span data-ttu-id="e8407-192">Int32</span><span class="sxs-lookup"><span data-stu-id="e8407-192">Int32</span></span>|<span data-ttu-id="e8407-193">许可证总数。</span><span class="sxs-lookup"><span data-stu-id="e8407-193">Total license count.</span></span>|
|<span data-ttu-id="e8407-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e8407-194">usedLicenseCount</span></span>|<span data-ttu-id="e8407-195">Int32</span><span class="sxs-lookup"><span data-stu-id="e8407-195">Int32</span></span>|<span data-ttu-id="e8407-196">使用的许可证数。</span><span class="sxs-lookup"><span data-stu-id="e8407-196">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="e8407-197">响应</span><span class="sxs-lookup"><span data-stu-id="e8407-197">Response</span></span>
<span data-ttu-id="e8407-198">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppEBook](../resources/intune-books-iosvppebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e8407-198">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8407-199">示例</span><span class="sxs-lookup"><span data-stu-id="e8407-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8407-200">请求</span><span class="sxs-lookup"><span data-stu-id="e8407-200">Request</span></span>
<span data-ttu-id="e8407-201">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8407-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}
Content-type: application/json
Content-length: 806

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
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

### <a name="response"></a><span data-ttu-id="e8407-202">响应</span><span class="sxs-lookup"><span data-stu-id="e8407-202">Response</span></span>
<span data-ttu-id="e8407-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e8407-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





