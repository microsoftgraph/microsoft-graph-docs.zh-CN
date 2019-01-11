---
title: 更新 webApp
description: 更新 webApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f1b2362a6a46d33d859ce0eb39f0a117a29aa8fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871090"
---
# <a name="update-webapp"></a><span data-ttu-id="32b45-103">更新 webApp</span><span class="sxs-lookup"><span data-stu-id="32b45-103">Update webApp</span></span>

> <span data-ttu-id="32b45-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="32b45-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32b45-105">更新 [webApp](../resources/intune-apps-webapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="32b45-105">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="32b45-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="32b45-106">Prerequisites</span></span>
<span data-ttu-id="32b45-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="32b45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32b45-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="32b45-109">Permission type</span></span>|<span data-ttu-id="32b45-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="32b45-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32b45-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32b45-111">Delegated (work or school account)</span></span>|<span data-ttu-id="32b45-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32b45-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="32b45-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32b45-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32b45-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="32b45-114">Not supported.</span></span>|
|<span data-ttu-id="32b45-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="32b45-115">Application</span></span>|<span data-ttu-id="32b45-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="32b45-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32b45-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32b45-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="32b45-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="32b45-118">Request headers</span></span>
|<span data-ttu-id="32b45-119">标头</span><span class="sxs-lookup"><span data-stu-id="32b45-119">Header</span></span>|<span data-ttu-id="32b45-120">值</span><span class="sxs-lookup"><span data-stu-id="32b45-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32b45-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="32b45-121">Authorization</span></span>|<span data-ttu-id="32b45-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="32b45-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32b45-123">Accept</span><span class="sxs-lookup"><span data-stu-id="32b45-123">Accept</span></span>|<span data-ttu-id="32b45-124">application/json</span><span class="sxs-lookup"><span data-stu-id="32b45-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32b45-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="32b45-125">Request body</span></span>
<span data-ttu-id="32b45-126">在请求正文中，提供 [webApp](../resources/intune-apps-webapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32b45-126">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="32b45-127">下表显示创建 [webApp](../resources/intune-apps-webapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="32b45-127">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="32b45-128">属性</span><span class="sxs-lookup"><span data-stu-id="32b45-128">Property</span></span>|<span data-ttu-id="32b45-129">类型</span><span class="sxs-lookup"><span data-stu-id="32b45-129">Type</span></span>|<span data-ttu-id="32b45-130">说明</span><span class="sxs-lookup"><span data-stu-id="32b45-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32b45-131">id</span><span class="sxs-lookup"><span data-stu-id="32b45-131">id</span></span>|<span data-ttu-id="32b45-132">String</span><span class="sxs-lookup"><span data-stu-id="32b45-132">String</span></span>|<span data-ttu-id="32b45-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="32b45-133">Key of the entity.</span></span> <span data-ttu-id="32b45-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32b45-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="32b45-135">displayName</span><span class="sxs-lookup"><span data-stu-id="32b45-135">displayName</span></span>|<span data-ttu-id="32b45-136">String</span><span class="sxs-lookup"><span data-stu-id="32b45-136">String</span></span>|<span data-ttu-id="32b45-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="32b45-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="32b45-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32b45-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="32b45-139">description</span><span class="sxs-lookup"><span data-stu-id="32b45-139">description</span></span>|<span data-ttu-id="32b45-140">String</span><span class="sxs-lookup"><span data-stu-id="32b45-140">String</span></span>|<span data-ttu-id="32b45-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="32b45-141">The description of the app.</span></span> <span data-ttu-id="32b45-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32b45-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="32b45-143">publisher</span><span class="sxs-lookup"><span data-stu-id="32b45-143">publisher</span></span>|<span data-ttu-id="32b45-144">String</span><span class="sxs-lookup"><span data-stu-id="32b45-144">String</span></span>|<span data-ttu-id="32b45-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="32b45-145">The publisher of the app.</span></span> <span data-ttu-id="32b45-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32b45-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="32b45-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="32b45-147">largeIcon</span></span>|[<span data-ttu-id="32b45-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="32b45-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="32b45-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="32b45-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="32b45-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32b45-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="32b45-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32b45-151">createdDateTime</span></span>|<span data-ttu-id="32b45-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32b45-152">DateTimeOffset</span></span>|<span data-ttu-id="32b45-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="32b45-153">The date and time the app was created.</span></span> <span data-ttu-id="32b45-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32b45-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="32b45-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32b45-155">lastModifiedDateTime</span></span>|<span data-ttu-id="32b45-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32b45-156">DateTimeOffset</span></span>|<span data-ttu-id="32b45-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="32b45-157">The date and time the app was last modified.</span></span> <span data-ttu-id="32b45-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32b45-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="32b45-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="32b45-159">isFeatured</span></span>|<span data-ttu-id="32b45-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="32b45-160">Boolean</span></span>|<span data-ttu-id="32b45-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32b45-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="32b45-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="32b45-162">privacyInformationUrl</span></span>|<span data-ttu-id="32b45-163">String</span><span class="sxs-lookup"><span data-stu-id="32b45-163">String</span></span>|<span data-ttu-id="32b45-164">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="32b45-164">The privacy statement Url.</span></span> <span data-ttu-id="32b45-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32b45-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="32b45-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="32b45-166">informationUrl</span></span>|<span data-ttu-id="32b45-167">String</span><span class="sxs-lookup"><span data-stu-id="32b45-167">String</span></span>|<span data-ttu-id="32b45-168">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="32b45-168">The more information Url.</span></span> <span data-ttu-id="32b45-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32b45-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="32b45-170">owner</span><span class="sxs-lookup"><span data-stu-id="32b45-170">owner</span></span>|<span data-ttu-id="32b45-171">String</span><span class="sxs-lookup"><span data-stu-id="32b45-171">String</span></span>|<span data-ttu-id="32b45-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="32b45-172">The owner of the app.</span></span> <span data-ttu-id="32b45-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32b45-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="32b45-174">developer</span><span class="sxs-lookup"><span data-stu-id="32b45-174">developer</span></span>|<span data-ttu-id="32b45-175">String</span><span class="sxs-lookup"><span data-stu-id="32b45-175">String</span></span>|<span data-ttu-id="32b45-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="32b45-176">The developer of the app.</span></span> <span data-ttu-id="32b45-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32b45-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="32b45-178">notes</span><span class="sxs-lookup"><span data-stu-id="32b45-178">notes</span></span>|<span data-ttu-id="32b45-179">String</span><span class="sxs-lookup"><span data-stu-id="32b45-179">String</span></span>|<span data-ttu-id="32b45-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="32b45-180">Notes for the app.</span></span> <span data-ttu-id="32b45-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32b45-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="32b45-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="32b45-182">publishingState</span></span>|[<span data-ttu-id="32b45-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="32b45-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="32b45-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="32b45-184">The publishing state for the app.</span></span> <span data-ttu-id="32b45-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="32b45-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="32b45-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="32b45-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="32b45-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="32b45-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="32b45-188">appUrl</span><span class="sxs-lookup"><span data-stu-id="32b45-188">appUrl</span></span>|<span data-ttu-id="32b45-189">String</span><span class="sxs-lookup"><span data-stu-id="32b45-189">String</span></span>|<span data-ttu-id="32b45-190">Web 应用 URL。</span><span class="sxs-lookup"><span data-stu-id="32b45-190">The web app URL.</span></span>|
|<span data-ttu-id="32b45-191">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="32b45-191">useManagedBrowser</span></span>|<span data-ttu-id="32b45-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="32b45-192">Boolean</span></span>|<span data-ttu-id="32b45-193">是否使用托管浏览器。</span><span class="sxs-lookup"><span data-stu-id="32b45-193">Whether or not to use managed browser.</span></span> <span data-ttu-id="32b45-194">此属性仅适用于 Android 和 iOS。</span><span class="sxs-lookup"><span data-stu-id="32b45-194">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="32b45-195">响应</span><span class="sxs-lookup"><span data-stu-id="32b45-195">Response</span></span>
<span data-ttu-id="32b45-196">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [webApp](../resources/intune-apps-webapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="32b45-196">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32b45-197">示例</span><span class="sxs-lookup"><span data-stu-id="32b45-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="32b45-198">请求</span><span class="sxs-lookup"><span data-stu-id="32b45-198">Request</span></span>
<span data-ttu-id="32b45-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="32b45-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="32b45-200">响应</span><span class="sxs-lookup"><span data-stu-id="32b45-200">Response</span></span>
<span data-ttu-id="32b45-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="32b45-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



