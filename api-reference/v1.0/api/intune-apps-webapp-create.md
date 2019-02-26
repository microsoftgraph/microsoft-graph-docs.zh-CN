---
title: 创建 webApp
description: 创建新的 webApp 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf435ce228e8f169b76ac03def68a2a84f472f84
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252698"
---
# <a name="create-webapp"></a><span data-ttu-id="66af7-103">创建 webApp</span><span class="sxs-lookup"><span data-stu-id="66af7-103">Create webApp</span></span>

> <span data-ttu-id="66af7-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66af7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66af7-105">创建新的 [webApp](../resources/intune-apps-webapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="66af7-105">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66af7-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="66af7-106">Prerequisites</span></span>
<span data-ttu-id="66af7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="66af7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="66af7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="66af7-109">Permission type</span></span>|<span data-ttu-id="66af7-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="66af7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66af7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66af7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="66af7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66af7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="66af7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66af7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66af7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="66af7-114">Not supported.</span></span>|
|<span data-ttu-id="66af7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="66af7-115">Application</span></span>|<span data-ttu-id="66af7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="66af7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66af7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66af7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="66af7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="66af7-118">Request headers</span></span>
|<span data-ttu-id="66af7-119">标头</span><span class="sxs-lookup"><span data-stu-id="66af7-119">Header</span></span>|<span data-ttu-id="66af7-120">值</span><span class="sxs-lookup"><span data-stu-id="66af7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66af7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="66af7-121">Authorization</span></span>|<span data-ttu-id="66af7-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="66af7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66af7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="66af7-123">Accept</span></span>|<span data-ttu-id="66af7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="66af7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66af7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="66af7-125">Request body</span></span>
<span data-ttu-id="66af7-126">在请求正文中，提供 webApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66af7-126">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="66af7-127">下表显示创建 webApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="66af7-127">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="66af7-128">属性</span><span class="sxs-lookup"><span data-stu-id="66af7-128">Property</span></span>|<span data-ttu-id="66af7-129">类型</span><span class="sxs-lookup"><span data-stu-id="66af7-129">Type</span></span>|<span data-ttu-id="66af7-130">说明</span><span class="sxs-lookup"><span data-stu-id="66af7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66af7-131">id</span><span class="sxs-lookup"><span data-stu-id="66af7-131">id</span></span>|<span data-ttu-id="66af7-132">字符串</span><span class="sxs-lookup"><span data-stu-id="66af7-132">String</span></span>|<span data-ttu-id="66af7-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="66af7-133">Key of the entity.</span></span> <span data-ttu-id="66af7-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66af7-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66af7-135">displayName</span><span class="sxs-lookup"><span data-stu-id="66af7-135">displayName</span></span>|<span data-ttu-id="66af7-136">String</span><span class="sxs-lookup"><span data-stu-id="66af7-136">String</span></span>|<span data-ttu-id="66af7-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="66af7-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="66af7-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66af7-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66af7-139">description</span><span class="sxs-lookup"><span data-stu-id="66af7-139">description</span></span>|<span data-ttu-id="66af7-140">字符串</span><span class="sxs-lookup"><span data-stu-id="66af7-140">String</span></span>|<span data-ttu-id="66af7-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="66af7-141">The description of the app.</span></span> <span data-ttu-id="66af7-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66af7-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66af7-143">publisher</span><span class="sxs-lookup"><span data-stu-id="66af7-143">publisher</span></span>|<span data-ttu-id="66af7-144">String</span><span class="sxs-lookup"><span data-stu-id="66af7-144">String</span></span>|<span data-ttu-id="66af7-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="66af7-145">The publisher of the app.</span></span> <span data-ttu-id="66af7-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66af7-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66af7-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="66af7-147">largeIcon</span></span>|[<span data-ttu-id="66af7-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="66af7-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="66af7-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="66af7-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="66af7-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66af7-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66af7-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66af7-151">createdDateTime</span></span>|<span data-ttu-id="66af7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66af7-152">DateTimeOffset</span></span>|<span data-ttu-id="66af7-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="66af7-153">The date and time the app was created.</span></span> <span data-ttu-id="66af7-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66af7-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66af7-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66af7-155">lastModifiedDateTime</span></span>|<span data-ttu-id="66af7-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66af7-156">DateTimeOffset</span></span>|<span data-ttu-id="66af7-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="66af7-157">The date and time the app was last modified.</span></span> <span data-ttu-id="66af7-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66af7-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66af7-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="66af7-159">isFeatured</span></span>|<span data-ttu-id="66af7-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="66af7-160">Boolean</span></span>|<span data-ttu-id="66af7-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66af7-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66af7-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="66af7-162">privacyInformationUrl</span></span>|<span data-ttu-id="66af7-163">String</span><span class="sxs-lookup"><span data-stu-id="66af7-163">String</span></span>|<span data-ttu-id="66af7-164">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="66af7-164">The privacy statement Url.</span></span> <span data-ttu-id="66af7-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66af7-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66af7-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="66af7-166">informationUrl</span></span>|<span data-ttu-id="66af7-167">String</span><span class="sxs-lookup"><span data-stu-id="66af7-167">String</span></span>|<span data-ttu-id="66af7-168">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="66af7-168">The more information Url.</span></span> <span data-ttu-id="66af7-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66af7-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66af7-170">owner</span><span class="sxs-lookup"><span data-stu-id="66af7-170">owner</span></span>|<span data-ttu-id="66af7-171">String</span><span class="sxs-lookup"><span data-stu-id="66af7-171">String</span></span>|<span data-ttu-id="66af7-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="66af7-172">The owner of the app.</span></span> <span data-ttu-id="66af7-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66af7-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66af7-174">developer</span><span class="sxs-lookup"><span data-stu-id="66af7-174">developer</span></span>|<span data-ttu-id="66af7-175">String</span><span class="sxs-lookup"><span data-stu-id="66af7-175">String</span></span>|<span data-ttu-id="66af7-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="66af7-176">The developer of the app.</span></span> <span data-ttu-id="66af7-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66af7-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66af7-178">notes</span><span class="sxs-lookup"><span data-stu-id="66af7-178">notes</span></span>|<span data-ttu-id="66af7-179">String</span><span class="sxs-lookup"><span data-stu-id="66af7-179">String</span></span>|<span data-ttu-id="66af7-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="66af7-180">Notes for the app.</span></span> <span data-ttu-id="66af7-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66af7-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66af7-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="66af7-182">publishingState</span></span>|[<span data-ttu-id="66af7-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="66af7-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="66af7-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="66af7-184">The publishing state for the app.</span></span> <span data-ttu-id="66af7-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="66af7-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="66af7-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="66af7-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="66af7-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="66af7-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="66af7-188">appUrl</span><span class="sxs-lookup"><span data-stu-id="66af7-188">appUrl</span></span>|<span data-ttu-id="66af7-189">String</span><span class="sxs-lookup"><span data-stu-id="66af7-189">String</span></span>|<span data-ttu-id="66af7-190">Web 应用 URL。</span><span class="sxs-lookup"><span data-stu-id="66af7-190">The web app URL.</span></span>|
|<span data-ttu-id="66af7-191">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="66af7-191">useManagedBrowser</span></span>|<span data-ttu-id="66af7-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="66af7-192">Boolean</span></span>|<span data-ttu-id="66af7-193">是否使用托管浏览器。</span><span class="sxs-lookup"><span data-stu-id="66af7-193">Whether or not to use managed browser.</span></span> <span data-ttu-id="66af7-194">此属性仅适用于 Android 和 iOS。</span><span class="sxs-lookup"><span data-stu-id="66af7-194">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="66af7-195">响应</span><span class="sxs-lookup"><span data-stu-id="66af7-195">Response</span></span>
<span data-ttu-id="66af7-196">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [webApp](../resources/intune-apps-webapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="66af7-196">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66af7-197">示例</span><span class="sxs-lookup"><span data-stu-id="66af7-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="66af7-198">请求</span><span class="sxs-lookup"><span data-stu-id="66af7-198">Request</span></span>
<span data-ttu-id="66af7-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66af7-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 645

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
  "publishingState": "processing",
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="66af7-200">响应</span><span class="sxs-lookup"><span data-stu-id="66af7-200">Response</span></span>
<span data-ttu-id="66af7-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66af7-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 817

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
  "publishingState": "processing",
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```



