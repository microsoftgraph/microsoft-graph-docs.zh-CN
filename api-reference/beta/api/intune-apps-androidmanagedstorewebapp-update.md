---
title: 更新 androidManagedStoreWebApp
description: 更新 androidManagedStoreWebApp 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c2bf5c47ad9a30eb6d3b5c012981e3e56c0553f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445832"
---
# <a name="update-androidmanagedstorewebapp"></a><span data-ttu-id="67bc6-103">更新 androidManagedStoreWebApp</span><span class="sxs-lookup"><span data-stu-id="67bc6-103">Update androidManagedStoreWebApp</span></span>

<span data-ttu-id="67bc6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="67bc6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67bc6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="67bc6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67bc6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="67bc6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67bc6-107">更新[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="67bc6-107">Update the properties of a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67bc6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="67bc6-108">Prerequisites</span></span>
<span data-ttu-id="67bc6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67bc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67bc6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="67bc6-111">Permission type</span></span>|<span data-ttu-id="67bc6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="67bc6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67bc6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67bc6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67bc6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67bc6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="67bc6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67bc6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67bc6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="67bc6-116">Not supported.</span></span>|
|<span data-ttu-id="67bc6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="67bc6-117">Application</span></span>|<span data-ttu-id="67bc6-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67bc6-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67bc6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67bc6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="67bc6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="67bc6-120">Request headers</span></span>
|<span data-ttu-id="67bc6-121">标头</span><span class="sxs-lookup"><span data-stu-id="67bc6-121">Header</span></span>|<span data-ttu-id="67bc6-122">值</span><span class="sxs-lookup"><span data-stu-id="67bc6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67bc6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="67bc6-123">Authorization</span></span>|<span data-ttu-id="67bc6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="67bc6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67bc6-125">接受</span><span class="sxs-lookup"><span data-stu-id="67bc6-125">Accept</span></span>|<span data-ttu-id="67bc6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67bc6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67bc6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="67bc6-127">Request body</span></span>
<span data-ttu-id="67bc6-128">在请求正文中，提供[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67bc6-128">In the request body, supply a JSON representation for the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

<span data-ttu-id="67bc6-129">下表显示创建[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="67bc6-129">The following table shows the properties that are required when you create the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).</span></span>

|<span data-ttu-id="67bc6-130">属性</span><span class="sxs-lookup"><span data-stu-id="67bc6-130">Property</span></span>|<span data-ttu-id="67bc6-131">类型</span><span class="sxs-lookup"><span data-stu-id="67bc6-131">Type</span></span>|<span data-ttu-id="67bc6-132">说明</span><span class="sxs-lookup"><span data-stu-id="67bc6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67bc6-133">id</span><span class="sxs-lookup"><span data-stu-id="67bc6-133">id</span></span>|<span data-ttu-id="67bc6-134">字符串</span><span class="sxs-lookup"><span data-stu-id="67bc6-134">String</span></span>|<span data-ttu-id="67bc6-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="67bc6-135">Key of the entity.</span></span> <span data-ttu-id="67bc6-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="67bc6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="67bc6-137">displayName</span></span>|<span data-ttu-id="67bc6-138">String</span><span class="sxs-lookup"><span data-stu-id="67bc6-138">String</span></span>|<span data-ttu-id="67bc6-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="67bc6-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="67bc6-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="67bc6-141">说明</span><span class="sxs-lookup"><span data-stu-id="67bc6-141">description</span></span>|<span data-ttu-id="67bc6-142">字符串</span><span class="sxs-lookup"><span data-stu-id="67bc6-142">String</span></span>|<span data-ttu-id="67bc6-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="67bc6-143">The description of the app.</span></span> <span data-ttu-id="67bc6-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="67bc6-145">publisher</span><span class="sxs-lookup"><span data-stu-id="67bc6-145">publisher</span></span>|<span data-ttu-id="67bc6-146">String</span><span class="sxs-lookup"><span data-stu-id="67bc6-146">String</span></span>|<span data-ttu-id="67bc6-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="67bc6-147">The publisher of the app.</span></span> <span data-ttu-id="67bc6-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="67bc6-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="67bc6-149">largeIcon</span></span>|[<span data-ttu-id="67bc6-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="67bc6-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="67bc6-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="67bc6-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="67bc6-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="67bc6-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67bc6-153">createdDateTime</span></span>|<span data-ttu-id="67bc6-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67bc6-154">DateTimeOffset</span></span>|<span data-ttu-id="67bc6-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="67bc6-155">The date and time the app was created.</span></span> <span data-ttu-id="67bc6-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="67bc6-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67bc6-157">lastModifiedDateTime</span></span>|<span data-ttu-id="67bc6-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67bc6-158">DateTimeOffset</span></span>|<span data-ttu-id="67bc6-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="67bc6-159">The date and time the app was last modified.</span></span> <span data-ttu-id="67bc6-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="67bc6-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="67bc6-161">isFeatured</span></span>|<span data-ttu-id="67bc6-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="67bc6-162">Boolean</span></span>|<span data-ttu-id="67bc6-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="67bc6-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="67bc6-164">privacyInformationUrl</span></span>|<span data-ttu-id="67bc6-165">String</span><span class="sxs-lookup"><span data-stu-id="67bc6-165">String</span></span>|<span data-ttu-id="67bc6-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="67bc6-166">The privacy statement Url.</span></span> <span data-ttu-id="67bc6-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="67bc6-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="67bc6-168">informationUrl</span></span>|<span data-ttu-id="67bc6-169">String</span><span class="sxs-lookup"><span data-stu-id="67bc6-169">String</span></span>|<span data-ttu-id="67bc6-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="67bc6-170">The more information Url.</span></span> <span data-ttu-id="67bc6-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="67bc6-172">owner</span><span class="sxs-lookup"><span data-stu-id="67bc6-172">owner</span></span>|<span data-ttu-id="67bc6-173">String</span><span class="sxs-lookup"><span data-stu-id="67bc6-173">String</span></span>|<span data-ttu-id="67bc6-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="67bc6-174">The owner of the app.</span></span> <span data-ttu-id="67bc6-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="67bc6-176">developer</span><span class="sxs-lookup"><span data-stu-id="67bc6-176">developer</span></span>|<span data-ttu-id="67bc6-177">String</span><span class="sxs-lookup"><span data-stu-id="67bc6-177">String</span></span>|<span data-ttu-id="67bc6-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="67bc6-178">The developer of the app.</span></span> <span data-ttu-id="67bc6-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="67bc6-180">notes</span><span class="sxs-lookup"><span data-stu-id="67bc6-180">notes</span></span>|<span data-ttu-id="67bc6-181">String</span><span class="sxs-lookup"><span data-stu-id="67bc6-181">String</span></span>|<span data-ttu-id="67bc6-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="67bc6-182">Notes for the app.</span></span> <span data-ttu-id="67bc6-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="67bc6-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="67bc6-184">uploadState</span></span>|<span data-ttu-id="67bc6-185">Int32</span><span class="sxs-lookup"><span data-stu-id="67bc6-185">Int32</span></span>|<span data-ttu-id="67bc6-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="67bc6-186">The upload state.</span></span> <span data-ttu-id="67bc6-187">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="67bc6-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="67bc6-188">publishingState</span></span>|[<span data-ttu-id="67bc6-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="67bc6-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="67bc6-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="67bc6-190">The publishing state for the app.</span></span> <span data-ttu-id="67bc6-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="67bc6-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="67bc6-192">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="67bc6-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="67bc6-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="67bc6-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="67bc6-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="67bc6-194">isAssigned</span></span>|<span data-ttu-id="67bc6-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="67bc6-195">Boolean</span></span>|<span data-ttu-id="67bc6-196">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="67bc6-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="67bc6-197">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="67bc6-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="67bc6-198">roleScopeTagIds</span></span>|<span data-ttu-id="67bc6-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="67bc6-199">String collection</span></span>|<span data-ttu-id="67bc6-200">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="67bc6-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="67bc6-201">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="67bc6-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="67bc6-202">dependentAppCount</span></span>|<span data-ttu-id="67bc6-203">Int32</span><span class="sxs-lookup"><span data-stu-id="67bc6-203">Int32</span></span>|<span data-ttu-id="67bc6-204">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="67bc6-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="67bc6-205">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="67bc6-206">packageId</span><span class="sxs-lookup"><span data-stu-id="67bc6-206">packageId</span></span>|<span data-ttu-id="67bc6-207">String</span><span class="sxs-lookup"><span data-stu-id="67bc6-207">String</span></span>|<span data-ttu-id="67bc6-208">包标识符。</span><span class="sxs-lookup"><span data-stu-id="67bc6-208">The package identifier.</span></span> <span data-ttu-id="67bc6-209">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-209">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="67bc6-210">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="67bc6-210">appIdentifier</span></span>|<span data-ttu-id="67bc6-211">String</span><span class="sxs-lookup"><span data-stu-id="67bc6-211">String</span></span>|<span data-ttu-id="67bc6-212">标识名称。</span><span class="sxs-lookup"><span data-stu-id="67bc6-212">The Identity Name.</span></span> <span data-ttu-id="67bc6-213">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-213">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="67bc6-214">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="67bc6-214">usedLicenseCount</span></span>|<span data-ttu-id="67bc6-215">Int32</span><span class="sxs-lookup"><span data-stu-id="67bc6-215">Int32</span></span>|<span data-ttu-id="67bc6-216">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="67bc6-216">The number of VPP licenses in use.</span></span> <span data-ttu-id="67bc6-217">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-217">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="67bc6-218">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="67bc6-218">totalLicenseCount</span></span>|<span data-ttu-id="67bc6-219">Int32</span><span class="sxs-lookup"><span data-stu-id="67bc6-219">Int32</span></span>|<span data-ttu-id="67bc6-220">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="67bc6-220">The total number of VPP licenses.</span></span> <span data-ttu-id="67bc6-221">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-221">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="67bc6-222">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="67bc6-222">appStoreUrl</span></span>|<span data-ttu-id="67bc6-223">String</span><span class="sxs-lookup"><span data-stu-id="67bc6-223">String</span></span>|<span data-ttu-id="67bc6-224">"播放工作商店" 应用程序 URL。</span><span class="sxs-lookup"><span data-stu-id="67bc6-224">The Play for Work Store app URL.</span></span> <span data-ttu-id="67bc6-225">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-225">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="67bc6-226">isPrivate</span><span class="sxs-lookup"><span data-stu-id="67bc6-226">isPrivate</span></span>|<span data-ttu-id="67bc6-227">布尔</span><span class="sxs-lookup"><span data-stu-id="67bc6-227">Boolean</span></span>|<span data-ttu-id="67bc6-228">指示应用程序是否仅适用于给定企业的用户。</span><span class="sxs-lookup"><span data-stu-id="67bc6-228">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="67bc6-229">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-229">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="67bc6-230">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="67bc6-230">isSystemApp</span></span>|<span data-ttu-id="67bc6-231">布尔</span><span class="sxs-lookup"><span data-stu-id="67bc6-231">Boolean</span></span>|<span data-ttu-id="67bc6-232">指示应用程序是否为预安装的系统应用程序。</span><span class="sxs-lookup"><span data-stu-id="67bc6-232">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="67bc6-233">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-233">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="67bc6-234">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="67bc6-234">supportsOemConfig</span></span>|<span data-ttu-id="67bc6-235">布尔</span><span class="sxs-lookup"><span data-stu-id="67bc6-235">Boolean</span></span>|<span data-ttu-id="67bc6-236">此应用是否支持 OEMConfig 策略。</span><span class="sxs-lookup"><span data-stu-id="67bc6-236">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="67bc6-237">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="67bc6-237">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="67bc6-238">响应</span><span class="sxs-lookup"><span data-stu-id="67bc6-238">Response</span></span>
<span data-ttu-id="67bc6-239">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="67bc6-239">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67bc6-240">示例</span><span class="sxs-lookup"><span data-stu-id="67bc6-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="67bc6-241">请求</span><span class="sxs-lookup"><span data-stu-id="67bc6-241">Request</span></span>
<span data-ttu-id="67bc6-242">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="67bc6-242">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="67bc6-243">响应</span><span class="sxs-lookup"><span data-stu-id="67bc6-243">Response</span></span>
<span data-ttu-id="67bc6-p127">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="67bc6-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





