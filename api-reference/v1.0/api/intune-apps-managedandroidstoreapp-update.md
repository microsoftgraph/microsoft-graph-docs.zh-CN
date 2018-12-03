---
title: 更新 managedAndroidStoreApp
description: 更新 managedAndroidStoreApp 对象的属性。
ms.openlocfilehash: 9e2ec9983c2f658c0b085616835c2b24b8ae2c60
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008794"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="5fad6-103">更新 managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="5fad6-103">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="5fad6-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5fad6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5fad6-105">更新 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5fad6-105">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5fad6-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="5fad6-106">Prerequisites</span></span>
<span data-ttu-id="5fad6-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="5fad6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fad6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5fad6-109">Permission type</span></span>|<span data-ttu-id="5fad6-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5fad6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fad6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5fad6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5fad6-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fad6-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5fad6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5fad6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fad6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5fad6-114">Not supported.</span></span>|
|<span data-ttu-id="5fad6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5fad6-115">Application</span></span>|<span data-ttu-id="5fad6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5fad6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fad6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5fad6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="5fad6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5fad6-118">Request headers</span></span>
|<span data-ttu-id="5fad6-119">标头</span><span class="sxs-lookup"><span data-stu-id="5fad6-119">Header</span></span>|<span data-ttu-id="5fad6-120">值</span><span class="sxs-lookup"><span data-stu-id="5fad6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fad6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fad6-121">Authorization</span></span>|<span data-ttu-id="5fad6-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5fad6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fad6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5fad6-123">Accept</span></span>|<span data-ttu-id="5fad6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5fad6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fad6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5fad6-125">Request body</span></span>
<span data-ttu-id="5fad6-126">在请求正文中，提供 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fad6-126">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="5fad6-127">下表显示了创建 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5fad6-127">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="5fad6-128">属性</span><span class="sxs-lookup"><span data-stu-id="5fad6-128">Property</span></span>|<span data-ttu-id="5fad6-129">类型</span><span class="sxs-lookup"><span data-stu-id="5fad6-129">Type</span></span>|<span data-ttu-id="5fad6-130">说明</span><span class="sxs-lookup"><span data-stu-id="5fad6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fad6-131">id</span><span class="sxs-lookup"><span data-stu-id="5fad6-131">id</span></span>|<span data-ttu-id="5fad6-132">String</span><span class="sxs-lookup"><span data-stu-id="5fad6-132">String</span></span>|<span data-ttu-id="5fad6-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5fad6-133">Key of the entity.</span></span> <span data-ttu-id="5fad6-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fad6-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5fad6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="5fad6-135">displayName</span></span>|<span data-ttu-id="5fad6-136">String</span><span class="sxs-lookup"><span data-stu-id="5fad6-136">String</span></span>|<span data-ttu-id="5fad6-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="5fad6-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5fad6-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fad6-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5fad6-139">description</span><span class="sxs-lookup"><span data-stu-id="5fad6-139">description</span></span>|<span data-ttu-id="5fad6-140">String</span><span class="sxs-lookup"><span data-stu-id="5fad6-140">String</span></span>|<span data-ttu-id="5fad6-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="5fad6-141">The description of the app.</span></span> <span data-ttu-id="5fad6-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fad6-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5fad6-143">publisher</span><span class="sxs-lookup"><span data-stu-id="5fad6-143">publisher</span></span>|<span data-ttu-id="5fad6-144">String</span><span class="sxs-lookup"><span data-stu-id="5fad6-144">String</span></span>|<span data-ttu-id="5fad6-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="5fad6-145">The publisher of the app.</span></span> <span data-ttu-id="5fad6-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fad6-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5fad6-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5fad6-147">largeIcon</span></span>|[<span data-ttu-id="5fad6-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5fad6-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5fad6-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="5fad6-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5fad6-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fad6-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5fad6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5fad6-151">createdDateTime</span></span>|<span data-ttu-id="5fad6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fad6-152">DateTimeOffset</span></span>|<span data-ttu-id="5fad6-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5fad6-153">The date and time the app was created.</span></span> <span data-ttu-id="5fad6-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fad6-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5fad6-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5fad6-155">lastModifiedDateTime</span></span>|<span data-ttu-id="5fad6-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fad6-156">DateTimeOffset</span></span>|<span data-ttu-id="5fad6-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5fad6-157">The date and time the app was last modified.</span></span> <span data-ttu-id="5fad6-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fad6-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5fad6-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5fad6-159">isFeatured</span></span>|<span data-ttu-id="5fad6-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fad6-160">Boolean</span></span>|<span data-ttu-id="5fad6-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fad6-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5fad6-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5fad6-162">privacyInformationUrl</span></span>|<span data-ttu-id="5fad6-163">String</span><span class="sxs-lookup"><span data-stu-id="5fad6-163">String</span></span>|<span data-ttu-id="5fad6-164">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="5fad6-164">The privacy statement Url.</span></span> <span data-ttu-id="5fad6-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fad6-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5fad6-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5fad6-166">informationUrl</span></span>|<span data-ttu-id="5fad6-167">String</span><span class="sxs-lookup"><span data-stu-id="5fad6-167">String</span></span>|<span data-ttu-id="5fad6-168">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="5fad6-168">The more information Url.</span></span> <span data-ttu-id="5fad6-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fad6-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5fad6-170">owner</span><span class="sxs-lookup"><span data-stu-id="5fad6-170">owner</span></span>|<span data-ttu-id="5fad6-171">String</span><span class="sxs-lookup"><span data-stu-id="5fad6-171">String</span></span>|<span data-ttu-id="5fad6-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="5fad6-172">The owner of the app.</span></span> <span data-ttu-id="5fad6-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fad6-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5fad6-174">developer</span><span class="sxs-lookup"><span data-stu-id="5fad6-174">developer</span></span>|<span data-ttu-id="5fad6-175">String</span><span class="sxs-lookup"><span data-stu-id="5fad6-175">String</span></span>|<span data-ttu-id="5fad6-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="5fad6-176">The developer of the app.</span></span> <span data-ttu-id="5fad6-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fad6-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5fad6-178">notes</span><span class="sxs-lookup"><span data-stu-id="5fad6-178">notes</span></span>|<span data-ttu-id="5fad6-179">String</span><span class="sxs-lookup"><span data-stu-id="5fad6-179">String</span></span>|<span data-ttu-id="5fad6-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="5fad6-180">Notes for the app.</span></span> <span data-ttu-id="5fad6-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fad6-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5fad6-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="5fad6-182">publishingState</span></span>|[<span data-ttu-id="5fad6-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5fad6-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5fad6-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="5fad6-184">The publishing state for the app.</span></span> <span data-ttu-id="5fad6-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="5fad6-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5fad6-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="5fad6-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5fad6-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="5fad6-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5fad6-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="5fad6-188">appAvailability</span></span>|[<span data-ttu-id="5fad6-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="5fad6-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="5fad6-190">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="5fad6-190">The Application's availability.</span></span> <span data-ttu-id="5fad6-191">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="5fad6-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="5fad6-192">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="5fad6-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="5fad6-193">version</span><span class="sxs-lookup"><span data-stu-id="5fad6-193">version</span></span>|<span data-ttu-id="5fad6-194">String</span><span class="sxs-lookup"><span data-stu-id="5fad6-194">String</span></span>|<span data-ttu-id="5fad6-195">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="5fad6-195">The Application's version.</span></span> <span data-ttu-id="5fad6-196">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fad6-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="5fad6-197">packageId</span><span class="sxs-lookup"><span data-stu-id="5fad6-197">packageId</span></span>|<span data-ttu-id="5fad6-198">String</span><span class="sxs-lookup"><span data-stu-id="5fad6-198">String</span></span>|<span data-ttu-id="5fad6-199">应用的包 ID。</span><span class="sxs-lookup"><span data-stu-id="5fad6-199">The app's package ID.</span></span>|
|<span data-ttu-id="5fad6-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="5fad6-200">appStoreUrl</span></span>|<span data-ttu-id="5fad6-201">String</span><span class="sxs-lookup"><span data-stu-id="5fad6-201">String</span></span>|<span data-ttu-id="5fad6-202">Android AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="5fad6-202">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="5fad6-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5fad6-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="5fad6-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5fad6-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="5fad6-205">最低受支持操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="5fad6-205">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="5fad6-206">响应</span><span class="sxs-lookup"><span data-stu-id="5fad6-206">Response</span></span>
<span data-ttu-id="5fad6-207">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5fad6-207">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fad6-208">示例</span><span class="sxs-lookup"><span data-stu-id="5fad6-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="5fad6-209">请求</span><span class="sxs-lookup"><span data-stu-id="5fad6-209">Request</span></span>
<span data-ttu-id="5fad6-210">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5fad6-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1016

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="5fad6-211">响应</span><span class="sxs-lookup"><span data-stu-id="5fad6-211">Response</span></span>
<span data-ttu-id="5fad6-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5fad6-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1188

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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



