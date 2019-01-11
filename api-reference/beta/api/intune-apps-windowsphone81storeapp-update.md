---
title: 更新 windowsPhone81StoreApp
description: 更新 windowsPhone81StoreApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d1ba9c814d29d57c0bcb8024dc70b537c4a92b57
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875416"
---
# <a name="update-windowsphone81storeapp"></a><span data-ttu-id="55b67-103">更新 windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="55b67-103">Update windowsPhone81StoreApp</span></span>

> <span data-ttu-id="55b67-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="55b67-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55b67-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="55b67-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55b67-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="55b67-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55b67-107">更新[windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="55b67-107">Update the properties of a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="55b67-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="55b67-108">Prerequisites</span></span>
<span data-ttu-id="55b67-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="55b67-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55b67-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="55b67-111">Permission type</span></span>|<span data-ttu-id="55b67-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="55b67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55b67-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55b67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55b67-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55b67-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="55b67-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55b67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55b67-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="55b67-116">Not supported.</span></span>|
|<span data-ttu-id="55b67-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="55b67-117">Application</span></span>|<span data-ttu-id="55b67-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="55b67-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55b67-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55b67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="55b67-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="55b67-120">Request headers</span></span>
|<span data-ttu-id="55b67-121">标头</span><span class="sxs-lookup"><span data-stu-id="55b67-121">Header</span></span>|<span data-ttu-id="55b67-122">值</span><span class="sxs-lookup"><span data-stu-id="55b67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55b67-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="55b67-123">Authorization</span></span>|<span data-ttu-id="55b67-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="55b67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55b67-125">Accept</span><span class="sxs-lookup"><span data-stu-id="55b67-125">Accept</span></span>|<span data-ttu-id="55b67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55b67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55b67-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="55b67-127">Request body</span></span>
<span data-ttu-id="55b67-128">在请求正文中，提供[windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55b67-128">In the request body, supply a JSON representation for the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

<span data-ttu-id="55b67-129">下表显示时创建[windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="55b67-129">The following table shows the properties that are required when you create the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md).</span></span>

|<span data-ttu-id="55b67-130">属性</span><span class="sxs-lookup"><span data-stu-id="55b67-130">Property</span></span>|<span data-ttu-id="55b67-131">类型</span><span class="sxs-lookup"><span data-stu-id="55b67-131">Type</span></span>|<span data-ttu-id="55b67-132">说明</span><span class="sxs-lookup"><span data-stu-id="55b67-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55b67-133">id</span><span class="sxs-lookup"><span data-stu-id="55b67-133">id</span></span>|<span data-ttu-id="55b67-134">String</span><span class="sxs-lookup"><span data-stu-id="55b67-134">String</span></span>|<span data-ttu-id="55b67-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="55b67-135">Key of the entity.</span></span> <span data-ttu-id="55b67-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55b67-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55b67-137">displayName</span><span class="sxs-lookup"><span data-stu-id="55b67-137">displayName</span></span>|<span data-ttu-id="55b67-138">String</span><span class="sxs-lookup"><span data-stu-id="55b67-138">String</span></span>|<span data-ttu-id="55b67-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="55b67-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="55b67-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55b67-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55b67-141">description</span><span class="sxs-lookup"><span data-stu-id="55b67-141">description</span></span>|<span data-ttu-id="55b67-142">String</span><span class="sxs-lookup"><span data-stu-id="55b67-142">String</span></span>|<span data-ttu-id="55b67-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="55b67-143">The description of the app.</span></span> <span data-ttu-id="55b67-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55b67-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55b67-145">publisher</span><span class="sxs-lookup"><span data-stu-id="55b67-145">publisher</span></span>|<span data-ttu-id="55b67-146">String</span><span class="sxs-lookup"><span data-stu-id="55b67-146">String</span></span>|<span data-ttu-id="55b67-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="55b67-147">The publisher of the app.</span></span> <span data-ttu-id="55b67-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55b67-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55b67-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="55b67-149">largeIcon</span></span>|[<span data-ttu-id="55b67-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="55b67-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="55b67-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="55b67-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="55b67-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55b67-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55b67-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55b67-153">createdDateTime</span></span>|<span data-ttu-id="55b67-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55b67-154">DateTimeOffset</span></span>|<span data-ttu-id="55b67-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="55b67-155">The date and time the app was created.</span></span> <span data-ttu-id="55b67-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55b67-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55b67-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55b67-157">lastModifiedDateTime</span></span>|<span data-ttu-id="55b67-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55b67-158">DateTimeOffset</span></span>|<span data-ttu-id="55b67-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="55b67-159">The date and time the app was last modified.</span></span> <span data-ttu-id="55b67-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55b67-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55b67-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="55b67-161">isFeatured</span></span>|<span data-ttu-id="55b67-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="55b67-162">Boolean</span></span>|<span data-ttu-id="55b67-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55b67-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55b67-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="55b67-164">privacyInformationUrl</span></span>|<span data-ttu-id="55b67-165">String</span><span class="sxs-lookup"><span data-stu-id="55b67-165">String</span></span>|<span data-ttu-id="55b67-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="55b67-166">The privacy statement Url.</span></span> <span data-ttu-id="55b67-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55b67-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55b67-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="55b67-168">informationUrl</span></span>|<span data-ttu-id="55b67-169">String</span><span class="sxs-lookup"><span data-stu-id="55b67-169">String</span></span>|<span data-ttu-id="55b67-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="55b67-170">The more information Url.</span></span> <span data-ttu-id="55b67-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55b67-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55b67-172">owner</span><span class="sxs-lookup"><span data-stu-id="55b67-172">owner</span></span>|<span data-ttu-id="55b67-173">String</span><span class="sxs-lookup"><span data-stu-id="55b67-173">String</span></span>|<span data-ttu-id="55b67-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="55b67-174">The owner of the app.</span></span> <span data-ttu-id="55b67-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55b67-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55b67-176">developer</span><span class="sxs-lookup"><span data-stu-id="55b67-176">developer</span></span>|<span data-ttu-id="55b67-177">String</span><span class="sxs-lookup"><span data-stu-id="55b67-177">String</span></span>|<span data-ttu-id="55b67-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="55b67-178">The developer of the app.</span></span> <span data-ttu-id="55b67-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55b67-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55b67-180">notes</span><span class="sxs-lookup"><span data-stu-id="55b67-180">notes</span></span>|<span data-ttu-id="55b67-181">String</span><span class="sxs-lookup"><span data-stu-id="55b67-181">String</span></span>|<span data-ttu-id="55b67-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="55b67-182">Notes for the app.</span></span> <span data-ttu-id="55b67-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55b67-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55b67-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="55b67-184">uploadState</span></span>|<span data-ttu-id="55b67-185">Int32</span><span class="sxs-lookup"><span data-stu-id="55b67-185">Int32</span></span>|<span data-ttu-id="55b67-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="55b67-186">The upload state.</span></span> <span data-ttu-id="55b67-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55b67-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55b67-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="55b67-188">publishingState</span></span>|[<span data-ttu-id="55b67-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="55b67-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="55b67-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="55b67-190">The publishing state for the app.</span></span> <span data-ttu-id="55b67-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="55b67-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="55b67-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="55b67-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="55b67-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="55b67-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="55b67-194">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="55b67-194">appStoreUrl</span></span>|<span data-ttu-id="55b67-195">String</span><span class="sxs-lookup"><span data-stu-id="55b67-195">String</span></span>|<span data-ttu-id="55b67-196">Windows Phone 8.1 应用程序存储 URL。</span><span class="sxs-lookup"><span data-stu-id="55b67-196">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="55b67-197">响应</span><span class="sxs-lookup"><span data-stu-id="55b67-197">Response</span></span>
<span data-ttu-id="55b67-198">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="55b67-198">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55b67-199">示例</span><span class="sxs-lookup"><span data-stu-id="55b67-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="55b67-200">请求</span><span class="sxs-lookup"><span data-stu-id="55b67-200">Request</span></span>
<span data-ttu-id="55b67-201">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="55b67-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 666

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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="55b67-202">响应</span><span class="sxs-lookup"><span data-stu-id="55b67-202">Response</span></span>
<span data-ttu-id="55b67-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="55b67-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 835

{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
  "id": "f68ce6a1-e6a1-f68c-a1e6-8cf6a1e68cf6",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```





