---
title: 创建 windowsStoreApp
description: 创建新的 windowsStoreApp 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 524c02ac23655f9313c75dffad2bea0c77176431
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394227"
---
# <a name="create-windowsstoreapp"></a><span data-ttu-id="51cb5-103">创建 windowsStoreApp</span><span class="sxs-lookup"><span data-stu-id="51cb5-103">Create windowsStoreApp</span></span>

> <span data-ttu-id="51cb5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="51cb5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="51cb5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="51cb5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51cb5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51cb5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51cb5-107">创建新的[windowsStoreApp](../resources/intune-apps-windowsstoreapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="51cb5-107">Create a new [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51cb5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="51cb5-108">Prerequisites</span></span>
<span data-ttu-id="51cb5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="51cb5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="51cb5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="51cb5-111">Permission type</span></span>|<span data-ttu-id="51cb5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="51cb5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51cb5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51cb5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51cb5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51cb5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="51cb5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51cb5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51cb5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="51cb5-116">Not supported.</span></span>|
|<span data-ttu-id="51cb5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="51cb5-117">Application</span></span>|<span data-ttu-id="51cb5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="51cb5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51cb5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51cb5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="51cb5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="51cb5-120">Request headers</span></span>
|<span data-ttu-id="51cb5-121">标头</span><span class="sxs-lookup"><span data-stu-id="51cb5-121">Header</span></span>|<span data-ttu-id="51cb5-122">值</span><span class="sxs-lookup"><span data-stu-id="51cb5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51cb5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="51cb5-123">Authorization</span></span>|<span data-ttu-id="51cb5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="51cb5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51cb5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="51cb5-125">Accept</span></span>|<span data-ttu-id="51cb5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51cb5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51cb5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="51cb5-127">Request body</span></span>
<span data-ttu-id="51cb5-128">在请求正文中，提供 windowsStoreApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51cb5-128">In the request body, supply a JSON representation for the windowsStoreApp object.</span></span>

<span data-ttu-id="51cb5-129">下表显示时创建 windowsStoreApp 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="51cb5-129">The following table shows the properties that are required when you create the windowsStoreApp.</span></span>

