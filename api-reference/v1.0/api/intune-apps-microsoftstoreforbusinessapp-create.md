---
title: 创建 microsoftStoreForBusinessApp
description: 创建新的 microsoftStoreForBusinessApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7dccd660fb741254d4b600e73f35a17864a9ba29
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759768"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="543cb-103">创建 microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="543cb-103">Create microsoftStoreForBusinessApp</span></span>

<span data-ttu-id="543cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="543cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="543cb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="543cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="543cb-106">创建新的 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="543cb-106">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="543cb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="543cb-107">Prerequisites</span></span>
<span data-ttu-id="543cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="543cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="543cb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="543cb-110">Permission type</span></span>|<span data-ttu-id="543cb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="543cb-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="543cb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="543cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="543cb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="543cb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="543cb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="543cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="543cb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="543cb-115">Not supported.</span></span>|
|<span data-ttu-id="543cb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="543cb-116">Application</span></span>|<span data-ttu-id="543cb-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="543cb-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="543cb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="543cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="543cb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="543cb-119">Request headers</span></span>
|<span data-ttu-id="543cb-120">标头</span><span class="sxs-lookup"><span data-stu-id="543cb-120">Header</span></span>|<span data-ttu-id="543cb-121">值</span><span class="sxs-lookup"><span data-stu-id="543cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="543cb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="543cb-122">Authorization</span></span>|<span data-ttu-id="543cb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="543cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="543cb-124">接受</span><span class="sxs-lookup"><span data-stu-id="543cb-124">Accept</span></span>|<span data-ttu-id="543cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="543cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="543cb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="543cb-126">Request body</span></span>
<span data-ttu-id="543cb-127">在请求正文中，提供 microsoftStoreForBusinessApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="543cb-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="543cb-128">下表显示了创建 microsoftStoreForBusinessApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="543cb-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="543cb-129">属性</span><span class="sxs-lookup"><span data-stu-id="543cb-129">Property</span></span>|<span data-ttu-id="543cb-130">类型</span><span class="sxs-lookup"><span data-stu-id="543cb-130">Type</span></span>|<span data-ttu-id="543cb-131">说明</span><span class="sxs-lookup"><span data-stu-id="543cb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="543cb-132">id</span><span class="sxs-lookup"><span data-stu-id="543cb-132">id</span></span>|<span data-ttu-id="543cb-133">String</span><span class="sxs-lookup"><span data-stu-id="543cb-133">String</span></span>|<span data-ttu-id="543cb-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="543cb-134">Key of the entity.</span></span> <span data-ttu-id="543cb-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="543cb-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="543cb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="543cb-136">displayName</span></span>|<span data-ttu-id="543cb-137">String</span><span class="sxs-lookup"><span data-stu-id="543cb-137">String</span></span>|<span data-ttu-id="543cb-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="543cb-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="543cb-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="543cb-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="543cb-140">description</span><span class="sxs-lookup"><span data-stu-id="543cb-140">description</span></span>|<span data-ttu-id="543cb-141">String</span><span class="sxs-lookup"><span data-stu-id="543cb-141">String</span></span>|<span data-ttu-id="543cb-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="543cb-142">The description of the app.</span></span> <span data-ttu-id="543cb-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="543cb-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="543cb-144">publisher</span><span class="sxs-lookup"><span data-stu-id="543cb-144">publisher</span></span>|<span data-ttu-id="543cb-145">String</span><span class="sxs-lookup"><span data-stu-id="543cb-145">String</span></span>|<span data-ttu-id="543cb-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="543cb-146">The publisher of the app.</span></span> <span data-ttu-id="543cb-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="543cb-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="543cb-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="543cb-148">largeIcon</span></span>|[<span data-ttu-id="543cb-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="543cb-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="543cb-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="543cb-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="543cb-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="543cb-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="543cb-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="543cb-152">createdDateTime</span></span>|<span data-ttu-id="543cb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="543cb-153">DateTimeOffset</span></span>|<span data-ttu-id="543cb-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="543cb-154">The date and time the app was created.</span></span> <span data-ttu-id="543cb-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="543cb-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="543cb-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="543cb-156">lastModifiedDateTime</span></span>|<span data-ttu-id="543cb-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="543cb-157">DateTimeOffset</span></span>|<span data-ttu-id="543cb-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="543cb-158">The date and time the app was last modified.</span></span> <span data-ttu-id="543cb-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="543cb-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="543cb-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="543cb-160">isFeatured</span></span>|<span data-ttu-id="543cb-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="543cb-161">Boolean</span></span>|<span data-ttu-id="543cb-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="543cb-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="543cb-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="543cb-163">privacyInformationUrl</span></span>|<span data-ttu-id="543cb-164">String</span><span class="sxs-lookup"><span data-stu-id="543cb-164">String</span></span>|<span data-ttu-id="543cb-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="543cb-165">The privacy statement Url.</span></span> <span data-ttu-id="543cb-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="543cb-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="543cb-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="543cb-167">informationUrl</span></span>|<span data-ttu-id="543cb-168">String</span><span class="sxs-lookup"><span data-stu-id="543cb-168">String</span></span>|<span data-ttu-id="543cb-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="543cb-169">The more information Url.</span></span> <span data-ttu-id="543cb-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="543cb-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="543cb-171">所有者</span><span class="sxs-lookup"><span data-stu-id="543cb-171">owner</span></span>|<span data-ttu-id="543cb-172">String</span><span class="sxs-lookup"><span data-stu-id="543cb-172">String</span></span>|<span data-ttu-id="543cb-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="543cb-173">The owner of the app.</span></span> <span data-ttu-id="543cb-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="543cb-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="543cb-175">developer</span><span class="sxs-lookup"><span data-stu-id="543cb-175">developer</span></span>|<span data-ttu-id="543cb-176">String</span><span class="sxs-lookup"><span data-stu-id="543cb-176">String</span></span>|<span data-ttu-id="543cb-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="543cb-177">The developer of the app.</span></span> <span data-ttu-id="543cb-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="543cb-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="543cb-179">notes</span><span class="sxs-lookup"><span data-stu-id="543cb-179">notes</span></span>|<span data-ttu-id="543cb-180">String</span><span class="sxs-lookup"><span data-stu-id="543cb-180">String</span></span>|<span data-ttu-id="543cb-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="543cb-181">Notes for the app.</span></span> <span data-ttu-id="543cb-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="543cb-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="543cb-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="543cb-183">publishingState</span></span>|[<span data-ttu-id="543cb-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="543cb-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="543cb-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="543cb-185">The publishing state for the app.</span></span> <span data-ttu-id="543cb-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="543cb-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="543cb-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="543cb-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="543cb-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="543cb-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="543cb-189">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="543cb-189">usedLicenseCount</span></span>|<span data-ttu-id="543cb-190">Int32</span><span class="sxs-lookup"><span data-stu-id="543cb-190">Int32</span></span>|<span data-ttu-id="543cb-191">使用中的适用于企业的 Microsoft Store 许可证数。</span><span class="sxs-lookup"><span data-stu-id="543cb-191">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="543cb-192">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="543cb-192">totalLicenseCount</span></span>|<span data-ttu-id="543cb-193">Int32</span><span class="sxs-lookup"><span data-stu-id="543cb-193">Int32</span></span>|<span data-ttu-id="543cb-194">适用于企业的 Microsoft Store 许可证总数。</span><span class="sxs-lookup"><span data-stu-id="543cb-194">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="543cb-195">productKey</span><span class="sxs-lookup"><span data-stu-id="543cb-195">productKey</span></span>|<span data-ttu-id="543cb-196">String</span><span class="sxs-lookup"><span data-stu-id="543cb-196">String</span></span>|<span data-ttu-id="543cb-197">应用产品密钥</span><span class="sxs-lookup"><span data-stu-id="543cb-197">The app product key</span></span>|
|<span data-ttu-id="543cb-198">licenseType</span><span class="sxs-lookup"><span data-stu-id="543cb-198">licenseType</span></span>|[<span data-ttu-id="543cb-199">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="543cb-199">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="543cb-200">应用程序许可证类型。</span><span class="sxs-lookup"><span data-stu-id="543cb-200">The app license type.</span></span> <span data-ttu-id="543cb-201">可取值为：`offline`、`online`。</span><span class="sxs-lookup"><span data-stu-id="543cb-201">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="543cb-202">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="543cb-202">packageIdentityName</span></span>|<span data-ttu-id="543cb-203">String</span><span class="sxs-lookup"><span data-stu-id="543cb-203">String</span></span>|<span data-ttu-id="543cb-204">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="543cb-204">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="543cb-205">响应</span><span class="sxs-lookup"><span data-stu-id="543cb-205">Response</span></span>
<span data-ttu-id="543cb-206">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="543cb-206">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="543cb-207">示例</span><span class="sxs-lookup"><span data-stu-id="543cb-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="543cb-208">请求</span><span class="sxs-lookup"><span data-stu-id="543cb-208">Request</span></span>
<span data-ttu-id="543cb-209">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="543cb-209">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="543cb-210">响应</span><span class="sxs-lookup"><span data-stu-id="543cb-210">Response</span></span>
<span data-ttu-id="543cb-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="543cb-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




