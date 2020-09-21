---
title: 创建 microsoftStoreForBusinessApp
description: 创建新的 microsoftStoreForBusinessApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc3b4f8b4a7e82aa888cb4b843e15499724d6bec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073227"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="3ac59-103">创建 microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="3ac59-103">Create microsoftStoreForBusinessApp</span></span>

<span data-ttu-id="3ac59-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ac59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ac59-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ac59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ac59-106">创建新的 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3ac59-106">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ac59-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3ac59-107">Prerequisites</span></span>
<span data-ttu-id="3ac59-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ac59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ac59-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ac59-110">Permission type</span></span>|<span data-ttu-id="3ac59-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3ac59-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ac59-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ac59-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ac59-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ac59-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3ac59-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ac59-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ac59-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ac59-115">Not supported.</span></span>|
|<span data-ttu-id="3ac59-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ac59-116">Application</span></span>|<span data-ttu-id="3ac59-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ac59-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ac59-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ac59-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3ac59-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ac59-119">Request headers</span></span>
|<span data-ttu-id="3ac59-120">标头</span><span class="sxs-lookup"><span data-stu-id="3ac59-120">Header</span></span>|<span data-ttu-id="3ac59-121">值</span><span class="sxs-lookup"><span data-stu-id="3ac59-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ac59-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ac59-122">Authorization</span></span>|<span data-ttu-id="3ac59-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3ac59-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ac59-124">接受</span><span class="sxs-lookup"><span data-stu-id="3ac59-124">Accept</span></span>|<span data-ttu-id="3ac59-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3ac59-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ac59-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ac59-126">Request body</span></span>
<span data-ttu-id="3ac59-127">在请求正文中，提供 microsoftStoreForBusinessApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ac59-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="3ac59-128">下表显示了创建 microsoftStoreForBusinessApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3ac59-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="3ac59-129">属性</span><span class="sxs-lookup"><span data-stu-id="3ac59-129">Property</span></span>|<span data-ttu-id="3ac59-130">类型</span><span class="sxs-lookup"><span data-stu-id="3ac59-130">Type</span></span>|<span data-ttu-id="3ac59-131">说明</span><span class="sxs-lookup"><span data-stu-id="3ac59-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ac59-132">id</span><span class="sxs-lookup"><span data-stu-id="3ac59-132">id</span></span>|<span data-ttu-id="3ac59-133">String</span><span class="sxs-lookup"><span data-stu-id="3ac59-133">String</span></span>|<span data-ttu-id="3ac59-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3ac59-134">Key of the entity.</span></span> <span data-ttu-id="3ac59-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3ac59-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ac59-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3ac59-136">displayName</span></span>|<span data-ttu-id="3ac59-137">String</span><span class="sxs-lookup"><span data-stu-id="3ac59-137">String</span></span>|<span data-ttu-id="3ac59-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="3ac59-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3ac59-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3ac59-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ac59-140">description</span><span class="sxs-lookup"><span data-stu-id="3ac59-140">description</span></span>|<span data-ttu-id="3ac59-141">String</span><span class="sxs-lookup"><span data-stu-id="3ac59-141">String</span></span>|<span data-ttu-id="3ac59-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="3ac59-142">The description of the app.</span></span> <span data-ttu-id="3ac59-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3ac59-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ac59-144">publisher</span><span class="sxs-lookup"><span data-stu-id="3ac59-144">publisher</span></span>|<span data-ttu-id="3ac59-145">String</span><span class="sxs-lookup"><span data-stu-id="3ac59-145">String</span></span>|<span data-ttu-id="3ac59-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="3ac59-146">The publisher of the app.</span></span> <span data-ttu-id="3ac59-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3ac59-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ac59-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3ac59-148">largeIcon</span></span>|[<span data-ttu-id="3ac59-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3ac59-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3ac59-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="3ac59-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3ac59-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3ac59-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ac59-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ac59-152">createdDateTime</span></span>|<span data-ttu-id="3ac59-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ac59-153">DateTimeOffset</span></span>|<span data-ttu-id="3ac59-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3ac59-154">The date and time the app was created.</span></span> <span data-ttu-id="3ac59-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3ac59-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ac59-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ac59-156">lastModifiedDateTime</span></span>|<span data-ttu-id="3ac59-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ac59-157">DateTimeOffset</span></span>|<span data-ttu-id="3ac59-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3ac59-158">The date and time the app was last modified.</span></span> <span data-ttu-id="3ac59-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3ac59-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ac59-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3ac59-160">isFeatured</span></span>|<span data-ttu-id="3ac59-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ac59-161">Boolean</span></span>|<span data-ttu-id="3ac59-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3ac59-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ac59-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3ac59-163">privacyInformationUrl</span></span>|<span data-ttu-id="3ac59-164">String</span><span class="sxs-lookup"><span data-stu-id="3ac59-164">String</span></span>|<span data-ttu-id="3ac59-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="3ac59-165">The privacy statement Url.</span></span> <span data-ttu-id="3ac59-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3ac59-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ac59-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3ac59-167">informationUrl</span></span>|<span data-ttu-id="3ac59-168">String</span><span class="sxs-lookup"><span data-stu-id="3ac59-168">String</span></span>|<span data-ttu-id="3ac59-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="3ac59-169">The more information Url.</span></span> <span data-ttu-id="3ac59-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3ac59-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ac59-171">owner</span><span class="sxs-lookup"><span data-stu-id="3ac59-171">owner</span></span>|<span data-ttu-id="3ac59-172">String</span><span class="sxs-lookup"><span data-stu-id="3ac59-172">String</span></span>|<span data-ttu-id="3ac59-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="3ac59-173">The owner of the app.</span></span> <span data-ttu-id="3ac59-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3ac59-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ac59-175">developer</span><span class="sxs-lookup"><span data-stu-id="3ac59-175">developer</span></span>|<span data-ttu-id="3ac59-176">String</span><span class="sxs-lookup"><span data-stu-id="3ac59-176">String</span></span>|<span data-ttu-id="3ac59-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="3ac59-177">The developer of the app.</span></span> <span data-ttu-id="3ac59-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3ac59-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ac59-179">notes</span><span class="sxs-lookup"><span data-stu-id="3ac59-179">notes</span></span>|<span data-ttu-id="3ac59-180">String</span><span class="sxs-lookup"><span data-stu-id="3ac59-180">String</span></span>|<span data-ttu-id="3ac59-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="3ac59-181">Notes for the app.</span></span> <span data-ttu-id="3ac59-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3ac59-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ac59-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="3ac59-183">publishingState</span></span>|[<span data-ttu-id="3ac59-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3ac59-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3ac59-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="3ac59-185">The publishing state for the app.</span></span> <span data-ttu-id="3ac59-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="3ac59-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3ac59-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="3ac59-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3ac59-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="3ac59-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3ac59-189">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3ac59-189">usedLicenseCount</span></span>|<span data-ttu-id="3ac59-190">Int32</span><span class="sxs-lookup"><span data-stu-id="3ac59-190">Int32</span></span>|<span data-ttu-id="3ac59-191">使用中的适用于企业的 Microsoft Store 许可证数。</span><span class="sxs-lookup"><span data-stu-id="3ac59-191">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="3ac59-192">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3ac59-192">totalLicenseCount</span></span>|<span data-ttu-id="3ac59-193">Int32</span><span class="sxs-lookup"><span data-stu-id="3ac59-193">Int32</span></span>|<span data-ttu-id="3ac59-194">适用于企业的 Microsoft Store 许可证总数。</span><span class="sxs-lookup"><span data-stu-id="3ac59-194">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="3ac59-195">productKey</span><span class="sxs-lookup"><span data-stu-id="3ac59-195">productKey</span></span>|<span data-ttu-id="3ac59-196">String</span><span class="sxs-lookup"><span data-stu-id="3ac59-196">String</span></span>|<span data-ttu-id="3ac59-197">应用产品密钥</span><span class="sxs-lookup"><span data-stu-id="3ac59-197">The app product key</span></span>|
|<span data-ttu-id="3ac59-198">licenseType</span><span class="sxs-lookup"><span data-stu-id="3ac59-198">licenseType</span></span>|[<span data-ttu-id="3ac59-199">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="3ac59-199">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="3ac59-200">应用程序许可证类型。</span><span class="sxs-lookup"><span data-stu-id="3ac59-200">The app license type.</span></span> <span data-ttu-id="3ac59-201">可取值为：`offline`、`online`。</span><span class="sxs-lookup"><span data-stu-id="3ac59-201">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="3ac59-202">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="3ac59-202">packageIdentityName</span></span>|<span data-ttu-id="3ac59-203">String</span><span class="sxs-lookup"><span data-stu-id="3ac59-203">String</span></span>|<span data-ttu-id="3ac59-204">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="3ac59-204">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="3ac59-205">响应</span><span class="sxs-lookup"><span data-stu-id="3ac59-205">Response</span></span>
<span data-ttu-id="3ac59-206">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3ac59-206">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ac59-207">示例</span><span class="sxs-lookup"><span data-stu-id="3ac59-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ac59-208">请求</span><span class="sxs-lookup"><span data-stu-id="3ac59-208">Request</span></span>
<span data-ttu-id="3ac59-209">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ac59-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 769

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="3ac59-210">响应</span><span class="sxs-lookup"><span data-stu-id="3ac59-210">Response</span></span>
<span data-ttu-id="3ac59-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3ac59-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 941

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```









