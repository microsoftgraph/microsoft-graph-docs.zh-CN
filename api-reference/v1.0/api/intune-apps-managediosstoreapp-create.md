---
title: 创建 managedIOSStoreApp
description: 创建新的 managedIOSStoreApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7f8d2748e3ea1c2b57a7e9906ae8d3bea11dcfec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997457"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="51bfa-103">创建 managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="51bfa-103">Create managedIOSStoreApp</span></span>

<span data-ttu-id="51bfa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51bfa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51bfa-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51bfa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51bfa-106">创建新的 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51bfa-106">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51bfa-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="51bfa-107">Prerequisites</span></span>
<span data-ttu-id="51bfa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="51bfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="51bfa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="51bfa-110">Permission type</span></span>|<span data-ttu-id="51bfa-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="51bfa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51bfa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51bfa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51bfa-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51bfa-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="51bfa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51bfa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51bfa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="51bfa-115">Not supported.</span></span>|
|<span data-ttu-id="51bfa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="51bfa-116">Application</span></span>|<span data-ttu-id="51bfa-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51bfa-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51bfa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51bfa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="51bfa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="51bfa-119">Request headers</span></span>
|<span data-ttu-id="51bfa-120">标头</span><span class="sxs-lookup"><span data-stu-id="51bfa-120">Header</span></span>|<span data-ttu-id="51bfa-121">值</span><span class="sxs-lookup"><span data-stu-id="51bfa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51bfa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="51bfa-122">Authorization</span></span>|<span data-ttu-id="51bfa-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="51bfa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51bfa-124">接受</span><span class="sxs-lookup"><span data-stu-id="51bfa-124">Accept</span></span>|<span data-ttu-id="51bfa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="51bfa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51bfa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="51bfa-126">Request body</span></span>
<span data-ttu-id="51bfa-127">在请求正文中，提供 managedIOSStoreApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51bfa-127">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="51bfa-128">下表显示创建 managedIOSStoreApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="51bfa-128">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="51bfa-129">属性</span><span class="sxs-lookup"><span data-stu-id="51bfa-129">Property</span></span>|<span data-ttu-id="51bfa-130">类型</span><span class="sxs-lookup"><span data-stu-id="51bfa-130">Type</span></span>|<span data-ttu-id="51bfa-131">说明</span><span class="sxs-lookup"><span data-stu-id="51bfa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51bfa-132">id</span><span class="sxs-lookup"><span data-stu-id="51bfa-132">id</span></span>|<span data-ttu-id="51bfa-133">String</span><span class="sxs-lookup"><span data-stu-id="51bfa-133">String</span></span>|<span data-ttu-id="51bfa-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="51bfa-134">Key of the entity.</span></span> <span data-ttu-id="51bfa-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51bfa-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51bfa-136">displayName</span><span class="sxs-lookup"><span data-stu-id="51bfa-136">displayName</span></span>|<span data-ttu-id="51bfa-137">String</span><span class="sxs-lookup"><span data-stu-id="51bfa-137">String</span></span>|<span data-ttu-id="51bfa-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="51bfa-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="51bfa-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51bfa-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51bfa-140">description</span><span class="sxs-lookup"><span data-stu-id="51bfa-140">description</span></span>|<span data-ttu-id="51bfa-141">String</span><span class="sxs-lookup"><span data-stu-id="51bfa-141">String</span></span>|<span data-ttu-id="51bfa-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="51bfa-142">The description of the app.</span></span> <span data-ttu-id="51bfa-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51bfa-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51bfa-144">publisher</span><span class="sxs-lookup"><span data-stu-id="51bfa-144">publisher</span></span>|<span data-ttu-id="51bfa-145">String</span><span class="sxs-lookup"><span data-stu-id="51bfa-145">String</span></span>|<span data-ttu-id="51bfa-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="51bfa-146">The publisher of the app.</span></span> <span data-ttu-id="51bfa-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51bfa-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51bfa-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="51bfa-148">largeIcon</span></span>|[<span data-ttu-id="51bfa-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="51bfa-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="51bfa-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="51bfa-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="51bfa-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51bfa-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51bfa-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51bfa-152">createdDateTime</span></span>|<span data-ttu-id="51bfa-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51bfa-153">DateTimeOffset</span></span>|<span data-ttu-id="51bfa-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="51bfa-154">The date and time the app was created.</span></span> <span data-ttu-id="51bfa-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51bfa-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51bfa-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51bfa-156">lastModifiedDateTime</span></span>|<span data-ttu-id="51bfa-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51bfa-157">DateTimeOffset</span></span>|<span data-ttu-id="51bfa-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="51bfa-158">The date and time the app was last modified.</span></span> <span data-ttu-id="51bfa-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51bfa-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51bfa-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="51bfa-160">isFeatured</span></span>|<span data-ttu-id="51bfa-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="51bfa-161">Boolean</span></span>|<span data-ttu-id="51bfa-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51bfa-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51bfa-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="51bfa-163">privacyInformationUrl</span></span>|<span data-ttu-id="51bfa-164">String</span><span class="sxs-lookup"><span data-stu-id="51bfa-164">String</span></span>|<span data-ttu-id="51bfa-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="51bfa-165">The privacy statement Url.</span></span> <span data-ttu-id="51bfa-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51bfa-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51bfa-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="51bfa-167">informationUrl</span></span>|<span data-ttu-id="51bfa-168">String</span><span class="sxs-lookup"><span data-stu-id="51bfa-168">String</span></span>|<span data-ttu-id="51bfa-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="51bfa-169">The more information Url.</span></span> <span data-ttu-id="51bfa-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51bfa-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51bfa-171">所有者</span><span class="sxs-lookup"><span data-stu-id="51bfa-171">owner</span></span>|<span data-ttu-id="51bfa-172">String</span><span class="sxs-lookup"><span data-stu-id="51bfa-172">String</span></span>|<span data-ttu-id="51bfa-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="51bfa-173">The owner of the app.</span></span> <span data-ttu-id="51bfa-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51bfa-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51bfa-175">developer</span><span class="sxs-lookup"><span data-stu-id="51bfa-175">developer</span></span>|<span data-ttu-id="51bfa-176">String</span><span class="sxs-lookup"><span data-stu-id="51bfa-176">String</span></span>|<span data-ttu-id="51bfa-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="51bfa-177">The developer of the app.</span></span> <span data-ttu-id="51bfa-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51bfa-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51bfa-179">notes</span><span class="sxs-lookup"><span data-stu-id="51bfa-179">notes</span></span>|<span data-ttu-id="51bfa-180">String</span><span class="sxs-lookup"><span data-stu-id="51bfa-180">String</span></span>|<span data-ttu-id="51bfa-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="51bfa-181">Notes for the app.</span></span> <span data-ttu-id="51bfa-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51bfa-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51bfa-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="51bfa-183">publishingState</span></span>|[<span data-ttu-id="51bfa-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="51bfa-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="51bfa-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="51bfa-185">The publishing state for the app.</span></span> <span data-ttu-id="51bfa-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="51bfa-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="51bfa-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="51bfa-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="51bfa-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="51bfa-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="51bfa-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="51bfa-189">appAvailability</span></span>|[<span data-ttu-id="51bfa-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="51bfa-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="51bfa-191">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="51bfa-191">The Application's availability.</span></span> <span data-ttu-id="51bfa-192">继承自 [managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="51bfa-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="51bfa-193">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="51bfa-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="51bfa-194">version</span><span class="sxs-lookup"><span data-stu-id="51bfa-194">version</span></span>|<span data-ttu-id="51bfa-195">String</span><span class="sxs-lookup"><span data-stu-id="51bfa-195">String</span></span>|<span data-ttu-id="51bfa-196">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="51bfa-196">The Application's version.</span></span> <span data-ttu-id="51bfa-197">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="51bfa-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="51bfa-198">bundleId</span><span class="sxs-lookup"><span data-stu-id="51bfa-198">bundleId</span></span>|<span data-ttu-id="51bfa-199">String</span><span class="sxs-lookup"><span data-stu-id="51bfa-199">String</span></span>|<span data-ttu-id="51bfa-200">应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="51bfa-200">The app's Bundle ID.</span></span>|
|<span data-ttu-id="51bfa-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="51bfa-201">appStoreUrl</span></span>|<span data-ttu-id="51bfa-202">String</span><span class="sxs-lookup"><span data-stu-id="51bfa-202">String</span></span>|<span data-ttu-id="51bfa-203">Apple AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="51bfa-203">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="51bfa-204">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="51bfa-204">applicableDeviceType</span></span>|[<span data-ttu-id="51bfa-205">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="51bfa-205">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="51bfa-206">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="51bfa-206">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="51bfa-207">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="51bfa-207">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="51bfa-208">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="51bfa-208">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="51bfa-209">最低受支持操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="51bfa-209">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="51bfa-210">响应</span><span class="sxs-lookup"><span data-stu-id="51bfa-210">Response</span></span>
<span data-ttu-id="51bfa-211">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51bfa-211">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51bfa-212">示例</span><span class="sxs-lookup"><span data-stu-id="51bfa-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="51bfa-213">请求</span><span class="sxs-lookup"><span data-stu-id="51bfa-213">Request</span></span>
<span data-ttu-id="51bfa-214">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="51bfa-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1104

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
    "v12_0": true,
    "v13_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="51bfa-215">响应</span><span class="sxs-lookup"><span data-stu-id="51bfa-215">Response</span></span>
<span data-ttu-id="51bfa-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="51bfa-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1276

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
    "v12_0": true,
    "v13_0": true
  }
}
```









