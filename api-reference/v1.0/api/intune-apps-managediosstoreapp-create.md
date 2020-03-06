---
title: 创建 managedIOSStoreApp
description: 创建新的 managedIOSStoreApp 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 666b3f38d626180a2be1b2bb64088a5b50fb111b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516164"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="78f34-103">创建 managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="78f34-103">Create managedIOSStoreApp</span></span>

<span data-ttu-id="78f34-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78f34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78f34-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="78f34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78f34-106">创建新的 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78f34-106">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78f34-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="78f34-107">Prerequisites</span></span>
<span data-ttu-id="78f34-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="78f34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="78f34-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="78f34-110">Permission type</span></span>|<span data-ttu-id="78f34-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="78f34-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78f34-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78f34-112">Delegated (work or school account)</span></span>|<span data-ttu-id="78f34-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f34-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="78f34-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78f34-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78f34-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="78f34-115">Not supported.</span></span>|
|<span data-ttu-id="78f34-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="78f34-116">Application</span></span>|<span data-ttu-id="78f34-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f34-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78f34-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78f34-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="78f34-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="78f34-119">Request headers</span></span>
|<span data-ttu-id="78f34-120">标头</span><span class="sxs-lookup"><span data-stu-id="78f34-120">Header</span></span>|<span data-ttu-id="78f34-121">值</span><span class="sxs-lookup"><span data-stu-id="78f34-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78f34-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="78f34-122">Authorization</span></span>|<span data-ttu-id="78f34-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="78f34-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78f34-124">接受</span><span class="sxs-lookup"><span data-stu-id="78f34-124">Accept</span></span>|<span data-ttu-id="78f34-125">application/json</span><span class="sxs-lookup"><span data-stu-id="78f34-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78f34-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="78f34-126">Request body</span></span>
<span data-ttu-id="78f34-127">在请求正文中，提供 managedIOSStoreApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78f34-127">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="78f34-128">下表显示创建 managedIOSStoreApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="78f34-128">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="78f34-129">属性</span><span class="sxs-lookup"><span data-stu-id="78f34-129">Property</span></span>|<span data-ttu-id="78f34-130">类型</span><span class="sxs-lookup"><span data-stu-id="78f34-130">Type</span></span>|<span data-ttu-id="78f34-131">说明</span><span class="sxs-lookup"><span data-stu-id="78f34-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78f34-132">id</span><span class="sxs-lookup"><span data-stu-id="78f34-132">id</span></span>|<span data-ttu-id="78f34-133">字符串</span><span class="sxs-lookup"><span data-stu-id="78f34-133">String</span></span>|<span data-ttu-id="78f34-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="78f34-134">Key of the entity.</span></span> <span data-ttu-id="78f34-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78f34-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78f34-136">displayName</span><span class="sxs-lookup"><span data-stu-id="78f34-136">displayName</span></span>|<span data-ttu-id="78f34-137">字符串</span><span class="sxs-lookup"><span data-stu-id="78f34-137">String</span></span>|<span data-ttu-id="78f34-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="78f34-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="78f34-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78f34-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78f34-140">说明</span><span class="sxs-lookup"><span data-stu-id="78f34-140">description</span></span>|<span data-ttu-id="78f34-141">字符串</span><span class="sxs-lookup"><span data-stu-id="78f34-141">String</span></span>|<span data-ttu-id="78f34-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="78f34-142">The description of the app.</span></span> <span data-ttu-id="78f34-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78f34-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78f34-144">publisher</span><span class="sxs-lookup"><span data-stu-id="78f34-144">publisher</span></span>|<span data-ttu-id="78f34-145">字符串</span><span class="sxs-lookup"><span data-stu-id="78f34-145">String</span></span>|<span data-ttu-id="78f34-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="78f34-146">The publisher of the app.</span></span> <span data-ttu-id="78f34-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78f34-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78f34-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="78f34-148">largeIcon</span></span>|[<span data-ttu-id="78f34-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="78f34-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="78f34-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="78f34-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="78f34-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78f34-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78f34-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78f34-152">createdDateTime</span></span>|<span data-ttu-id="78f34-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78f34-153">DateTimeOffset</span></span>|<span data-ttu-id="78f34-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="78f34-154">The date and time the app was created.</span></span> <span data-ttu-id="78f34-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78f34-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78f34-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78f34-156">lastModifiedDateTime</span></span>|<span data-ttu-id="78f34-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78f34-157">DateTimeOffset</span></span>|<span data-ttu-id="78f34-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="78f34-158">The date and time the app was last modified.</span></span> <span data-ttu-id="78f34-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78f34-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78f34-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="78f34-160">isFeatured</span></span>|<span data-ttu-id="78f34-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="78f34-161">Boolean</span></span>|<span data-ttu-id="78f34-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78f34-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78f34-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="78f34-163">privacyInformationUrl</span></span>|<span data-ttu-id="78f34-164">字符串</span><span class="sxs-lookup"><span data-stu-id="78f34-164">String</span></span>|<span data-ttu-id="78f34-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="78f34-165">The privacy statement Url.</span></span> <span data-ttu-id="78f34-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78f34-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78f34-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="78f34-167">informationUrl</span></span>|<span data-ttu-id="78f34-168">字符串</span><span class="sxs-lookup"><span data-stu-id="78f34-168">String</span></span>|<span data-ttu-id="78f34-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="78f34-169">The more information Url.</span></span> <span data-ttu-id="78f34-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78f34-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78f34-171">owner</span><span class="sxs-lookup"><span data-stu-id="78f34-171">owner</span></span>|<span data-ttu-id="78f34-172">String</span><span class="sxs-lookup"><span data-stu-id="78f34-172">String</span></span>|<span data-ttu-id="78f34-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="78f34-173">The owner of the app.</span></span> <span data-ttu-id="78f34-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78f34-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78f34-175">developer</span><span class="sxs-lookup"><span data-stu-id="78f34-175">developer</span></span>|<span data-ttu-id="78f34-176">字符串</span><span class="sxs-lookup"><span data-stu-id="78f34-176">String</span></span>|<span data-ttu-id="78f34-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="78f34-177">The developer of the app.</span></span> <span data-ttu-id="78f34-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78f34-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78f34-179">notes</span><span class="sxs-lookup"><span data-stu-id="78f34-179">notes</span></span>|<span data-ttu-id="78f34-180">字符串</span><span class="sxs-lookup"><span data-stu-id="78f34-180">String</span></span>|<span data-ttu-id="78f34-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="78f34-181">Notes for the app.</span></span> <span data-ttu-id="78f34-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78f34-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78f34-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="78f34-183">publishingState</span></span>|[<span data-ttu-id="78f34-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="78f34-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="78f34-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="78f34-185">The publishing state for the app.</span></span> <span data-ttu-id="78f34-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="78f34-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="78f34-187">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="78f34-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="78f34-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="78f34-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="78f34-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="78f34-189">appAvailability</span></span>|[<span data-ttu-id="78f34-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="78f34-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="78f34-191">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="78f34-191">The Application's availability.</span></span> <span data-ttu-id="78f34-192">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="78f34-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="78f34-193">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="78f34-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="78f34-194">version</span><span class="sxs-lookup"><span data-stu-id="78f34-194">version</span></span>|<span data-ttu-id="78f34-195">String</span><span class="sxs-lookup"><span data-stu-id="78f34-195">String</span></span>|<span data-ttu-id="78f34-196">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="78f34-196">The Application's version.</span></span> <span data-ttu-id="78f34-197">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="78f34-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="78f34-198">bundleId</span><span class="sxs-lookup"><span data-stu-id="78f34-198">bundleId</span></span>|<span data-ttu-id="78f34-199">字符串</span><span class="sxs-lookup"><span data-stu-id="78f34-199">String</span></span>|<span data-ttu-id="78f34-200">应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="78f34-200">The app's Bundle ID.</span></span>|
|<span data-ttu-id="78f34-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="78f34-201">appStoreUrl</span></span>|<span data-ttu-id="78f34-202">String</span><span class="sxs-lookup"><span data-stu-id="78f34-202">String</span></span>|<span data-ttu-id="78f34-203">Apple AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="78f34-203">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="78f34-204">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="78f34-204">applicableDeviceType</span></span>|[<span data-ttu-id="78f34-205">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="78f34-205">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="78f34-206">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="78f34-206">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="78f34-207">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="78f34-207">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="78f34-208">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="78f34-208">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="78f34-209">最低受支持操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="78f34-209">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="78f34-210">响应</span><span class="sxs-lookup"><span data-stu-id="78f34-210">Response</span></span>
<span data-ttu-id="78f34-211">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78f34-211">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78f34-212">示例</span><span class="sxs-lookup"><span data-stu-id="78f34-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="78f34-213">请求</span><span class="sxs-lookup"><span data-stu-id="78f34-213">Request</span></span>
<span data-ttu-id="78f34-214">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="78f34-214">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="78f34-215">响应</span><span class="sxs-lookup"><span data-stu-id="78f34-215">Response</span></span>
<span data-ttu-id="78f34-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="78f34-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




