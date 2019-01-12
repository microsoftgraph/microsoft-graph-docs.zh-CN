---
title: 更新 managedIOSStoreApp
description: 更新 managedIOSStoreApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 75ee18a47c693c9099ccd18fb0b5434353c85397
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923367"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="415c8-103">更新 managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="415c8-103">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="415c8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="415c8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="415c8-105">更新 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="415c8-105">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="415c8-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="415c8-106">Prerequisites</span></span>
<span data-ttu-id="415c8-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="415c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="415c8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="415c8-109">Permission type</span></span>|<span data-ttu-id="415c8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="415c8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="415c8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="415c8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="415c8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="415c8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="415c8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="415c8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="415c8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="415c8-114">Not supported.</span></span>|
|<span data-ttu-id="415c8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="415c8-115">Application</span></span>|<span data-ttu-id="415c8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="415c8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="415c8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="415c8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="415c8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="415c8-118">Request headers</span></span>
|<span data-ttu-id="415c8-119">标头</span><span class="sxs-lookup"><span data-stu-id="415c8-119">Header</span></span>|<span data-ttu-id="415c8-120">值</span><span class="sxs-lookup"><span data-stu-id="415c8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="415c8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="415c8-121">Authorization</span></span>|<span data-ttu-id="415c8-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="415c8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="415c8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="415c8-123">Accept</span></span>|<span data-ttu-id="415c8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="415c8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="415c8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="415c8-125">Request body</span></span>
<span data-ttu-id="415c8-126">在请求正文中，提供 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="415c8-126">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="415c8-127">下表显示创建 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="415c8-127">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="415c8-128">属性</span><span class="sxs-lookup"><span data-stu-id="415c8-128">Property</span></span>|<span data-ttu-id="415c8-129">类型</span><span class="sxs-lookup"><span data-stu-id="415c8-129">Type</span></span>|<span data-ttu-id="415c8-130">说明</span><span class="sxs-lookup"><span data-stu-id="415c8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="415c8-131">id</span><span class="sxs-lookup"><span data-stu-id="415c8-131">id</span></span>|<span data-ttu-id="415c8-132">String</span><span class="sxs-lookup"><span data-stu-id="415c8-132">String</span></span>|<span data-ttu-id="415c8-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="415c8-133">Key of the entity.</span></span> <span data-ttu-id="415c8-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="415c8-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="415c8-135">displayName</span><span class="sxs-lookup"><span data-stu-id="415c8-135">displayName</span></span>|<span data-ttu-id="415c8-136">String</span><span class="sxs-lookup"><span data-stu-id="415c8-136">String</span></span>|<span data-ttu-id="415c8-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="415c8-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="415c8-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="415c8-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="415c8-139">description</span><span class="sxs-lookup"><span data-stu-id="415c8-139">description</span></span>|<span data-ttu-id="415c8-140">String</span><span class="sxs-lookup"><span data-stu-id="415c8-140">String</span></span>|<span data-ttu-id="415c8-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="415c8-141">The description of the app.</span></span> <span data-ttu-id="415c8-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="415c8-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="415c8-143">publisher</span><span class="sxs-lookup"><span data-stu-id="415c8-143">publisher</span></span>|<span data-ttu-id="415c8-144">String</span><span class="sxs-lookup"><span data-stu-id="415c8-144">String</span></span>|<span data-ttu-id="415c8-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="415c8-145">The publisher of the app.</span></span> <span data-ttu-id="415c8-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="415c8-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="415c8-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="415c8-147">largeIcon</span></span>|[<span data-ttu-id="415c8-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="415c8-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="415c8-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="415c8-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="415c8-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="415c8-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="415c8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="415c8-151">createdDateTime</span></span>|<span data-ttu-id="415c8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="415c8-152">DateTimeOffset</span></span>|<span data-ttu-id="415c8-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="415c8-153">The date and time the app was created.</span></span> <span data-ttu-id="415c8-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="415c8-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="415c8-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="415c8-155">lastModifiedDateTime</span></span>|<span data-ttu-id="415c8-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="415c8-156">DateTimeOffset</span></span>|<span data-ttu-id="415c8-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="415c8-157">The date and time the app was last modified.</span></span> <span data-ttu-id="415c8-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="415c8-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="415c8-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="415c8-159">isFeatured</span></span>|<span data-ttu-id="415c8-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="415c8-160">Boolean</span></span>|<span data-ttu-id="415c8-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="415c8-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="415c8-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="415c8-162">privacyInformationUrl</span></span>|<span data-ttu-id="415c8-163">String</span><span class="sxs-lookup"><span data-stu-id="415c8-163">String</span></span>|<span data-ttu-id="415c8-164">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="415c8-164">The privacy statement Url.</span></span> <span data-ttu-id="415c8-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="415c8-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="415c8-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="415c8-166">informationUrl</span></span>|<span data-ttu-id="415c8-167">String</span><span class="sxs-lookup"><span data-stu-id="415c8-167">String</span></span>|<span data-ttu-id="415c8-168">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="415c8-168">The more information Url.</span></span> <span data-ttu-id="415c8-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="415c8-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="415c8-170">owner</span><span class="sxs-lookup"><span data-stu-id="415c8-170">owner</span></span>|<span data-ttu-id="415c8-171">String</span><span class="sxs-lookup"><span data-stu-id="415c8-171">String</span></span>|<span data-ttu-id="415c8-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="415c8-172">The owner of the app.</span></span> <span data-ttu-id="415c8-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="415c8-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="415c8-174">developer</span><span class="sxs-lookup"><span data-stu-id="415c8-174">developer</span></span>|<span data-ttu-id="415c8-175">String</span><span class="sxs-lookup"><span data-stu-id="415c8-175">String</span></span>|<span data-ttu-id="415c8-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="415c8-176">The developer of the app.</span></span> <span data-ttu-id="415c8-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="415c8-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="415c8-178">notes</span><span class="sxs-lookup"><span data-stu-id="415c8-178">notes</span></span>|<span data-ttu-id="415c8-179">String</span><span class="sxs-lookup"><span data-stu-id="415c8-179">String</span></span>|<span data-ttu-id="415c8-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="415c8-180">Notes for the app.</span></span> <span data-ttu-id="415c8-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="415c8-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="415c8-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="415c8-182">publishingState</span></span>|[<span data-ttu-id="415c8-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="415c8-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="415c8-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="415c8-184">The publishing state for the app.</span></span> <span data-ttu-id="415c8-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="415c8-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="415c8-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="415c8-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="415c8-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="415c8-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="415c8-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="415c8-188">appAvailability</span></span>|[<span data-ttu-id="415c8-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="415c8-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="415c8-190">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="415c8-190">The Application's availability.</span></span> <span data-ttu-id="415c8-191">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="415c8-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="415c8-192">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="415c8-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="415c8-193">version</span><span class="sxs-lookup"><span data-stu-id="415c8-193">version</span></span>|<span data-ttu-id="415c8-194">String</span><span class="sxs-lookup"><span data-stu-id="415c8-194">String</span></span>|<span data-ttu-id="415c8-195">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="415c8-195">The Application's version.</span></span> <span data-ttu-id="415c8-196">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="415c8-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="415c8-197">bundleId</span><span class="sxs-lookup"><span data-stu-id="415c8-197">bundleId</span></span>|<span data-ttu-id="415c8-198">String</span><span class="sxs-lookup"><span data-stu-id="415c8-198">String</span></span>|<span data-ttu-id="415c8-199">应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="415c8-199">The app's Bundle ID.</span></span>|
|<span data-ttu-id="415c8-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="415c8-200">appStoreUrl</span></span>|<span data-ttu-id="415c8-201">String</span><span class="sxs-lookup"><span data-stu-id="415c8-201">String</span></span>|<span data-ttu-id="415c8-202">Apple AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="415c8-202">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="415c8-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="415c8-203">applicableDeviceType</span></span>|[<span data-ttu-id="415c8-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="415c8-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="415c8-205">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="415c8-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="415c8-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="415c8-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="415c8-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="415c8-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="415c8-208">最低受支持操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="415c8-208">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="415c8-209">响应</span><span class="sxs-lookup"><span data-stu-id="415c8-209">Response</span></span>
<span data-ttu-id="415c8-210">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="415c8-210">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="415c8-211">示例</span><span class="sxs-lookup"><span data-stu-id="415c8-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="415c8-212">请求</span><span class="sxs-lookup"><span data-stu-id="415c8-212">Request</span></span>
<span data-ttu-id="415c8-213">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="415c8-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1084

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="415c8-214">响应</span><span class="sxs-lookup"><span data-stu-id="415c8-214">Response</span></span>
<span data-ttu-id="415c8-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="415c8-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1256

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```



