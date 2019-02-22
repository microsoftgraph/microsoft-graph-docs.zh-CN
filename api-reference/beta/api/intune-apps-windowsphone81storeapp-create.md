---
title: 创建 windowsPhone81StoreApp
description: 创建新的 windowsPhone81StoreApp 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 556ce1344034ee4fbb91a66fa053b17c1cc99214
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173883"
---
# <a name="create-windowsphone81storeapp"></a><span data-ttu-id="ce953-103">创建 windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="ce953-103">Create windowsPhone81StoreApp</span></span>

> <span data-ttu-id="ce953-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ce953-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce953-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce953-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce953-106">创建新的[windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ce953-106">Create a new [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce953-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ce953-107">Prerequisites</span></span>
<span data-ttu-id="ce953-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ce953-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ce953-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce953-110">Permission type</span></span>|<span data-ttu-id="ce953-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ce953-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce953-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce953-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ce953-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce953-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ce953-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce953-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce953-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce953-115">Not supported.</span></span>|
|<span data-ttu-id="ce953-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce953-116">Application</span></span>|<span data-ttu-id="ce953-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce953-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce953-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce953-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ce953-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce953-119">Request headers</span></span>
|<span data-ttu-id="ce953-120">标头</span><span class="sxs-lookup"><span data-stu-id="ce953-120">Header</span></span>|<span data-ttu-id="ce953-121">值</span><span class="sxs-lookup"><span data-stu-id="ce953-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce953-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce953-122">Authorization</span></span>|<span data-ttu-id="ce953-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ce953-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce953-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ce953-124">Accept</span></span>|<span data-ttu-id="ce953-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ce953-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce953-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce953-126">Request body</span></span>
<span data-ttu-id="ce953-127">在请求正文中, 提供 windowsPhone81StoreApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce953-127">In the request body, supply a JSON representation for the windowsPhone81StoreApp object.</span></span>

<span data-ttu-id="ce953-128">下表显示创建 windowsPhone81StoreApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ce953-128">The following table shows the properties that are required when you create the windowsPhone81StoreApp.</span></span>

|<span data-ttu-id="ce953-129">属性</span><span class="sxs-lookup"><span data-stu-id="ce953-129">Property</span></span>|<span data-ttu-id="ce953-130">类型</span><span class="sxs-lookup"><span data-stu-id="ce953-130">Type</span></span>|<span data-ttu-id="ce953-131">说明</span><span class="sxs-lookup"><span data-stu-id="ce953-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce953-132">id</span><span class="sxs-lookup"><span data-stu-id="ce953-132">id</span></span>|<span data-ttu-id="ce953-133">字串符号</span><span class="sxs-lookup"><span data-stu-id="ce953-133">String</span></span>|<span data-ttu-id="ce953-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ce953-134">Key of the entity.</span></span> <span data-ttu-id="ce953-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce953-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce953-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ce953-136">displayName</span></span>|<span data-ttu-id="ce953-137">字符串</span><span class="sxs-lookup"><span data-stu-id="ce953-137">String</span></span>|<span data-ttu-id="ce953-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="ce953-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ce953-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce953-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce953-140">description</span><span class="sxs-lookup"><span data-stu-id="ce953-140">description</span></span>|<span data-ttu-id="ce953-141">字符串</span><span class="sxs-lookup"><span data-stu-id="ce953-141">String</span></span>|<span data-ttu-id="ce953-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="ce953-142">The description of the app.</span></span> <span data-ttu-id="ce953-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce953-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce953-144">publisher</span><span class="sxs-lookup"><span data-stu-id="ce953-144">publisher</span></span>|<span data-ttu-id="ce953-145">字符串</span><span class="sxs-lookup"><span data-stu-id="ce953-145">String</span></span>|<span data-ttu-id="ce953-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="ce953-146">The publisher of the app.</span></span> <span data-ttu-id="ce953-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce953-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce953-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ce953-148">largeIcon</span></span>|[<span data-ttu-id="ce953-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ce953-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ce953-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="ce953-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ce953-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce953-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce953-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce953-152">createdDateTime</span></span>|<span data-ttu-id="ce953-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce953-153">DateTimeOffset</span></span>|<span data-ttu-id="ce953-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ce953-154">The date and time the app was created.</span></span> <span data-ttu-id="ce953-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce953-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce953-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce953-156">lastModifiedDateTime</span></span>|<span data-ttu-id="ce953-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce953-157">DateTimeOffset</span></span>|<span data-ttu-id="ce953-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ce953-158">The date and time the app was last modified.</span></span> <span data-ttu-id="ce953-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce953-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce953-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ce953-160">isFeatured</span></span>|<span data-ttu-id="ce953-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce953-161">Boolean</span></span>|<span data-ttu-id="ce953-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce953-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce953-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ce953-163">privacyInformationUrl</span></span>|<span data-ttu-id="ce953-164">字符串</span><span class="sxs-lookup"><span data-stu-id="ce953-164">String</span></span>|<span data-ttu-id="ce953-165">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="ce953-165">The privacy statement Url.</span></span> <span data-ttu-id="ce953-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce953-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce953-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ce953-167">informationUrl</span></span>|<span data-ttu-id="ce953-168">字符串</span><span class="sxs-lookup"><span data-stu-id="ce953-168">String</span></span>|<span data-ttu-id="ce953-169">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="ce953-169">The more information Url.</span></span> <span data-ttu-id="ce953-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce953-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce953-171">owner</span><span class="sxs-lookup"><span data-stu-id="ce953-171">owner</span></span>|<span data-ttu-id="ce953-172">String</span><span class="sxs-lookup"><span data-stu-id="ce953-172">String</span></span>|<span data-ttu-id="ce953-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="ce953-173">The owner of the app.</span></span> <span data-ttu-id="ce953-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce953-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce953-175">developer</span><span class="sxs-lookup"><span data-stu-id="ce953-175">developer</span></span>|<span data-ttu-id="ce953-176">String</span><span class="sxs-lookup"><span data-stu-id="ce953-176">String</span></span>|<span data-ttu-id="ce953-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="ce953-177">The developer of the app.</span></span> <span data-ttu-id="ce953-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce953-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce953-179">notes</span><span class="sxs-lookup"><span data-stu-id="ce953-179">notes</span></span>|<span data-ttu-id="ce953-180">String</span><span class="sxs-lookup"><span data-stu-id="ce953-180">String</span></span>|<span data-ttu-id="ce953-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="ce953-181">Notes for the app.</span></span> <span data-ttu-id="ce953-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce953-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce953-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="ce953-183">uploadState</span></span>|<span data-ttu-id="ce953-184">Int32</span><span class="sxs-lookup"><span data-stu-id="ce953-184">Int32</span></span>|<span data-ttu-id="ce953-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="ce953-185">The upload state.</span></span> <span data-ttu-id="ce953-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce953-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce953-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="ce953-187">publishingState</span></span>|[<span data-ttu-id="ce953-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ce953-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ce953-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="ce953-189">The publishing state for the app.</span></span> <span data-ttu-id="ce953-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="ce953-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ce953-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="ce953-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ce953-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="ce953-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ce953-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ce953-193">isAssigned</span></span>|<span data-ttu-id="ce953-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce953-194">Boolean</span></span>|<span data-ttu-id="ce953-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="ce953-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ce953-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce953-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce953-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ce953-197">roleScopeTagIds</span></span>|<span data-ttu-id="ce953-198">String collection</span><span class="sxs-lookup"><span data-stu-id="ce953-198">String collection</span></span>|<span data-ttu-id="ce953-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="ce953-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ce953-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce953-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce953-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ce953-201">appStoreUrl</span></span>|<span data-ttu-id="ce953-202">String</span><span class="sxs-lookup"><span data-stu-id="ce953-202">String</span></span>|<span data-ttu-id="ce953-203">Windows Phone 8.1 应用商店 URL。</span><span class="sxs-lookup"><span data-stu-id="ce953-203">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="ce953-204">响应</span><span class="sxs-lookup"><span data-stu-id="ce953-204">Response</span></span>
<span data-ttu-id="ce953-205">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ce953-205">If successful, this method returns a `201 Created` response code and a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce953-206">示例</span><span class="sxs-lookup"><span data-stu-id="ce953-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce953-207">请求</span><span class="sxs-lookup"><span data-stu-id="ce953-207">Request</span></span>
<span data-ttu-id="ce953-208">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce953-208">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 748

{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="ce953-209">响应</span><span class="sxs-lookup"><span data-stu-id="ce953-209">Response</span></span>
<span data-ttu-id="ce953-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ce953-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 920

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




