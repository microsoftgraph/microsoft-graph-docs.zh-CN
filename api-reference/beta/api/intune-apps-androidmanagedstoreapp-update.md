---
title: 更新 androidManagedStoreApp
description: 更新 androidManagedStoreApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 45f37c037b1a9e1d66ff9ce7ace58a51453b6eb4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879392"
---
# <a name="update-androidmanagedstoreapp"></a><span data-ttu-id="19a04-103">更新 androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="19a04-103">Update androidManagedStoreApp</span></span>

> <span data-ttu-id="19a04-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="19a04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19a04-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="19a04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19a04-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="19a04-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19a04-107">更新[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="19a04-107">Update the properties of a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="19a04-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="19a04-108">Prerequisites</span></span>
<span data-ttu-id="19a04-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="19a04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19a04-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="19a04-111">Permission type</span></span>|<span data-ttu-id="19a04-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="19a04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19a04-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19a04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19a04-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19a04-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="19a04-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19a04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19a04-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="19a04-116">Not supported.</span></span>|
|<span data-ttu-id="19a04-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="19a04-117">Application</span></span>|<span data-ttu-id="19a04-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="19a04-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19a04-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19a04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="19a04-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="19a04-120">Request headers</span></span>
|<span data-ttu-id="19a04-121">标头</span><span class="sxs-lookup"><span data-stu-id="19a04-121">Header</span></span>|<span data-ttu-id="19a04-122">值</span><span class="sxs-lookup"><span data-stu-id="19a04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19a04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19a04-123">Authorization</span></span>|<span data-ttu-id="19a04-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="19a04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19a04-125">Accept</span><span class="sxs-lookup"><span data-stu-id="19a04-125">Accept</span></span>|<span data-ttu-id="19a04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19a04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19a04-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="19a04-127">Request body</span></span>
<span data-ttu-id="19a04-128">在请求正文中，提供[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19a04-128">In the request body, supply a JSON representation for the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

<span data-ttu-id="19a04-129">下表显示时创建[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="19a04-129">The following table shows the properties that are required when you create the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span></span>

|<span data-ttu-id="19a04-130">属性</span><span class="sxs-lookup"><span data-stu-id="19a04-130">Property</span></span>|<span data-ttu-id="19a04-131">类型</span><span class="sxs-lookup"><span data-stu-id="19a04-131">Type</span></span>|<span data-ttu-id="19a04-132">说明</span><span class="sxs-lookup"><span data-stu-id="19a04-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19a04-133">id</span><span class="sxs-lookup"><span data-stu-id="19a04-133">id</span></span>|<span data-ttu-id="19a04-134">String</span><span class="sxs-lookup"><span data-stu-id="19a04-134">String</span></span>|<span data-ttu-id="19a04-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="19a04-135">Key of the entity.</span></span> <span data-ttu-id="19a04-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19a04-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19a04-137">displayName</span><span class="sxs-lookup"><span data-stu-id="19a04-137">displayName</span></span>|<span data-ttu-id="19a04-138">String</span><span class="sxs-lookup"><span data-stu-id="19a04-138">String</span></span>|<span data-ttu-id="19a04-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="19a04-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="19a04-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19a04-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19a04-141">description</span><span class="sxs-lookup"><span data-stu-id="19a04-141">description</span></span>|<span data-ttu-id="19a04-142">String</span><span class="sxs-lookup"><span data-stu-id="19a04-142">String</span></span>|<span data-ttu-id="19a04-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="19a04-143">The description of the app.</span></span> <span data-ttu-id="19a04-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19a04-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19a04-145">publisher</span><span class="sxs-lookup"><span data-stu-id="19a04-145">publisher</span></span>|<span data-ttu-id="19a04-146">String</span><span class="sxs-lookup"><span data-stu-id="19a04-146">String</span></span>|<span data-ttu-id="19a04-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="19a04-147">The publisher of the app.</span></span> <span data-ttu-id="19a04-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19a04-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19a04-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="19a04-149">largeIcon</span></span>|[<span data-ttu-id="19a04-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="19a04-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="19a04-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="19a04-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="19a04-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19a04-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19a04-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19a04-153">createdDateTime</span></span>|<span data-ttu-id="19a04-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19a04-154">DateTimeOffset</span></span>|<span data-ttu-id="19a04-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="19a04-155">The date and time the app was created.</span></span> <span data-ttu-id="19a04-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19a04-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19a04-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19a04-157">lastModifiedDateTime</span></span>|<span data-ttu-id="19a04-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19a04-158">DateTimeOffset</span></span>|<span data-ttu-id="19a04-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="19a04-159">The date and time the app was last modified.</span></span> <span data-ttu-id="19a04-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19a04-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19a04-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="19a04-161">isFeatured</span></span>|<span data-ttu-id="19a04-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="19a04-162">Boolean</span></span>|<span data-ttu-id="19a04-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19a04-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19a04-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="19a04-164">privacyInformationUrl</span></span>|<span data-ttu-id="19a04-165">String</span><span class="sxs-lookup"><span data-stu-id="19a04-165">String</span></span>|<span data-ttu-id="19a04-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="19a04-166">The privacy statement Url.</span></span> <span data-ttu-id="19a04-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19a04-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19a04-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="19a04-168">informationUrl</span></span>|<span data-ttu-id="19a04-169">String</span><span class="sxs-lookup"><span data-stu-id="19a04-169">String</span></span>|<span data-ttu-id="19a04-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="19a04-170">The more information Url.</span></span> <span data-ttu-id="19a04-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19a04-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19a04-172">owner</span><span class="sxs-lookup"><span data-stu-id="19a04-172">owner</span></span>|<span data-ttu-id="19a04-173">String</span><span class="sxs-lookup"><span data-stu-id="19a04-173">String</span></span>|<span data-ttu-id="19a04-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="19a04-174">The owner of the app.</span></span> <span data-ttu-id="19a04-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19a04-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19a04-176">developer</span><span class="sxs-lookup"><span data-stu-id="19a04-176">developer</span></span>|<span data-ttu-id="19a04-177">String</span><span class="sxs-lookup"><span data-stu-id="19a04-177">String</span></span>|<span data-ttu-id="19a04-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="19a04-178">The developer of the app.</span></span> <span data-ttu-id="19a04-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19a04-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19a04-180">notes</span><span class="sxs-lookup"><span data-stu-id="19a04-180">notes</span></span>|<span data-ttu-id="19a04-181">String</span><span class="sxs-lookup"><span data-stu-id="19a04-181">String</span></span>|<span data-ttu-id="19a04-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="19a04-182">Notes for the app.</span></span> <span data-ttu-id="19a04-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19a04-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19a04-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="19a04-184">uploadState</span></span>|<span data-ttu-id="19a04-185">Int32</span><span class="sxs-lookup"><span data-stu-id="19a04-185">Int32</span></span>|<span data-ttu-id="19a04-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="19a04-186">The upload state.</span></span> <span data-ttu-id="19a04-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19a04-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19a04-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="19a04-188">publishingState</span></span>|[<span data-ttu-id="19a04-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="19a04-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="19a04-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="19a04-190">The publishing state for the app.</span></span> <span data-ttu-id="19a04-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="19a04-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="19a04-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="19a04-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="19a04-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="19a04-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="19a04-194">packageId</span><span class="sxs-lookup"><span data-stu-id="19a04-194">packageId</span></span>|<span data-ttu-id="19a04-195">String</span><span class="sxs-lookup"><span data-stu-id="19a04-195">String</span></span>|<span data-ttu-id="19a04-196">包标识符。</span><span class="sxs-lookup"><span data-stu-id="19a04-196">The package identifier.</span></span>|
|<span data-ttu-id="19a04-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="19a04-197">appIdentifier</span></span>|<span data-ttu-id="19a04-198">String</span><span class="sxs-lookup"><span data-stu-id="19a04-198">String</span></span>|<span data-ttu-id="19a04-199">标识名称。</span><span class="sxs-lookup"><span data-stu-id="19a04-199">The Identity Name.</span></span>|
|<span data-ttu-id="19a04-200">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="19a04-200">usedLicenseCount</span></span>|<span data-ttu-id="19a04-201">Int32</span><span class="sxs-lookup"><span data-stu-id="19a04-201">Int32</span></span>|<span data-ttu-id="19a04-202">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="19a04-202">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="19a04-203">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="19a04-203">totalLicenseCount</span></span>|<span data-ttu-id="19a04-204">Int32</span><span class="sxs-lookup"><span data-stu-id="19a04-204">Int32</span></span>|<span data-ttu-id="19a04-205">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="19a04-205">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="19a04-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="19a04-206">appStoreUrl</span></span>|<span data-ttu-id="19a04-207">String</span><span class="sxs-lookup"><span data-stu-id="19a04-207">String</span></span>|<span data-ttu-id="19a04-208">工作存储应用程序 url 播放。</span><span class="sxs-lookup"><span data-stu-id="19a04-208">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="19a04-209">响应</span><span class="sxs-lookup"><span data-stu-id="19a04-209">Response</span></span>
<span data-ttu-id="19a04-210">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="19a04-210">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19a04-211">示例</span><span class="sxs-lookup"><span data-stu-id="19a04-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="19a04-212">请求</span><span class="sxs-lookup"><span data-stu-id="19a04-212">Request</span></span>
<span data-ttu-id="19a04-213">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="19a04-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 799

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="19a04-214">响应</span><span class="sxs-lookup"><span data-stu-id="19a04-214">Response</span></span>
<span data-ttu-id="19a04-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19a04-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 968

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
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
  "uploadState": 11,
  "publishingState": "processing",
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```





