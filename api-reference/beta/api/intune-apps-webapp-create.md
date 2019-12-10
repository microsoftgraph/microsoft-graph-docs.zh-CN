---
title: 创建 webApp
description: 创建新的 webApp 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 88481853c5b6734defea02bdac32b8d66480a145
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39934201"
---
# <a name="create-webapp"></a><span data-ttu-id="c6e65-103">创建 webApp</span><span class="sxs-lookup"><span data-stu-id="c6e65-103">Create webApp</span></span>

> <span data-ttu-id="c6e65-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c6e65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6e65-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6e65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6e65-106">创建新的 [webApp](../resources/intune-apps-webapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6e65-106">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6e65-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c6e65-107">Prerequisites</span></span>
<span data-ttu-id="c6e65-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6e65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6e65-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6e65-110">Permission type</span></span>|<span data-ttu-id="c6e65-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c6e65-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6e65-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6e65-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6e65-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6e65-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c6e65-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6e65-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6e65-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6e65-115">Not supported.</span></span>|
|<span data-ttu-id="c6e65-116">Application</span><span class="sxs-lookup"><span data-stu-id="c6e65-116">Application</span></span>|<span data-ttu-id="c6e65-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6e65-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6e65-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6e65-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c6e65-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6e65-119">Request headers</span></span>
|<span data-ttu-id="c6e65-120">标头</span><span class="sxs-lookup"><span data-stu-id="c6e65-120">Header</span></span>|<span data-ttu-id="c6e65-121">值</span><span class="sxs-lookup"><span data-stu-id="c6e65-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6e65-122">授权</span><span class="sxs-lookup"><span data-stu-id="c6e65-122">Authorization</span></span>|<span data-ttu-id="c6e65-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c6e65-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6e65-124">接受</span><span class="sxs-lookup"><span data-stu-id="c6e65-124">Accept</span></span>|<span data-ttu-id="c6e65-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c6e65-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6e65-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6e65-126">Request body</span></span>
<span data-ttu-id="c6e65-127">在请求正文中，提供 webApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6e65-127">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="c6e65-128">下表显示创建 webApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c6e65-128">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="c6e65-129">属性</span><span class="sxs-lookup"><span data-stu-id="c6e65-129">Property</span></span>|<span data-ttu-id="c6e65-130">类型</span><span class="sxs-lookup"><span data-stu-id="c6e65-130">Type</span></span>|<span data-ttu-id="c6e65-131">说明</span><span class="sxs-lookup"><span data-stu-id="c6e65-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6e65-132">id</span><span class="sxs-lookup"><span data-stu-id="c6e65-132">id</span></span>|<span data-ttu-id="c6e65-133">字符串</span><span class="sxs-lookup"><span data-stu-id="c6e65-133">String</span></span>|<span data-ttu-id="c6e65-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c6e65-134">Key of the entity.</span></span> <span data-ttu-id="c6e65-135">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6e65-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e65-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c6e65-136">displayName</span></span>|<span data-ttu-id="c6e65-137">字符串</span><span class="sxs-lookup"><span data-stu-id="c6e65-137">String</span></span>|<span data-ttu-id="c6e65-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="c6e65-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c6e65-139">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6e65-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e65-140">说明</span><span class="sxs-lookup"><span data-stu-id="c6e65-140">description</span></span>|<span data-ttu-id="c6e65-141">字符串</span><span class="sxs-lookup"><span data-stu-id="c6e65-141">String</span></span>|<span data-ttu-id="c6e65-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="c6e65-142">The description of the app.</span></span> <span data-ttu-id="c6e65-143">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6e65-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e65-144">publisher</span><span class="sxs-lookup"><span data-stu-id="c6e65-144">publisher</span></span>|<span data-ttu-id="c6e65-145">字符串</span><span class="sxs-lookup"><span data-stu-id="c6e65-145">String</span></span>|<span data-ttu-id="c6e65-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="c6e65-146">The publisher of the app.</span></span> <span data-ttu-id="c6e65-147">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6e65-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e65-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c6e65-148">largeIcon</span></span>|[<span data-ttu-id="c6e65-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c6e65-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c6e65-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="c6e65-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c6e65-151">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6e65-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e65-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6e65-152">createdDateTime</span></span>|<span data-ttu-id="c6e65-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6e65-153">DateTimeOffset</span></span>|<span data-ttu-id="c6e65-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c6e65-154">The date and time the app was created.</span></span> <span data-ttu-id="c6e65-155">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6e65-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e65-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6e65-156">lastModifiedDateTime</span></span>|<span data-ttu-id="c6e65-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6e65-157">DateTimeOffset</span></span>|<span data-ttu-id="c6e65-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c6e65-158">The date and time the app was last modified.</span></span> <span data-ttu-id="c6e65-159">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6e65-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e65-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c6e65-160">isFeatured</span></span>|<span data-ttu-id="c6e65-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6e65-161">Boolean</span></span>|<span data-ttu-id="c6e65-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6e65-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e65-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c6e65-163">privacyInformationUrl</span></span>|<span data-ttu-id="c6e65-164">字符串</span><span class="sxs-lookup"><span data-stu-id="c6e65-164">String</span></span>|<span data-ttu-id="c6e65-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="c6e65-165">The privacy statement Url.</span></span> <span data-ttu-id="c6e65-166">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6e65-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e65-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c6e65-167">informationUrl</span></span>|<span data-ttu-id="c6e65-168">字符串</span><span class="sxs-lookup"><span data-stu-id="c6e65-168">String</span></span>|<span data-ttu-id="c6e65-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="c6e65-169">The more information Url.</span></span> <span data-ttu-id="c6e65-170">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6e65-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e65-171">owner</span><span class="sxs-lookup"><span data-stu-id="c6e65-171">owner</span></span>|<span data-ttu-id="c6e65-172">String</span><span class="sxs-lookup"><span data-stu-id="c6e65-172">String</span></span>|<span data-ttu-id="c6e65-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="c6e65-173">The owner of the app.</span></span> <span data-ttu-id="c6e65-174">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6e65-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e65-175">developer</span><span class="sxs-lookup"><span data-stu-id="c6e65-175">developer</span></span>|<span data-ttu-id="c6e65-176">字符串</span><span class="sxs-lookup"><span data-stu-id="c6e65-176">String</span></span>|<span data-ttu-id="c6e65-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="c6e65-177">The developer of the app.</span></span> <span data-ttu-id="c6e65-178">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6e65-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e65-179">notes</span><span class="sxs-lookup"><span data-stu-id="c6e65-179">notes</span></span>|<span data-ttu-id="c6e65-180">字符串</span><span class="sxs-lookup"><span data-stu-id="c6e65-180">String</span></span>|<span data-ttu-id="c6e65-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="c6e65-181">Notes for the app.</span></span> <span data-ttu-id="c6e65-182">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6e65-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e65-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="c6e65-183">uploadState</span></span>|<span data-ttu-id="c6e65-184">Int32</span><span class="sxs-lookup"><span data-stu-id="c6e65-184">Int32</span></span>|<span data-ttu-id="c6e65-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="c6e65-185">The upload state.</span></span> <span data-ttu-id="c6e65-186">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6e65-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e65-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="c6e65-187">publishingState</span></span>|[<span data-ttu-id="c6e65-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c6e65-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c6e65-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="c6e65-189">The publishing state for the app.</span></span> <span data-ttu-id="c6e65-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="c6e65-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c6e65-191">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="c6e65-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="c6e65-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="c6e65-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c6e65-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c6e65-193">isAssigned</span></span>|<span data-ttu-id="c6e65-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6e65-194">Boolean</span></span>|<span data-ttu-id="c6e65-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="c6e65-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c6e65-196">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6e65-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e65-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c6e65-197">roleScopeTagIds</span></span>|<span data-ttu-id="c6e65-198">String collection</span><span class="sxs-lookup"><span data-stu-id="c6e65-198">String collection</span></span>|<span data-ttu-id="c6e65-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="c6e65-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c6e65-200">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6e65-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e65-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="c6e65-201">dependentAppCount</span></span>|<span data-ttu-id="c6e65-202">Int32</span><span class="sxs-lookup"><span data-stu-id="c6e65-202">Int32</span></span>|<span data-ttu-id="c6e65-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="c6e65-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="c6e65-204">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6e65-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c6e65-205">appUrl</span><span class="sxs-lookup"><span data-stu-id="c6e65-205">appUrl</span></span>|<span data-ttu-id="c6e65-206">String</span><span class="sxs-lookup"><span data-stu-id="c6e65-206">String</span></span>|<span data-ttu-id="c6e65-207">Web 应用 URL。</span><span class="sxs-lookup"><span data-stu-id="c6e65-207">The web app URL.</span></span>|
|<span data-ttu-id="c6e65-208">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="c6e65-208">useManagedBrowser</span></span>|<span data-ttu-id="c6e65-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6e65-209">Boolean</span></span>|<span data-ttu-id="c6e65-210">是否使用托管浏览器。</span><span class="sxs-lookup"><span data-stu-id="c6e65-210">Whether or not to use managed browser.</span></span> <span data-ttu-id="c6e65-211">此属性仅适用于 Android 和 iOS。</span><span class="sxs-lookup"><span data-stu-id="c6e65-211">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="c6e65-212">响应</span><span class="sxs-lookup"><span data-stu-id="c6e65-212">Response</span></span>
<span data-ttu-id="c6e65-213">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [webApp](../resources/intune-apps-webapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6e65-213">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6e65-214">示例</span><span class="sxs-lookup"><span data-stu-id="c6e65-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6e65-215">请求</span><span class="sxs-lookup"><span data-stu-id="c6e65-215">Request</span></span>
<span data-ttu-id="c6e65-216">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c6e65-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="c6e65-217">响应</span><span class="sxs-lookup"><span data-stu-id="c6e65-217">Response</span></span>
<span data-ttu-id="c6e65-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c6e65-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





