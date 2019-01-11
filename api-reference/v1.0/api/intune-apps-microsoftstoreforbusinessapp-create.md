---
title: 创建 microsoftStoreForBusinessApp
description: 创建新的 microsoftStoreForBusinessApp 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eff4f4e03c69d866c879aec746c9b4e47d3dbe93
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840479"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="36c44-103">创建 microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="36c44-103">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="36c44-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="36c44-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36c44-105">创建新的 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36c44-105">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36c44-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="36c44-106">Prerequisites</span></span>
<span data-ttu-id="36c44-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="36c44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36c44-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="36c44-109">Permission type</span></span>|<span data-ttu-id="36c44-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="36c44-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36c44-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36c44-111">Delegated (work or school account)</span></span>|<span data-ttu-id="36c44-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36c44-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="36c44-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36c44-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36c44-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="36c44-114">Not supported.</span></span>|
|<span data-ttu-id="36c44-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="36c44-115">Application</span></span>|<span data-ttu-id="36c44-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="36c44-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36c44-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36c44-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="36c44-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="36c44-118">Request headers</span></span>
|<span data-ttu-id="36c44-119">标头</span><span class="sxs-lookup"><span data-stu-id="36c44-119">Header</span></span>|<span data-ttu-id="36c44-120">值</span><span class="sxs-lookup"><span data-stu-id="36c44-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36c44-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="36c44-121">Authorization</span></span>|<span data-ttu-id="36c44-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="36c44-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36c44-123">Accept</span><span class="sxs-lookup"><span data-stu-id="36c44-123">Accept</span></span>|<span data-ttu-id="36c44-124">application/json</span><span class="sxs-lookup"><span data-stu-id="36c44-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36c44-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="36c44-125">Request body</span></span>
<span data-ttu-id="36c44-126">在请求正文中，提供 microsoftStoreForBusinessApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36c44-126">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="36c44-127">下表显示了创建 microsoftStoreForBusinessApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="36c44-127">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="36c44-128">属性</span><span class="sxs-lookup"><span data-stu-id="36c44-128">Property</span></span>|<span data-ttu-id="36c44-129">类型</span><span class="sxs-lookup"><span data-stu-id="36c44-129">Type</span></span>|<span data-ttu-id="36c44-130">说明</span><span class="sxs-lookup"><span data-stu-id="36c44-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36c44-131">id</span><span class="sxs-lookup"><span data-stu-id="36c44-131">id</span></span>|<span data-ttu-id="36c44-132">String</span><span class="sxs-lookup"><span data-stu-id="36c44-132">String</span></span>|<span data-ttu-id="36c44-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="36c44-133">Key of the entity.</span></span> <span data-ttu-id="36c44-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="36c44-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c44-135">displayName</span><span class="sxs-lookup"><span data-stu-id="36c44-135">displayName</span></span>|<span data-ttu-id="36c44-136">String</span><span class="sxs-lookup"><span data-stu-id="36c44-136">String</span></span>|<span data-ttu-id="36c44-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="36c44-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="36c44-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="36c44-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c44-139">description</span><span class="sxs-lookup"><span data-stu-id="36c44-139">description</span></span>|<span data-ttu-id="36c44-140">String</span><span class="sxs-lookup"><span data-stu-id="36c44-140">String</span></span>|<span data-ttu-id="36c44-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="36c44-141">The description of the app.</span></span> <span data-ttu-id="36c44-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="36c44-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c44-143">publisher</span><span class="sxs-lookup"><span data-stu-id="36c44-143">publisher</span></span>|<span data-ttu-id="36c44-144">String</span><span class="sxs-lookup"><span data-stu-id="36c44-144">String</span></span>|<span data-ttu-id="36c44-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="36c44-145">The publisher of the app.</span></span> <span data-ttu-id="36c44-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="36c44-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c44-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="36c44-147">largeIcon</span></span>|[<span data-ttu-id="36c44-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="36c44-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="36c44-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="36c44-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="36c44-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="36c44-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c44-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36c44-151">createdDateTime</span></span>|<span data-ttu-id="36c44-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36c44-152">DateTimeOffset</span></span>|<span data-ttu-id="36c44-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="36c44-153">The date and time the app was created.</span></span> <span data-ttu-id="36c44-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="36c44-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c44-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36c44-155">lastModifiedDateTime</span></span>|<span data-ttu-id="36c44-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36c44-156">DateTimeOffset</span></span>|<span data-ttu-id="36c44-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="36c44-157">The date and time the app was last modified.</span></span> <span data-ttu-id="36c44-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="36c44-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c44-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="36c44-159">isFeatured</span></span>|<span data-ttu-id="36c44-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="36c44-160">Boolean</span></span>|<span data-ttu-id="36c44-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="36c44-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c44-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="36c44-162">privacyInformationUrl</span></span>|<span data-ttu-id="36c44-163">String</span><span class="sxs-lookup"><span data-stu-id="36c44-163">String</span></span>|<span data-ttu-id="36c44-164">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="36c44-164">The privacy statement Url.</span></span> <span data-ttu-id="36c44-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="36c44-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c44-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="36c44-166">informationUrl</span></span>|<span data-ttu-id="36c44-167">String</span><span class="sxs-lookup"><span data-stu-id="36c44-167">String</span></span>|<span data-ttu-id="36c44-168">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="36c44-168">The more information Url.</span></span> <span data-ttu-id="36c44-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="36c44-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c44-170">owner</span><span class="sxs-lookup"><span data-stu-id="36c44-170">owner</span></span>|<span data-ttu-id="36c44-171">String</span><span class="sxs-lookup"><span data-stu-id="36c44-171">String</span></span>|<span data-ttu-id="36c44-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="36c44-172">The owner of the app.</span></span> <span data-ttu-id="36c44-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="36c44-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c44-174">developer</span><span class="sxs-lookup"><span data-stu-id="36c44-174">developer</span></span>|<span data-ttu-id="36c44-175">String</span><span class="sxs-lookup"><span data-stu-id="36c44-175">String</span></span>|<span data-ttu-id="36c44-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="36c44-176">The developer of the app.</span></span> <span data-ttu-id="36c44-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="36c44-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c44-178">notes</span><span class="sxs-lookup"><span data-stu-id="36c44-178">notes</span></span>|<span data-ttu-id="36c44-179">String</span><span class="sxs-lookup"><span data-stu-id="36c44-179">String</span></span>|<span data-ttu-id="36c44-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="36c44-180">Notes for the app.</span></span> <span data-ttu-id="36c44-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="36c44-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c44-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="36c44-182">publishingState</span></span>|[<span data-ttu-id="36c44-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="36c44-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="36c44-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="36c44-184">The publishing state for the app.</span></span> <span data-ttu-id="36c44-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="36c44-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="36c44-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="36c44-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="36c44-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="36c44-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="36c44-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="36c44-188">usedLicenseCount</span></span>|<span data-ttu-id="36c44-189">Int32</span><span class="sxs-lookup"><span data-stu-id="36c44-189">Int32</span></span>|<span data-ttu-id="36c44-190">使用中的适用于企业的 Microsoft Store 许可证数。</span><span class="sxs-lookup"><span data-stu-id="36c44-190">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="36c44-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="36c44-191">totalLicenseCount</span></span>|<span data-ttu-id="36c44-192">Int32</span><span class="sxs-lookup"><span data-stu-id="36c44-192">Int32</span></span>|<span data-ttu-id="36c44-193">适用于企业的 Microsoft Store 许可证总数。</span><span class="sxs-lookup"><span data-stu-id="36c44-193">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="36c44-194">productKey</span><span class="sxs-lookup"><span data-stu-id="36c44-194">productKey</span></span>|<span data-ttu-id="36c44-195">String</span><span class="sxs-lookup"><span data-stu-id="36c44-195">String</span></span>|<span data-ttu-id="36c44-196">应用产品密钥</span><span class="sxs-lookup"><span data-stu-id="36c44-196">The app product key</span></span>|
|<span data-ttu-id="36c44-197">licenseType</span><span class="sxs-lookup"><span data-stu-id="36c44-197">licenseType</span></span>|[<span data-ttu-id="36c44-198">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="36c44-198">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="36c44-199">应用程序许可证类型。</span><span class="sxs-lookup"><span data-stu-id="36c44-199">The app license type.</span></span> <span data-ttu-id="36c44-200">可取值为：`offline`、`online`。</span><span class="sxs-lookup"><span data-stu-id="36c44-200">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="36c44-201">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="36c44-201">packageIdentityName</span></span>|<span data-ttu-id="36c44-202">String</span><span class="sxs-lookup"><span data-stu-id="36c44-202">String</span></span>|<span data-ttu-id="36c44-203">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="36c44-203">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="36c44-204">响应</span><span class="sxs-lookup"><span data-stu-id="36c44-204">Response</span></span>
<span data-ttu-id="36c44-205">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36c44-205">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36c44-206">示例</span><span class="sxs-lookup"><span data-stu-id="36c44-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="36c44-207">请求</span><span class="sxs-lookup"><span data-stu-id="36c44-207">Request</span></span>
<span data-ttu-id="36c44-208">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36c44-208">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="36c44-209">响应</span><span class="sxs-lookup"><span data-stu-id="36c44-209">Response</span></span>
<span data-ttu-id="36c44-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="36c44-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