|<span data-ttu-id="51cb5-130">属性</span><span class="sxs-lookup"><span data-stu-id="51cb5-130">Property</span></span>|<span data-ttu-id="51cb5-131">类型</span><span class="sxs-lookup"><span data-stu-id="51cb5-131">Type</span></span>|<span data-ttu-id="51cb5-132">说明</span><span class="sxs-lookup"><span data-stu-id="51cb5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51cb5-133">id</span><span class="sxs-lookup"><span data-stu-id="51cb5-133">id</span></span>|<span data-ttu-id="51cb5-134">String</span><span class="sxs-lookup"><span data-stu-id="51cb5-134">String</span></span>|<span data-ttu-id="51cb5-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="51cb5-135">Key of the entity.</span></span> <span data-ttu-id="51cb5-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51cb5-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51cb5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="51cb5-137">displayName</span></span>|<span data-ttu-id="51cb5-138">String</span><span class="sxs-lookup"><span data-stu-id="51cb5-138">String</span></span>|<span data-ttu-id="51cb5-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="51cb5-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="51cb5-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51cb5-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51cb5-141">description</span><span class="sxs-lookup"><span data-stu-id="51cb5-141">description</span></span>|<span data-ttu-id="51cb5-142">String</span><span class="sxs-lookup"><span data-stu-id="51cb5-142">String</span></span>|<span data-ttu-id="51cb5-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="51cb5-143">The description of the app.</span></span> <span data-ttu-id="51cb5-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51cb5-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51cb5-145">publisher</span><span class="sxs-lookup"><span data-stu-id="51cb5-145">publisher</span></span>|<span data-ttu-id="51cb5-146">String</span><span class="sxs-lookup"><span data-stu-id="51cb5-146">String</span></span>|<span data-ttu-id="51cb5-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="51cb5-147">The publisher of the app.</span></span> <span data-ttu-id="51cb5-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51cb5-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51cb5-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="51cb5-149">largeIcon</span></span>|[<span data-ttu-id="51cb5-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="51cb5-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="51cb5-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="51cb5-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="51cb5-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51cb5-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51cb5-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51cb5-153">createdDateTime</span></span>|<span data-ttu-id="51cb5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51cb5-154">DateTimeOffset</span></span>|<span data-ttu-id="51cb5-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="51cb5-155">The date and time the app was created.</span></span> <span data-ttu-id="51cb5-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51cb5-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51cb5-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51cb5-157">lastModifiedDateTime</span></span>|<span data-ttu-id="51cb5-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51cb5-158">DateTimeOffset</span></span>|<span data-ttu-id="51cb5-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="51cb5-159">The date and time the app was last modified.</span></span> <span data-ttu-id="51cb5-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51cb5-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51cb5-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="51cb5-161">isFeatured</span></span>|<span data-ttu-id="51cb5-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="51cb5-162">Boolean</span></span>|<span data-ttu-id="51cb5-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51cb5-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51cb5-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="51cb5-164">privacyInformationUrl</span></span>|<span data-ttu-id="51cb5-165">String</span><span class="sxs-lookup"><span data-stu-id="51cb5-165">String</span></span>|<span data-ttu-id="51cb5-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="51cb5-166">The privacy statement Url.</span></span> <span data-ttu-id="51cb5-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51cb5-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51cb5-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="51cb5-168">informationUrl</span></span>|<span data-ttu-id="51cb5-169">String</span><span class="sxs-lookup"><span data-stu-id="51cb5-169">String</span></span>|<span data-ttu-id="51cb5-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="51cb5-170">The more information Url.</span></span> <span data-ttu-id="51cb5-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51cb5-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51cb5-172">owner</span><span class="sxs-lookup"><span data-stu-id="51cb5-172">owner</span></span>|<span data-ttu-id="51cb5-173">String</span><span class="sxs-lookup"><span data-stu-id="51cb5-173">String</span></span>|<span data-ttu-id="51cb5-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="51cb5-174">The owner of the app.</span></span> <span data-ttu-id="51cb5-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51cb5-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51cb5-176">developer</span><span class="sxs-lookup"><span data-stu-id="51cb5-176">developer</span></span>|<span data-ttu-id="51cb5-177">String</span><span class="sxs-lookup"><span data-stu-id="51cb5-177">String</span></span>|<span data-ttu-id="51cb5-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="51cb5-178">The developer of the app.</span></span> <span data-ttu-id="51cb5-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51cb5-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51cb5-180">notes</span><span class="sxs-lookup"><span data-stu-id="51cb5-180">notes</span></span>|<span data-ttu-id="51cb5-181">String</span><span class="sxs-lookup"><span data-stu-id="51cb5-181">String</span></span>|<span data-ttu-id="51cb5-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="51cb5-182">Notes for the app.</span></span> <span data-ttu-id="51cb5-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51cb5-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51cb5-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="51cb5-184">uploadState</span></span>|<span data-ttu-id="51cb5-185">Int32</span><span class="sxs-lookup"><span data-stu-id="51cb5-185">Int32</span></span>|<span data-ttu-id="51cb5-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="51cb5-186">The upload state.</span></span> <span data-ttu-id="51cb5-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51cb5-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51cb5-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="51cb5-188">publishingState</span></span>|[<span data-ttu-id="51cb5-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="51cb5-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="51cb5-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="51cb5-190">The publishing state for the app.</span></span> <span data-ttu-id="51cb5-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="51cb5-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="51cb5-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="51cb5-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="51cb5-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="51cb5-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="51cb5-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="51cb5-194">isAssigned</span></span>|<span data-ttu-id="51cb5-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="51cb5-195">Boolean</span></span>|<span data-ttu-id="51cb5-196">值，指示是否将应用程序分配给至少一个组。</span><span class="sxs-lookup"><span data-stu-id="51cb5-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="51cb5-197">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51cb5-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51cb5-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="51cb5-198">roleScopeTagIds</span></span>|<span data-ttu-id="51cb5-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="51cb5-199">String collection</span></span>|<span data-ttu-id="51cb5-200">此移动应用程序的作用域标记 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="51cb5-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="51cb5-201">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51cb5-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51cb5-202">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="51cb5-202">appStoreUrl</span></span>|<span data-ttu-id="51cb5-203">String</span><span class="sxs-lookup"><span data-stu-id="51cb5-203">String</span></span>|<span data-ttu-id="51cb5-204">Windows 应用程序存储 URL。</span><span class="sxs-lookup"><span data-stu-id="51cb5-204">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="51cb5-205">响应</span><span class="sxs-lookup"><span data-stu-id="51cb5-205">Response</span></span>
<span data-ttu-id="51cb5-206">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsStoreApp](../resources/intune-apps-windowsstoreapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="51cb5-206">If successful, this method returns a `201 Created` response code and a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51cb5-207">示例</span><span class="sxs-lookup"><span data-stu-id="51cb5-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="51cb5-208">请求</span><span class="sxs-lookup"><span data-stu-id="51cb5-208">Request</span></span>
<span data-ttu-id="51cb5-209">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="51cb5-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 741

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
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

### <a name="response"></a><span data-ttu-id="51cb5-210">响应</span><span class="sxs-lookup"><span data-stu-id="51cb5-210">Response</span></span>
<span data-ttu-id="51cb5-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="51cb5-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 913

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




