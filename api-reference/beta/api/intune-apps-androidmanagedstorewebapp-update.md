---
title: 更新 androidManagedStoreWebApp
description: 更新 androidManagedStoreWebApp 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a31e4e0d2279f9cbd01446bbc9436f83774b4c9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762196"
---
# <a name="update-androidmanagedstorewebapp"></a><span data-ttu-id="4222d-103">更新 androidManagedStoreWebApp</span><span class="sxs-lookup"><span data-stu-id="4222d-103">Update androidManagedStoreWebApp</span></span>

> <span data-ttu-id="4222d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4222d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4222d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4222d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4222d-106">更新[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4222d-106">Update the properties of a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4222d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4222d-107">Prerequisites</span></span>
<span data-ttu-id="4222d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4222d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4222d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4222d-110">Permission type</span></span>|<span data-ttu-id="4222d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4222d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4222d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4222d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4222d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4222d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4222d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4222d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4222d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4222d-115">Not supported.</span></span>|
|<span data-ttu-id="4222d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4222d-116">Application</span></span>|<span data-ttu-id="4222d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4222d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4222d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4222d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4222d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4222d-119">Request headers</span></span>
|<span data-ttu-id="4222d-120">标头</span><span class="sxs-lookup"><span data-stu-id="4222d-120">Header</span></span>|<span data-ttu-id="4222d-121">值</span><span class="sxs-lookup"><span data-stu-id="4222d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4222d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4222d-122">Authorization</span></span>|<span data-ttu-id="4222d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4222d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4222d-124">接受</span><span class="sxs-lookup"><span data-stu-id="4222d-124">Accept</span></span>|<span data-ttu-id="4222d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4222d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4222d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4222d-126">Request body</span></span>
<span data-ttu-id="4222d-127">在请求正文中，提供[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4222d-127">In the request body, supply a JSON representation for the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

<span data-ttu-id="4222d-128">下表显示创建[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4222d-128">The following table shows the properties that are required when you create the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).</span></span>

|<span data-ttu-id="4222d-129">属性</span><span class="sxs-lookup"><span data-stu-id="4222d-129">Property</span></span>|<span data-ttu-id="4222d-130">类型</span><span class="sxs-lookup"><span data-stu-id="4222d-130">Type</span></span>|<span data-ttu-id="4222d-131">说明</span><span class="sxs-lookup"><span data-stu-id="4222d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4222d-132">id</span><span class="sxs-lookup"><span data-stu-id="4222d-132">id</span></span>|<span data-ttu-id="4222d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4222d-133">String</span></span>|<span data-ttu-id="4222d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4222d-134">Key of the entity.</span></span> <span data-ttu-id="4222d-135">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4222d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4222d-136">displayName</span></span>|<span data-ttu-id="4222d-137">String</span><span class="sxs-lookup"><span data-stu-id="4222d-137">String</span></span>|<span data-ttu-id="4222d-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="4222d-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4222d-139">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4222d-140">说明</span><span class="sxs-lookup"><span data-stu-id="4222d-140">description</span></span>|<span data-ttu-id="4222d-141">字符串</span><span class="sxs-lookup"><span data-stu-id="4222d-141">String</span></span>|<span data-ttu-id="4222d-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="4222d-142">The description of the app.</span></span> <span data-ttu-id="4222d-143">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4222d-144">publisher</span><span class="sxs-lookup"><span data-stu-id="4222d-144">publisher</span></span>|<span data-ttu-id="4222d-145">String</span><span class="sxs-lookup"><span data-stu-id="4222d-145">String</span></span>|<span data-ttu-id="4222d-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="4222d-146">The publisher of the app.</span></span> <span data-ttu-id="4222d-147">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4222d-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4222d-148">largeIcon</span></span>|[<span data-ttu-id="4222d-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4222d-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4222d-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="4222d-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4222d-151">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4222d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4222d-152">createdDateTime</span></span>|<span data-ttu-id="4222d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4222d-153">DateTimeOffset</span></span>|<span data-ttu-id="4222d-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4222d-154">The date and time the app was created.</span></span> <span data-ttu-id="4222d-155">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4222d-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4222d-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4222d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4222d-157">DateTimeOffset</span></span>|<span data-ttu-id="4222d-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4222d-158">The date and time the app was last modified.</span></span> <span data-ttu-id="4222d-159">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4222d-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4222d-160">isFeatured</span></span>|<span data-ttu-id="4222d-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4222d-161">Boolean</span></span>|<span data-ttu-id="4222d-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4222d-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4222d-163">privacyInformationUrl</span></span>|<span data-ttu-id="4222d-164">String</span><span class="sxs-lookup"><span data-stu-id="4222d-164">String</span></span>|<span data-ttu-id="4222d-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="4222d-165">The privacy statement Url.</span></span> <span data-ttu-id="4222d-166">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4222d-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4222d-167">informationUrl</span></span>|<span data-ttu-id="4222d-168">String</span><span class="sxs-lookup"><span data-stu-id="4222d-168">String</span></span>|<span data-ttu-id="4222d-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="4222d-169">The more information Url.</span></span> <span data-ttu-id="4222d-170">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4222d-171">owner</span><span class="sxs-lookup"><span data-stu-id="4222d-171">owner</span></span>|<span data-ttu-id="4222d-172">String</span><span class="sxs-lookup"><span data-stu-id="4222d-172">String</span></span>|<span data-ttu-id="4222d-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="4222d-173">The owner of the app.</span></span> <span data-ttu-id="4222d-174">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4222d-175">developer</span><span class="sxs-lookup"><span data-stu-id="4222d-175">developer</span></span>|<span data-ttu-id="4222d-176">String</span><span class="sxs-lookup"><span data-stu-id="4222d-176">String</span></span>|<span data-ttu-id="4222d-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="4222d-177">The developer of the app.</span></span> <span data-ttu-id="4222d-178">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4222d-179">notes</span><span class="sxs-lookup"><span data-stu-id="4222d-179">notes</span></span>|<span data-ttu-id="4222d-180">String</span><span class="sxs-lookup"><span data-stu-id="4222d-180">String</span></span>|<span data-ttu-id="4222d-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="4222d-181">Notes for the app.</span></span> <span data-ttu-id="4222d-182">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4222d-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="4222d-183">uploadState</span></span>|<span data-ttu-id="4222d-184">Int32</span><span class="sxs-lookup"><span data-stu-id="4222d-184">Int32</span></span>|<span data-ttu-id="4222d-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="4222d-185">The upload state.</span></span> <span data-ttu-id="4222d-186">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4222d-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="4222d-187">publishingState</span></span>|[<span data-ttu-id="4222d-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4222d-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4222d-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="4222d-189">The publishing state for the app.</span></span> <span data-ttu-id="4222d-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="4222d-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4222d-191">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="4222d-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="4222d-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="4222d-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4222d-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4222d-193">isAssigned</span></span>|<span data-ttu-id="4222d-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4222d-194">Boolean</span></span>|<span data-ttu-id="4222d-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="4222d-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4222d-196">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4222d-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4222d-197">roleScopeTagIds</span></span>|<span data-ttu-id="4222d-198">String collection</span><span class="sxs-lookup"><span data-stu-id="4222d-198">String collection</span></span>|<span data-ttu-id="4222d-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="4222d-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4222d-200">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4222d-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="4222d-201">dependentAppCount</span></span>|<span data-ttu-id="4222d-202">Int32</span><span class="sxs-lookup"><span data-stu-id="4222d-202">Int32</span></span>|<span data-ttu-id="4222d-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="4222d-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4222d-204">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4222d-205">packageId</span><span class="sxs-lookup"><span data-stu-id="4222d-205">packageId</span></span>|<span data-ttu-id="4222d-206">String</span><span class="sxs-lookup"><span data-stu-id="4222d-206">String</span></span>|<span data-ttu-id="4222d-207">包标识符。</span><span class="sxs-lookup"><span data-stu-id="4222d-207">The package identifier.</span></span> <span data-ttu-id="4222d-208">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-208">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="4222d-209">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="4222d-209">appIdentifier</span></span>|<span data-ttu-id="4222d-210">String</span><span class="sxs-lookup"><span data-stu-id="4222d-210">String</span></span>|<span data-ttu-id="4222d-211">标识名称。</span><span class="sxs-lookup"><span data-stu-id="4222d-211">The Identity Name.</span></span> <span data-ttu-id="4222d-212">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-212">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="4222d-213">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4222d-213">usedLicenseCount</span></span>|<span data-ttu-id="4222d-214">Int32</span><span class="sxs-lookup"><span data-stu-id="4222d-214">Int32</span></span>|<span data-ttu-id="4222d-215">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="4222d-215">The number of VPP licenses in use.</span></span> <span data-ttu-id="4222d-216">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-216">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="4222d-217">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4222d-217">totalLicenseCount</span></span>|<span data-ttu-id="4222d-218">Int32</span><span class="sxs-lookup"><span data-stu-id="4222d-218">Int32</span></span>|<span data-ttu-id="4222d-219">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="4222d-219">The total number of VPP licenses.</span></span> <span data-ttu-id="4222d-220">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-220">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="4222d-221">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4222d-221">appStoreUrl</span></span>|<span data-ttu-id="4222d-222">String</span><span class="sxs-lookup"><span data-stu-id="4222d-222">String</span></span>|<span data-ttu-id="4222d-223">"播放工作商店" 应用程序 URL。</span><span class="sxs-lookup"><span data-stu-id="4222d-223">The Play for Work Store app URL.</span></span> <span data-ttu-id="4222d-224">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-224">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="4222d-225">isPrivate</span><span class="sxs-lookup"><span data-stu-id="4222d-225">isPrivate</span></span>|<span data-ttu-id="4222d-226">布尔值</span><span class="sxs-lookup"><span data-stu-id="4222d-226">Boolean</span></span>|<span data-ttu-id="4222d-227">指示应用程序是否仅适用于给定企业的用户。</span><span class="sxs-lookup"><span data-stu-id="4222d-227">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="4222d-228">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-228">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="4222d-229">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="4222d-229">isSystemApp</span></span>|<span data-ttu-id="4222d-230">布尔值</span><span class="sxs-lookup"><span data-stu-id="4222d-230">Boolean</span></span>|<span data-ttu-id="4222d-231">指示应用程序是否为预安装的系统应用程序。</span><span class="sxs-lookup"><span data-stu-id="4222d-231">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="4222d-232">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-232">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="4222d-233">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="4222d-233">supportsOemConfig</span></span>|<span data-ttu-id="4222d-234">布尔值</span><span class="sxs-lookup"><span data-stu-id="4222d-234">Boolean</span></span>|<span data-ttu-id="4222d-235">此应用是否支持 OEMConfig 策略。</span><span class="sxs-lookup"><span data-stu-id="4222d-235">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="4222d-236">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="4222d-236">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4222d-237">响应</span><span class="sxs-lookup"><span data-stu-id="4222d-237">Response</span></span>
<span data-ttu-id="4222d-238">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4222d-238">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4222d-239">示例</span><span class="sxs-lookup"><span data-stu-id="4222d-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="4222d-240">请求</span><span class="sxs-lookup"><span data-stu-id="4222d-240">Request</span></span>
<span data-ttu-id="4222d-241">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4222d-241">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 987

{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="4222d-242">响应</span><span class="sxs-lookup"><span data-stu-id="4222d-242">Response</span></span>
<span data-ttu-id="4222d-p127">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4222d-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1159

{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
  "id": "e54aecbd-ecbd-e54a-bdec-4ae5bdec4ae5",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "supportsOemConfig": true
}
```




