---
title: 创建 managedIOSStoreApp
description: 创建新的 managedIOSStoreApp 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 33b7a336b5935041349556b06969e01936fcb1c1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39936526"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="95407-103">创建 managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="95407-103">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="95407-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95407-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95407-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95407-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95407-106">创建新的 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="95407-106">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95407-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="95407-107">Prerequisites</span></span>
<span data-ttu-id="95407-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95407-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95407-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="95407-110">Permission type</span></span>|<span data-ttu-id="95407-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="95407-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95407-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95407-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95407-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95407-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="95407-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95407-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95407-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="95407-115">Not supported.</span></span>|
|<span data-ttu-id="95407-116">Application</span><span class="sxs-lookup"><span data-stu-id="95407-116">Application</span></span>|<span data-ttu-id="95407-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95407-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95407-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95407-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="95407-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="95407-119">Request headers</span></span>
|<span data-ttu-id="95407-120">标头</span><span class="sxs-lookup"><span data-stu-id="95407-120">Header</span></span>|<span data-ttu-id="95407-121">值</span><span class="sxs-lookup"><span data-stu-id="95407-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95407-122">授权</span><span class="sxs-lookup"><span data-stu-id="95407-122">Authorization</span></span>|<span data-ttu-id="95407-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="95407-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95407-124">接受</span><span class="sxs-lookup"><span data-stu-id="95407-124">Accept</span></span>|<span data-ttu-id="95407-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95407-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95407-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="95407-126">Request body</span></span>
<span data-ttu-id="95407-127">在请求正文中，提供 managedIOSStoreApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95407-127">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="95407-128">下表显示创建 managedIOSStoreApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="95407-128">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="95407-129">属性</span><span class="sxs-lookup"><span data-stu-id="95407-129">Property</span></span>|<span data-ttu-id="95407-130">类型</span><span class="sxs-lookup"><span data-stu-id="95407-130">Type</span></span>|<span data-ttu-id="95407-131">说明</span><span class="sxs-lookup"><span data-stu-id="95407-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95407-132">id</span><span class="sxs-lookup"><span data-stu-id="95407-132">id</span></span>|<span data-ttu-id="95407-133">字符串</span><span class="sxs-lookup"><span data-stu-id="95407-133">String</span></span>|<span data-ttu-id="95407-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="95407-134">Key of the entity.</span></span> <span data-ttu-id="95407-135">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95407-136">displayName</span><span class="sxs-lookup"><span data-stu-id="95407-136">displayName</span></span>|<span data-ttu-id="95407-137">字符串</span><span class="sxs-lookup"><span data-stu-id="95407-137">String</span></span>|<span data-ttu-id="95407-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="95407-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="95407-139">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95407-140">说明</span><span class="sxs-lookup"><span data-stu-id="95407-140">description</span></span>|<span data-ttu-id="95407-141">字符串</span><span class="sxs-lookup"><span data-stu-id="95407-141">String</span></span>|<span data-ttu-id="95407-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="95407-142">The description of the app.</span></span> <span data-ttu-id="95407-143">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95407-144">publisher</span><span class="sxs-lookup"><span data-stu-id="95407-144">publisher</span></span>|<span data-ttu-id="95407-145">字符串</span><span class="sxs-lookup"><span data-stu-id="95407-145">String</span></span>|<span data-ttu-id="95407-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="95407-146">The publisher of the app.</span></span> <span data-ttu-id="95407-147">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95407-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="95407-148">largeIcon</span></span>|[<span data-ttu-id="95407-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="95407-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="95407-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="95407-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="95407-151">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95407-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95407-152">createdDateTime</span></span>|<span data-ttu-id="95407-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95407-153">DateTimeOffset</span></span>|<span data-ttu-id="95407-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="95407-154">The date and time the app was created.</span></span> <span data-ttu-id="95407-155">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95407-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95407-156">lastModifiedDateTime</span></span>|<span data-ttu-id="95407-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95407-157">DateTimeOffset</span></span>|<span data-ttu-id="95407-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="95407-158">The date and time the app was last modified.</span></span> <span data-ttu-id="95407-159">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95407-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="95407-160">isFeatured</span></span>|<span data-ttu-id="95407-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="95407-161">Boolean</span></span>|<span data-ttu-id="95407-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95407-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="95407-163">privacyInformationUrl</span></span>|<span data-ttu-id="95407-164">字符串</span><span class="sxs-lookup"><span data-stu-id="95407-164">String</span></span>|<span data-ttu-id="95407-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="95407-165">The privacy statement Url.</span></span> <span data-ttu-id="95407-166">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95407-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="95407-167">informationUrl</span></span>|<span data-ttu-id="95407-168">字符串</span><span class="sxs-lookup"><span data-stu-id="95407-168">String</span></span>|<span data-ttu-id="95407-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="95407-169">The more information Url.</span></span> <span data-ttu-id="95407-170">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95407-171">owner</span><span class="sxs-lookup"><span data-stu-id="95407-171">owner</span></span>|<span data-ttu-id="95407-172">String</span><span class="sxs-lookup"><span data-stu-id="95407-172">String</span></span>|<span data-ttu-id="95407-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="95407-173">The owner of the app.</span></span> <span data-ttu-id="95407-174">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95407-175">developer</span><span class="sxs-lookup"><span data-stu-id="95407-175">developer</span></span>|<span data-ttu-id="95407-176">字符串</span><span class="sxs-lookup"><span data-stu-id="95407-176">String</span></span>|<span data-ttu-id="95407-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="95407-177">The developer of the app.</span></span> <span data-ttu-id="95407-178">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95407-179">notes</span><span class="sxs-lookup"><span data-stu-id="95407-179">notes</span></span>|<span data-ttu-id="95407-180">字符串</span><span class="sxs-lookup"><span data-stu-id="95407-180">String</span></span>|<span data-ttu-id="95407-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="95407-181">Notes for the app.</span></span> <span data-ttu-id="95407-182">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95407-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="95407-183">uploadState</span></span>|<span data-ttu-id="95407-184">Int32</span><span class="sxs-lookup"><span data-stu-id="95407-184">Int32</span></span>|<span data-ttu-id="95407-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="95407-185">The upload state.</span></span> <span data-ttu-id="95407-186">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95407-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="95407-187">publishingState</span></span>|[<span data-ttu-id="95407-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="95407-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="95407-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="95407-189">The publishing state for the app.</span></span> <span data-ttu-id="95407-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="95407-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="95407-191">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="95407-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="95407-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="95407-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="95407-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="95407-193">isAssigned</span></span>|<span data-ttu-id="95407-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="95407-194">Boolean</span></span>|<span data-ttu-id="95407-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="95407-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="95407-196">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95407-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95407-197">roleScopeTagIds</span></span>|<span data-ttu-id="95407-198">String collection</span><span class="sxs-lookup"><span data-stu-id="95407-198">String collection</span></span>|<span data-ttu-id="95407-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="95407-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="95407-200">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95407-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="95407-201">dependentAppCount</span></span>|<span data-ttu-id="95407-202">Int32</span><span class="sxs-lookup"><span data-stu-id="95407-202">Int32</span></span>|<span data-ttu-id="95407-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="95407-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="95407-204">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95407-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="95407-205">appAvailability</span></span>|[<span data-ttu-id="95407-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="95407-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="95407-207">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="95407-207">The Application's availability.</span></span> <span data-ttu-id="95407-208">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="95407-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="95407-209">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="95407-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="95407-210">version</span><span class="sxs-lookup"><span data-stu-id="95407-210">version</span></span>|<span data-ttu-id="95407-211">String</span><span class="sxs-lookup"><span data-stu-id="95407-211">String</span></span>|<span data-ttu-id="95407-212">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="95407-212">The Application's version.</span></span> <span data-ttu-id="95407-213">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="95407-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="95407-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="95407-214">bundleId</span></span>|<span data-ttu-id="95407-215">字符串</span><span class="sxs-lookup"><span data-stu-id="95407-215">String</span></span>|<span data-ttu-id="95407-216">应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="95407-216">The app's Bundle ID.</span></span>|
|<span data-ttu-id="95407-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="95407-217">appStoreUrl</span></span>|<span data-ttu-id="95407-218">String</span><span class="sxs-lookup"><span data-stu-id="95407-218">String</span></span>|<span data-ttu-id="95407-219">Apple AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="95407-219">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="95407-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="95407-220">applicableDeviceType</span></span>|[<span data-ttu-id="95407-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="95407-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="95407-222">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="95407-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="95407-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="95407-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="95407-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="95407-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="95407-225">最低受支持操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="95407-225">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="95407-226">响应</span><span class="sxs-lookup"><span data-stu-id="95407-226">Response</span></span>
<span data-ttu-id="95407-227">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="95407-227">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95407-228">示例</span><span class="sxs-lookup"><span data-stu-id="95407-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="95407-229">请求</span><span class="sxs-lookup"><span data-stu-id="95407-229">Request</span></span>
<span data-ttu-id="95407-230">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="95407-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1238

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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
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

### <a name="response"></a><span data-ttu-id="95407-231">响应</span><span class="sxs-lookup"><span data-stu-id="95407-231">Response</span></span>
<span data-ttu-id="95407-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="95407-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1410

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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
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





