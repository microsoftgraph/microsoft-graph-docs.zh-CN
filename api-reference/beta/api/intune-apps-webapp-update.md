---
title: 更新 webApp
description: 更新 webApp 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c1fb65ad13c1019ad33f87b125b4797ebc4730f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39934089"
---
# <a name="update-webapp"></a><span data-ttu-id="28581-103">更新 webApp</span><span class="sxs-lookup"><span data-stu-id="28581-103">Update webApp</span></span>

> <span data-ttu-id="28581-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="28581-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28581-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="28581-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28581-106">更新 [webApp](../resources/intune-apps-webapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="28581-106">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28581-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="28581-107">Prerequisites</span></span>
<span data-ttu-id="28581-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="28581-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28581-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="28581-110">Permission type</span></span>|<span data-ttu-id="28581-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="28581-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28581-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28581-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28581-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28581-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="28581-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28581-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28581-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="28581-115">Not supported.</span></span>|
|<span data-ttu-id="28581-116">Application</span><span class="sxs-lookup"><span data-stu-id="28581-116">Application</span></span>|<span data-ttu-id="28581-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28581-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28581-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28581-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="28581-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="28581-119">Request headers</span></span>
|<span data-ttu-id="28581-120">标头</span><span class="sxs-lookup"><span data-stu-id="28581-120">Header</span></span>|<span data-ttu-id="28581-121">值</span><span class="sxs-lookup"><span data-stu-id="28581-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28581-122">授权</span><span class="sxs-lookup"><span data-stu-id="28581-122">Authorization</span></span>|<span data-ttu-id="28581-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="28581-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28581-124">接受</span><span class="sxs-lookup"><span data-stu-id="28581-124">Accept</span></span>|<span data-ttu-id="28581-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28581-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28581-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="28581-126">Request body</span></span>
<span data-ttu-id="28581-127">在请求正文中，提供 [webApp](../resources/intune-apps-webapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28581-127">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="28581-128">下表显示创建 [webApp](../resources/intune-apps-webapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="28581-128">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="28581-129">属性</span><span class="sxs-lookup"><span data-stu-id="28581-129">Property</span></span>|<span data-ttu-id="28581-130">类型</span><span class="sxs-lookup"><span data-stu-id="28581-130">Type</span></span>|<span data-ttu-id="28581-131">说明</span><span class="sxs-lookup"><span data-stu-id="28581-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28581-132">id</span><span class="sxs-lookup"><span data-stu-id="28581-132">id</span></span>|<span data-ttu-id="28581-133">字符串</span><span class="sxs-lookup"><span data-stu-id="28581-133">String</span></span>|<span data-ttu-id="28581-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="28581-134">Key of the entity.</span></span> <span data-ttu-id="28581-135">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="28581-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="28581-136">displayName</span><span class="sxs-lookup"><span data-stu-id="28581-136">displayName</span></span>|<span data-ttu-id="28581-137">字符串</span><span class="sxs-lookup"><span data-stu-id="28581-137">String</span></span>|<span data-ttu-id="28581-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="28581-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="28581-139">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="28581-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="28581-140">说明</span><span class="sxs-lookup"><span data-stu-id="28581-140">description</span></span>|<span data-ttu-id="28581-141">字符串</span><span class="sxs-lookup"><span data-stu-id="28581-141">String</span></span>|<span data-ttu-id="28581-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="28581-142">The description of the app.</span></span> <span data-ttu-id="28581-143">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="28581-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="28581-144">publisher</span><span class="sxs-lookup"><span data-stu-id="28581-144">publisher</span></span>|<span data-ttu-id="28581-145">字符串</span><span class="sxs-lookup"><span data-stu-id="28581-145">String</span></span>|<span data-ttu-id="28581-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="28581-146">The publisher of the app.</span></span> <span data-ttu-id="28581-147">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="28581-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="28581-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="28581-148">largeIcon</span></span>|[<span data-ttu-id="28581-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="28581-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="28581-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="28581-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="28581-151">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="28581-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="28581-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="28581-152">createdDateTime</span></span>|<span data-ttu-id="28581-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28581-153">DateTimeOffset</span></span>|<span data-ttu-id="28581-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="28581-154">The date and time the app was created.</span></span> <span data-ttu-id="28581-155">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="28581-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="28581-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28581-156">lastModifiedDateTime</span></span>|<span data-ttu-id="28581-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28581-157">DateTimeOffset</span></span>|<span data-ttu-id="28581-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="28581-158">The date and time the app was last modified.</span></span> <span data-ttu-id="28581-159">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="28581-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="28581-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="28581-160">isFeatured</span></span>|<span data-ttu-id="28581-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="28581-161">Boolean</span></span>|<span data-ttu-id="28581-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="28581-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="28581-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="28581-163">privacyInformationUrl</span></span>|<span data-ttu-id="28581-164">字符串</span><span class="sxs-lookup"><span data-stu-id="28581-164">String</span></span>|<span data-ttu-id="28581-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="28581-165">The privacy statement Url.</span></span> <span data-ttu-id="28581-166">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="28581-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="28581-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="28581-167">informationUrl</span></span>|<span data-ttu-id="28581-168">字符串</span><span class="sxs-lookup"><span data-stu-id="28581-168">String</span></span>|<span data-ttu-id="28581-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="28581-169">The more information Url.</span></span> <span data-ttu-id="28581-170">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="28581-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="28581-171">owner</span><span class="sxs-lookup"><span data-stu-id="28581-171">owner</span></span>|<span data-ttu-id="28581-172">String</span><span class="sxs-lookup"><span data-stu-id="28581-172">String</span></span>|<span data-ttu-id="28581-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="28581-173">The owner of the app.</span></span> <span data-ttu-id="28581-174">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="28581-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="28581-175">developer</span><span class="sxs-lookup"><span data-stu-id="28581-175">developer</span></span>|<span data-ttu-id="28581-176">字符串</span><span class="sxs-lookup"><span data-stu-id="28581-176">String</span></span>|<span data-ttu-id="28581-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="28581-177">The developer of the app.</span></span> <span data-ttu-id="28581-178">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="28581-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="28581-179">notes</span><span class="sxs-lookup"><span data-stu-id="28581-179">notes</span></span>|<span data-ttu-id="28581-180">字符串</span><span class="sxs-lookup"><span data-stu-id="28581-180">String</span></span>|<span data-ttu-id="28581-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="28581-181">Notes for the app.</span></span> <span data-ttu-id="28581-182">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="28581-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="28581-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="28581-183">uploadState</span></span>|<span data-ttu-id="28581-184">Int32</span><span class="sxs-lookup"><span data-stu-id="28581-184">Int32</span></span>|<span data-ttu-id="28581-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="28581-185">The upload state.</span></span> <span data-ttu-id="28581-186">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="28581-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="28581-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="28581-187">publishingState</span></span>|[<span data-ttu-id="28581-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="28581-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="28581-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="28581-189">The publishing state for the app.</span></span> <span data-ttu-id="28581-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="28581-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="28581-191">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="28581-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="28581-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="28581-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="28581-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="28581-193">isAssigned</span></span>|<span data-ttu-id="28581-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="28581-194">Boolean</span></span>|<span data-ttu-id="28581-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="28581-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="28581-196">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="28581-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="28581-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="28581-197">roleScopeTagIds</span></span>|<span data-ttu-id="28581-198">String collection</span><span class="sxs-lookup"><span data-stu-id="28581-198">String collection</span></span>|<span data-ttu-id="28581-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="28581-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="28581-200">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="28581-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="28581-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="28581-201">dependentAppCount</span></span>|<span data-ttu-id="28581-202">Int32</span><span class="sxs-lookup"><span data-stu-id="28581-202">Int32</span></span>|<span data-ttu-id="28581-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="28581-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="28581-204">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="28581-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="28581-205">appUrl</span><span class="sxs-lookup"><span data-stu-id="28581-205">appUrl</span></span>|<span data-ttu-id="28581-206">String</span><span class="sxs-lookup"><span data-stu-id="28581-206">String</span></span>|<span data-ttu-id="28581-207">Web 应用 URL。</span><span class="sxs-lookup"><span data-stu-id="28581-207">The web app URL.</span></span>|
|<span data-ttu-id="28581-208">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="28581-208">useManagedBrowser</span></span>|<span data-ttu-id="28581-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="28581-209">Boolean</span></span>|<span data-ttu-id="28581-210">是否使用托管浏览器。</span><span class="sxs-lookup"><span data-stu-id="28581-210">Whether or not to use managed browser.</span></span> <span data-ttu-id="28581-211">此属性仅适用于 Android 和 iOS。</span><span class="sxs-lookup"><span data-stu-id="28581-211">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="28581-212">响应</span><span class="sxs-lookup"><span data-stu-id="28581-212">Response</span></span>
<span data-ttu-id="28581-213">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [webApp](../resources/intune-apps-webapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="28581-213">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28581-214">示例</span><span class="sxs-lookup"><span data-stu-id="28581-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="28581-215">请求</span><span class="sxs-lookup"><span data-stu-id="28581-215">Request</span></span>
<span data-ttu-id="28581-216">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="28581-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 779

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="28581-217">响应</span><span class="sxs-lookup"><span data-stu-id="28581-217">Response</span></span>
<span data-ttu-id="28581-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="28581-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 951

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```





