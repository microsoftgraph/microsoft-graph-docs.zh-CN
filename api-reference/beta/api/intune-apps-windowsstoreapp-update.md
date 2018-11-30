---
title: 更新 windowsStoreApp
description: 更新 windowsStoreApp 对象的属性。
ms.openlocfilehash: 580c1e3570b5315d3ded9c126cf3bbdf17d7450c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046762"
---
# <a name="update-windowsstoreapp"></a><span data-ttu-id="df6af-103">更新 windowsStoreApp</span><span class="sxs-lookup"><span data-stu-id="df6af-103">Update windowsStoreApp</span></span>

> <span data-ttu-id="df6af-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="df6af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df6af-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="df6af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df6af-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="df6af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df6af-107">更新[windowsStoreApp](../resources/intune-apps-windowsstoreapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="df6af-107">Update the properties of a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="df6af-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="df6af-108">Prerequisites</span></span>
<span data-ttu-id="df6af-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="df6af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df6af-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="df6af-111">Permission type</span></span>|<span data-ttu-id="df6af-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="df6af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df6af-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df6af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df6af-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df6af-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="df6af-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df6af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df6af-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="df6af-116">Not supported.</span></span>|
|<span data-ttu-id="df6af-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="df6af-117">Application</span></span>|<span data-ttu-id="df6af-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="df6af-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df6af-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df6af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="df6af-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="df6af-120">Request headers</span></span>
|<span data-ttu-id="df6af-121">标头</span><span class="sxs-lookup"><span data-stu-id="df6af-121">Header</span></span>|<span data-ttu-id="df6af-122">值</span><span class="sxs-lookup"><span data-stu-id="df6af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df6af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df6af-123">Authorization</span></span>|<span data-ttu-id="df6af-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="df6af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df6af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="df6af-125">Accept</span></span>|<span data-ttu-id="df6af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df6af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df6af-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="df6af-127">Request body</span></span>
<span data-ttu-id="df6af-128">在请求正文中，提供[windowsStoreApp](../resources/intune-apps-windowsstoreapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df6af-128">In the request body, supply a JSON representation for the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

<span data-ttu-id="df6af-129">下表显示时创建[windowsStoreApp](../resources/intune-apps-windowsstoreapp.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="df6af-129">The following table shows the properties that are required when you create the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md).</span></span>

|<span data-ttu-id="df6af-130">属性</span><span class="sxs-lookup"><span data-stu-id="df6af-130">Property</span></span>|<span data-ttu-id="df6af-131">类型</span><span class="sxs-lookup"><span data-stu-id="df6af-131">Type</span></span>|<span data-ttu-id="df6af-132">说明</span><span class="sxs-lookup"><span data-stu-id="df6af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df6af-133">id</span><span class="sxs-lookup"><span data-stu-id="df6af-133">id</span></span>|<span data-ttu-id="df6af-134">String</span><span class="sxs-lookup"><span data-stu-id="df6af-134">String</span></span>|<span data-ttu-id="df6af-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="df6af-135">Key of the entity.</span></span> <span data-ttu-id="df6af-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df6af-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df6af-137">displayName</span><span class="sxs-lookup"><span data-stu-id="df6af-137">displayName</span></span>|<span data-ttu-id="df6af-138">String</span><span class="sxs-lookup"><span data-stu-id="df6af-138">String</span></span>|<span data-ttu-id="df6af-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="df6af-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="df6af-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df6af-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df6af-141">description</span><span class="sxs-lookup"><span data-stu-id="df6af-141">description</span></span>|<span data-ttu-id="df6af-142">String</span><span class="sxs-lookup"><span data-stu-id="df6af-142">String</span></span>|<span data-ttu-id="df6af-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="df6af-143">The description of the app.</span></span> <span data-ttu-id="df6af-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df6af-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df6af-145">publisher</span><span class="sxs-lookup"><span data-stu-id="df6af-145">publisher</span></span>|<span data-ttu-id="df6af-146">String</span><span class="sxs-lookup"><span data-stu-id="df6af-146">String</span></span>|<span data-ttu-id="df6af-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="df6af-147">The publisher of the app.</span></span> <span data-ttu-id="df6af-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df6af-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df6af-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="df6af-149">largeIcon</span></span>|[<span data-ttu-id="df6af-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="df6af-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="df6af-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="df6af-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="df6af-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df6af-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df6af-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df6af-153">createdDateTime</span></span>|<span data-ttu-id="df6af-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df6af-154">DateTimeOffset</span></span>|<span data-ttu-id="df6af-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="df6af-155">The date and time the app was created.</span></span> <span data-ttu-id="df6af-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df6af-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df6af-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df6af-157">lastModifiedDateTime</span></span>|<span data-ttu-id="df6af-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df6af-158">DateTimeOffset</span></span>|<span data-ttu-id="df6af-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="df6af-159">The date and time the app was last modified.</span></span> <span data-ttu-id="df6af-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df6af-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df6af-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="df6af-161">isFeatured</span></span>|<span data-ttu-id="df6af-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="df6af-162">Boolean</span></span>|<span data-ttu-id="df6af-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df6af-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df6af-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="df6af-164">privacyInformationUrl</span></span>|<span data-ttu-id="df6af-165">String</span><span class="sxs-lookup"><span data-stu-id="df6af-165">String</span></span>|<span data-ttu-id="df6af-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="df6af-166">The privacy statement Url.</span></span> <span data-ttu-id="df6af-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df6af-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df6af-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="df6af-168">informationUrl</span></span>|<span data-ttu-id="df6af-169">String</span><span class="sxs-lookup"><span data-stu-id="df6af-169">String</span></span>|<span data-ttu-id="df6af-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="df6af-170">The more information Url.</span></span> <span data-ttu-id="df6af-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df6af-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df6af-172">owner</span><span class="sxs-lookup"><span data-stu-id="df6af-172">owner</span></span>|<span data-ttu-id="df6af-173">String</span><span class="sxs-lookup"><span data-stu-id="df6af-173">String</span></span>|<span data-ttu-id="df6af-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="df6af-174">The owner of the app.</span></span> <span data-ttu-id="df6af-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df6af-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df6af-176">developer</span><span class="sxs-lookup"><span data-stu-id="df6af-176">developer</span></span>|<span data-ttu-id="df6af-177">String</span><span class="sxs-lookup"><span data-stu-id="df6af-177">String</span></span>|<span data-ttu-id="df6af-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="df6af-178">The developer of the app.</span></span> <span data-ttu-id="df6af-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df6af-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df6af-180">notes</span><span class="sxs-lookup"><span data-stu-id="df6af-180">notes</span></span>|<span data-ttu-id="df6af-181">String</span><span class="sxs-lookup"><span data-stu-id="df6af-181">String</span></span>|<span data-ttu-id="df6af-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="df6af-182">Notes for the app.</span></span> <span data-ttu-id="df6af-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df6af-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df6af-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="df6af-184">uploadState</span></span>|<span data-ttu-id="df6af-185">Int32</span><span class="sxs-lookup"><span data-stu-id="df6af-185">Int32</span></span>|<span data-ttu-id="df6af-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="df6af-186">The upload state.</span></span> <span data-ttu-id="df6af-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df6af-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df6af-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="df6af-188">publishingState</span></span>|[<span data-ttu-id="df6af-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="df6af-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="df6af-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="df6af-190">The publishing state for the app.</span></span> <span data-ttu-id="df6af-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="df6af-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="df6af-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="df6af-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="df6af-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="df6af-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="df6af-194">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="df6af-194">appStoreUrl</span></span>|<span data-ttu-id="df6af-195">String</span><span class="sxs-lookup"><span data-stu-id="df6af-195">String</span></span>|<span data-ttu-id="df6af-196">Windows 应用程序存储 URL。</span><span class="sxs-lookup"><span data-stu-id="df6af-196">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="df6af-197">响应</span><span class="sxs-lookup"><span data-stu-id="df6af-197">Response</span></span>
<span data-ttu-id="df6af-198">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsStoreApp](../resources/intune-apps-windowsstoreapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="df6af-198">If successful, this method returns a `200 OK` response code and an updated [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df6af-199">示例</span><span class="sxs-lookup"><span data-stu-id="df6af-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="df6af-200">请求</span><span class="sxs-lookup"><span data-stu-id="df6af-200">Request</span></span>
<span data-ttu-id="df6af-201">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df6af-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="df6af-202">响应</span><span class="sxs-lookup"><span data-stu-id="df6af-202">Response</span></span>
<span data-ttu-id="df6af-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df6af-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 828

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
  "id": "fd4a5f8a-5f8a-fd4a-8a5f-4afd8a5f4afd",
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





