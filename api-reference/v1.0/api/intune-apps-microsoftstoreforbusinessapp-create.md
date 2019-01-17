---
title: 创建 microsoftStoreForBusinessApp
description: 创建新的 microsoftStoreForBusinessApp 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b1f3a7147158ba0eb2e5df5c4199491225457ab8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972234"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="f3770-103">创建 microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="f3770-103">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="f3770-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f3770-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3770-105">创建新的 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f3770-105">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f3770-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f3770-106">Prerequisites</span></span>
<span data-ttu-id="f3770-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f3770-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3770-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3770-109">Permission type</span></span>|<span data-ttu-id="f3770-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f3770-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3770-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3770-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f3770-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3770-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f3770-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3770-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3770-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3770-114">Not supported.</span></span>|
|<span data-ttu-id="f3770-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3770-115">Application</span></span>|<span data-ttu-id="f3770-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3770-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3770-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3770-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f3770-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f3770-118">Request headers</span></span>
|<span data-ttu-id="f3770-119">标头</span><span class="sxs-lookup"><span data-stu-id="f3770-119">Header</span></span>|<span data-ttu-id="f3770-120">值</span><span class="sxs-lookup"><span data-stu-id="f3770-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3770-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3770-121">Authorization</span></span>|<span data-ttu-id="f3770-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f3770-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3770-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f3770-123">Accept</span></span>|<span data-ttu-id="f3770-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f3770-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3770-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3770-125">Request body</span></span>
<span data-ttu-id="f3770-126">在请求正文中，提供 microsoftStoreForBusinessApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3770-126">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="f3770-127">下表显示了创建 microsoftStoreForBusinessApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f3770-127">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="f3770-128">属性</span><span class="sxs-lookup"><span data-stu-id="f3770-128">Property</span></span>|<span data-ttu-id="f3770-129">类型</span><span class="sxs-lookup"><span data-stu-id="f3770-129">Type</span></span>|<span data-ttu-id="f3770-130">说明</span><span class="sxs-lookup"><span data-stu-id="f3770-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3770-131">id</span><span class="sxs-lookup"><span data-stu-id="f3770-131">id</span></span>|<span data-ttu-id="f3770-132">String</span><span class="sxs-lookup"><span data-stu-id="f3770-132">String</span></span>|<span data-ttu-id="f3770-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f3770-133">Key of the entity.</span></span> <span data-ttu-id="f3770-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3770-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3770-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f3770-135">displayName</span></span>|<span data-ttu-id="f3770-136">String</span><span class="sxs-lookup"><span data-stu-id="f3770-136">String</span></span>|<span data-ttu-id="f3770-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="f3770-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f3770-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3770-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3770-139">description</span><span class="sxs-lookup"><span data-stu-id="f3770-139">description</span></span>|<span data-ttu-id="f3770-140">String</span><span class="sxs-lookup"><span data-stu-id="f3770-140">String</span></span>|<span data-ttu-id="f3770-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="f3770-141">The description of the app.</span></span> <span data-ttu-id="f3770-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3770-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3770-143">publisher</span><span class="sxs-lookup"><span data-stu-id="f3770-143">publisher</span></span>|<span data-ttu-id="f3770-144">String</span><span class="sxs-lookup"><span data-stu-id="f3770-144">String</span></span>|<span data-ttu-id="f3770-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="f3770-145">The publisher of the app.</span></span> <span data-ttu-id="f3770-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3770-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3770-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f3770-147">largeIcon</span></span>|[<span data-ttu-id="f3770-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f3770-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f3770-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="f3770-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f3770-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3770-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3770-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3770-151">createdDateTime</span></span>|<span data-ttu-id="f3770-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3770-152">DateTimeOffset</span></span>|<span data-ttu-id="f3770-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f3770-153">The date and time the app was created.</span></span> <span data-ttu-id="f3770-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3770-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3770-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3770-155">lastModifiedDateTime</span></span>|<span data-ttu-id="f3770-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3770-156">DateTimeOffset</span></span>|<span data-ttu-id="f3770-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f3770-157">The date and time the app was last modified.</span></span> <span data-ttu-id="f3770-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3770-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3770-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f3770-159">isFeatured</span></span>|<span data-ttu-id="f3770-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3770-160">Boolean</span></span>|<span data-ttu-id="f3770-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3770-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3770-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f3770-162">privacyInformationUrl</span></span>|<span data-ttu-id="f3770-163">String</span><span class="sxs-lookup"><span data-stu-id="f3770-163">String</span></span>|<span data-ttu-id="f3770-164">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="f3770-164">The privacy statement Url.</span></span> <span data-ttu-id="f3770-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3770-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3770-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f3770-166">informationUrl</span></span>|<span data-ttu-id="f3770-167">String</span><span class="sxs-lookup"><span data-stu-id="f3770-167">String</span></span>|<span data-ttu-id="f3770-168">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="f3770-168">The more information Url.</span></span> <span data-ttu-id="f3770-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3770-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3770-170">owner</span><span class="sxs-lookup"><span data-stu-id="f3770-170">owner</span></span>|<span data-ttu-id="f3770-171">String</span><span class="sxs-lookup"><span data-stu-id="f3770-171">String</span></span>|<span data-ttu-id="f3770-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="f3770-172">The owner of the app.</span></span> <span data-ttu-id="f3770-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3770-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3770-174">developer</span><span class="sxs-lookup"><span data-stu-id="f3770-174">developer</span></span>|<span data-ttu-id="f3770-175">String</span><span class="sxs-lookup"><span data-stu-id="f3770-175">String</span></span>|<span data-ttu-id="f3770-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="f3770-176">The developer of the app.</span></span> <span data-ttu-id="f3770-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3770-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3770-178">notes</span><span class="sxs-lookup"><span data-stu-id="f3770-178">notes</span></span>|<span data-ttu-id="f3770-179">String</span><span class="sxs-lookup"><span data-stu-id="f3770-179">String</span></span>|<span data-ttu-id="f3770-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="f3770-180">Notes for the app.</span></span> <span data-ttu-id="f3770-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3770-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3770-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="f3770-182">publishingState</span></span>|[<span data-ttu-id="f3770-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f3770-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f3770-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="f3770-184">The publishing state for the app.</span></span> <span data-ttu-id="f3770-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="f3770-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f3770-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="f3770-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f3770-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="f3770-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f3770-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f3770-188">usedLicenseCount</span></span>|<span data-ttu-id="f3770-189">Int32</span><span class="sxs-lookup"><span data-stu-id="f3770-189">Int32</span></span>|<span data-ttu-id="f3770-190">使用中的适用于企业的 Microsoft Store 许可证数。</span><span class="sxs-lookup"><span data-stu-id="f3770-190">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="f3770-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f3770-191">totalLicenseCount</span></span>|<span data-ttu-id="f3770-192">Int32</span><span class="sxs-lookup"><span data-stu-id="f3770-192">Int32</span></span>|<span data-ttu-id="f3770-193">适用于企业的 Microsoft Store 许可证总数。</span><span class="sxs-lookup"><span data-stu-id="f3770-193">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="f3770-194">productKey</span><span class="sxs-lookup"><span data-stu-id="f3770-194">productKey</span></span>|<span data-ttu-id="f3770-195">String</span><span class="sxs-lookup"><span data-stu-id="f3770-195">String</span></span>|<span data-ttu-id="f3770-196">应用产品密钥</span><span class="sxs-lookup"><span data-stu-id="f3770-196">The app product key</span></span>|
|<span data-ttu-id="f3770-197">licenseType</span><span class="sxs-lookup"><span data-stu-id="f3770-197">licenseType</span></span>|[<span data-ttu-id="f3770-198">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="f3770-198">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="f3770-199">应用程序许可证类型。</span><span class="sxs-lookup"><span data-stu-id="f3770-199">The app license type.</span></span> <span data-ttu-id="f3770-200">可取值为：`offline`、`online`。</span><span class="sxs-lookup"><span data-stu-id="f3770-200">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="f3770-201">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="f3770-201">packageIdentityName</span></span>|<span data-ttu-id="f3770-202">String</span><span class="sxs-lookup"><span data-stu-id="f3770-202">String</span></span>|<span data-ttu-id="f3770-203">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="f3770-203">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="f3770-204">响应</span><span class="sxs-lookup"><span data-stu-id="f3770-204">Response</span></span>
<span data-ttu-id="f3770-205">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f3770-205">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3770-206">示例</span><span class="sxs-lookup"><span data-stu-id="f3770-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="f3770-207">请求</span><span class="sxs-lookup"><span data-stu-id="f3770-207">Request</span></span>
<span data-ttu-id="f3770-208">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f3770-208">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f3770-209">响应</span><span class="sxs-lookup"><span data-stu-id="f3770-209">Response</span></span>
<span data-ttu-id="f3770-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f3770-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



