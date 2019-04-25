---
title: 创建 androidStoreApp
description: 创建新的 androidStoreApp 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cabceb70911a4de50b26b01ea4856791a747d46
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577516"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="ec84b-103">创建 androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="ec84b-103">Create androidStoreApp</span></span>

> <span data-ttu-id="ec84b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ec84b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec84b-105">创建新的 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ec84b-105">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec84b-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="ec84b-106">Prerequisites</span></span>
<span data-ttu-id="ec84b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec84b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec84b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec84b-109">Permission type</span></span>|<span data-ttu-id="ec84b-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ec84b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec84b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec84b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ec84b-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec84b-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ec84b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec84b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec84b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec84b-114">Not supported.</span></span>|
|<span data-ttu-id="ec84b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec84b-115">Application</span></span>|<span data-ttu-id="ec84b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec84b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec84b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec84b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ec84b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec84b-118">Request headers</span></span>
|<span data-ttu-id="ec84b-119">标头</span><span class="sxs-lookup"><span data-stu-id="ec84b-119">Header</span></span>|<span data-ttu-id="ec84b-120">值</span><span class="sxs-lookup"><span data-stu-id="ec84b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec84b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec84b-121">Authorization</span></span>|<span data-ttu-id="ec84b-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ec84b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec84b-123">接受</span><span class="sxs-lookup"><span data-stu-id="ec84b-123">Accept</span></span>|<span data-ttu-id="ec84b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ec84b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec84b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec84b-125">Request body</span></span>
<span data-ttu-id="ec84b-126">在请求正文中，提供 androidStoreApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec84b-126">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="ec84b-127">下表显示创建 androidStoreApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ec84b-127">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="ec84b-128">属性</span><span class="sxs-lookup"><span data-stu-id="ec84b-128">Property</span></span>|<span data-ttu-id="ec84b-129">类型</span><span class="sxs-lookup"><span data-stu-id="ec84b-129">Type</span></span>|<span data-ttu-id="ec84b-130">说明</span><span class="sxs-lookup"><span data-stu-id="ec84b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec84b-131">id</span><span class="sxs-lookup"><span data-stu-id="ec84b-131">id</span></span>|<span data-ttu-id="ec84b-132">字符串</span><span class="sxs-lookup"><span data-stu-id="ec84b-132">String</span></span>|<span data-ttu-id="ec84b-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ec84b-133">Key of the entity.</span></span> <span data-ttu-id="ec84b-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec84b-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec84b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ec84b-135">displayName</span></span>|<span data-ttu-id="ec84b-136">String</span><span class="sxs-lookup"><span data-stu-id="ec84b-136">String</span></span>|<span data-ttu-id="ec84b-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="ec84b-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ec84b-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec84b-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec84b-139">说明</span><span class="sxs-lookup"><span data-stu-id="ec84b-139">description</span></span>|<span data-ttu-id="ec84b-140">String</span><span class="sxs-lookup"><span data-stu-id="ec84b-140">String</span></span>|<span data-ttu-id="ec84b-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="ec84b-141">The description of the app.</span></span> <span data-ttu-id="ec84b-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec84b-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec84b-143">publisher</span><span class="sxs-lookup"><span data-stu-id="ec84b-143">publisher</span></span>|<span data-ttu-id="ec84b-144">String</span><span class="sxs-lookup"><span data-stu-id="ec84b-144">String</span></span>|<span data-ttu-id="ec84b-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="ec84b-145">The publisher of the app.</span></span> <span data-ttu-id="ec84b-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec84b-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec84b-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ec84b-147">largeIcon</span></span>|[<span data-ttu-id="ec84b-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ec84b-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ec84b-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="ec84b-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ec84b-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec84b-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec84b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ec84b-151">createdDateTime</span></span>|<span data-ttu-id="ec84b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec84b-152">DateTimeOffset</span></span>|<span data-ttu-id="ec84b-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ec84b-153">The date and time the app was created.</span></span> <span data-ttu-id="ec84b-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec84b-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec84b-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec84b-155">lastModifiedDateTime</span></span>|<span data-ttu-id="ec84b-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec84b-156">DateTimeOffset</span></span>|<span data-ttu-id="ec84b-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ec84b-157">The date and time the app was last modified.</span></span> <span data-ttu-id="ec84b-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec84b-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec84b-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ec84b-159">isFeatured</span></span>|<span data-ttu-id="ec84b-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec84b-160">Boolean</span></span>|<span data-ttu-id="ec84b-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec84b-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec84b-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ec84b-162">privacyInformationUrl</span></span>|<span data-ttu-id="ec84b-163">String</span><span class="sxs-lookup"><span data-stu-id="ec84b-163">String</span></span>|<span data-ttu-id="ec84b-164">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="ec84b-164">The privacy statement Url.</span></span> <span data-ttu-id="ec84b-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec84b-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec84b-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ec84b-166">informationUrl</span></span>|<span data-ttu-id="ec84b-167">String</span><span class="sxs-lookup"><span data-stu-id="ec84b-167">String</span></span>|<span data-ttu-id="ec84b-168">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="ec84b-168">The more information Url.</span></span> <span data-ttu-id="ec84b-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec84b-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec84b-170">owner</span><span class="sxs-lookup"><span data-stu-id="ec84b-170">owner</span></span>|<span data-ttu-id="ec84b-171">字符串</span><span class="sxs-lookup"><span data-stu-id="ec84b-171">String</span></span>|<span data-ttu-id="ec84b-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="ec84b-172">The owner of the app.</span></span> <span data-ttu-id="ec84b-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec84b-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec84b-174">developer</span><span class="sxs-lookup"><span data-stu-id="ec84b-174">developer</span></span>|<span data-ttu-id="ec84b-175">String</span><span class="sxs-lookup"><span data-stu-id="ec84b-175">String</span></span>|<span data-ttu-id="ec84b-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="ec84b-176">The developer of the app.</span></span> <span data-ttu-id="ec84b-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec84b-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec84b-178">notes</span><span class="sxs-lookup"><span data-stu-id="ec84b-178">notes</span></span>|<span data-ttu-id="ec84b-179">String</span><span class="sxs-lookup"><span data-stu-id="ec84b-179">String</span></span>|<span data-ttu-id="ec84b-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="ec84b-180">Notes for the app.</span></span> <span data-ttu-id="ec84b-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec84b-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec84b-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="ec84b-182">publishingState</span></span>|[<span data-ttu-id="ec84b-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ec84b-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ec84b-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="ec84b-184">The publishing state for the app.</span></span> <span data-ttu-id="ec84b-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="ec84b-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ec84b-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="ec84b-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ec84b-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="ec84b-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ec84b-188">packageId</span><span class="sxs-lookup"><span data-stu-id="ec84b-188">packageId</span></span>|<span data-ttu-id="ec84b-189">String</span><span class="sxs-lookup"><span data-stu-id="ec84b-189">String</span></span>|<span data-ttu-id="ec84b-190">包标识符。</span><span class="sxs-lookup"><span data-stu-id="ec84b-190">The package identifier.</span></span>|
|<span data-ttu-id="ec84b-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ec84b-191">appStoreUrl</span></span>|<span data-ttu-id="ec84b-192">String</span><span class="sxs-lookup"><span data-stu-id="ec84b-192">String</span></span>|<span data-ttu-id="ec84b-193">Android 应用商店 URL。</span><span class="sxs-lookup"><span data-stu-id="ec84b-193">The Android app store URL.</span></span>|
|<span data-ttu-id="ec84b-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ec84b-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ec84b-195">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ec84b-195">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="ec84b-196">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="ec84b-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="ec84b-197">响应</span><span class="sxs-lookup"><span data-stu-id="ec84b-197">Response</span></span>
<span data-ttu-id="ec84b-198">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ec84b-198">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec84b-199">示例</span><span class="sxs-lookup"><span data-stu-id="ec84b-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec84b-200">请求</span><span class="sxs-lookup"><span data-stu-id="ec84b-200">Request</span></span>
<span data-ttu-id="ec84b-201">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ec84b-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 938

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```

### <a name="response"></a><span data-ttu-id="ec84b-202">响应</span><span class="sxs-lookup"><span data-stu-id="ec84b-202">Response</span></span>
<span data-ttu-id="ec84b-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ec84b-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1110

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```



