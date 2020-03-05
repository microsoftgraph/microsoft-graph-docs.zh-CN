---
title: 更新 androidManagedStoreApp
description: 更新 androidManagedStoreApp 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a8cf1e898e64ec2b8d958d935372553f8ca91993
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445895"
---
# <a name="update-androidmanagedstoreapp"></a><span data-ttu-id="7dadf-103">更新 androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="7dadf-103">Update androidManagedStoreApp</span></span>

<span data-ttu-id="7dadf-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7dadf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7dadf-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7dadf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7dadf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7dadf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dadf-107">更新[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7dadf-107">Update the properties of a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7dadf-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7dadf-108">Prerequisites</span></span>
<span data-ttu-id="7dadf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7dadf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dadf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7dadf-111">Permission type</span></span>|<span data-ttu-id="7dadf-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7dadf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dadf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7dadf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7dadf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dadf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7dadf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7dadf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dadf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7dadf-116">Not supported.</span></span>|
|<span data-ttu-id="7dadf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7dadf-117">Application</span></span>|<span data-ttu-id="7dadf-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dadf-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dadf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7dadf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="7dadf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7dadf-120">Request headers</span></span>
|<span data-ttu-id="7dadf-121">标头</span><span class="sxs-lookup"><span data-stu-id="7dadf-121">Header</span></span>|<span data-ttu-id="7dadf-122">值</span><span class="sxs-lookup"><span data-stu-id="7dadf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dadf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dadf-123">Authorization</span></span>|<span data-ttu-id="7dadf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7dadf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dadf-125">接受</span><span class="sxs-lookup"><span data-stu-id="7dadf-125">Accept</span></span>|<span data-ttu-id="7dadf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7dadf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dadf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7dadf-127">Request body</span></span>
<span data-ttu-id="7dadf-128">在请求正文中，提供[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7dadf-128">In the request body, supply a JSON representation for the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

<span data-ttu-id="7dadf-129">下表显示创建[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7dadf-129">The following table shows the properties that are required when you create the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span></span>

|<span data-ttu-id="7dadf-130">属性</span><span class="sxs-lookup"><span data-stu-id="7dadf-130">Property</span></span>|<span data-ttu-id="7dadf-131">类型</span><span class="sxs-lookup"><span data-stu-id="7dadf-131">Type</span></span>|<span data-ttu-id="7dadf-132">说明</span><span class="sxs-lookup"><span data-stu-id="7dadf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dadf-133">id</span><span class="sxs-lookup"><span data-stu-id="7dadf-133">id</span></span>|<span data-ttu-id="7dadf-134">字符串</span><span class="sxs-lookup"><span data-stu-id="7dadf-134">String</span></span>|<span data-ttu-id="7dadf-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7dadf-135">Key of the entity.</span></span> <span data-ttu-id="7dadf-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dadf-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dadf-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7dadf-137">displayName</span></span>|<span data-ttu-id="7dadf-138">String</span><span class="sxs-lookup"><span data-stu-id="7dadf-138">String</span></span>|<span data-ttu-id="7dadf-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="7dadf-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7dadf-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dadf-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dadf-141">说明</span><span class="sxs-lookup"><span data-stu-id="7dadf-141">description</span></span>|<span data-ttu-id="7dadf-142">字符串</span><span class="sxs-lookup"><span data-stu-id="7dadf-142">String</span></span>|<span data-ttu-id="7dadf-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="7dadf-143">The description of the app.</span></span> <span data-ttu-id="7dadf-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dadf-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dadf-145">publisher</span><span class="sxs-lookup"><span data-stu-id="7dadf-145">publisher</span></span>|<span data-ttu-id="7dadf-146">String</span><span class="sxs-lookup"><span data-stu-id="7dadf-146">String</span></span>|<span data-ttu-id="7dadf-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="7dadf-147">The publisher of the app.</span></span> <span data-ttu-id="7dadf-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dadf-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dadf-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7dadf-149">largeIcon</span></span>|[<span data-ttu-id="7dadf-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7dadf-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7dadf-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="7dadf-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7dadf-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dadf-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dadf-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7dadf-153">createdDateTime</span></span>|<span data-ttu-id="7dadf-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dadf-154">DateTimeOffset</span></span>|<span data-ttu-id="7dadf-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7dadf-155">The date and time the app was created.</span></span> <span data-ttu-id="7dadf-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dadf-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dadf-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7dadf-157">lastModifiedDateTime</span></span>|<span data-ttu-id="7dadf-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dadf-158">DateTimeOffset</span></span>|<span data-ttu-id="7dadf-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7dadf-159">The date and time the app was last modified.</span></span> <span data-ttu-id="7dadf-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dadf-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dadf-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7dadf-161">isFeatured</span></span>|<span data-ttu-id="7dadf-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dadf-162">Boolean</span></span>|<span data-ttu-id="7dadf-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dadf-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dadf-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7dadf-164">privacyInformationUrl</span></span>|<span data-ttu-id="7dadf-165">String</span><span class="sxs-lookup"><span data-stu-id="7dadf-165">String</span></span>|<span data-ttu-id="7dadf-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="7dadf-166">The privacy statement Url.</span></span> <span data-ttu-id="7dadf-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dadf-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dadf-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7dadf-168">informationUrl</span></span>|<span data-ttu-id="7dadf-169">String</span><span class="sxs-lookup"><span data-stu-id="7dadf-169">String</span></span>|<span data-ttu-id="7dadf-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="7dadf-170">The more information Url.</span></span> <span data-ttu-id="7dadf-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dadf-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dadf-172">owner</span><span class="sxs-lookup"><span data-stu-id="7dadf-172">owner</span></span>|<span data-ttu-id="7dadf-173">String</span><span class="sxs-lookup"><span data-stu-id="7dadf-173">String</span></span>|<span data-ttu-id="7dadf-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="7dadf-174">The owner of the app.</span></span> <span data-ttu-id="7dadf-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dadf-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dadf-176">developer</span><span class="sxs-lookup"><span data-stu-id="7dadf-176">developer</span></span>|<span data-ttu-id="7dadf-177">String</span><span class="sxs-lookup"><span data-stu-id="7dadf-177">String</span></span>|<span data-ttu-id="7dadf-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="7dadf-178">The developer of the app.</span></span> <span data-ttu-id="7dadf-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dadf-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dadf-180">notes</span><span class="sxs-lookup"><span data-stu-id="7dadf-180">notes</span></span>|<span data-ttu-id="7dadf-181">String</span><span class="sxs-lookup"><span data-stu-id="7dadf-181">String</span></span>|<span data-ttu-id="7dadf-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="7dadf-182">Notes for the app.</span></span> <span data-ttu-id="7dadf-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dadf-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dadf-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="7dadf-184">uploadState</span></span>|<span data-ttu-id="7dadf-185">Int32</span><span class="sxs-lookup"><span data-stu-id="7dadf-185">Int32</span></span>|<span data-ttu-id="7dadf-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="7dadf-186">The upload state.</span></span> <span data-ttu-id="7dadf-187">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dadf-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dadf-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="7dadf-188">publishingState</span></span>|[<span data-ttu-id="7dadf-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7dadf-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7dadf-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="7dadf-190">The publishing state for the app.</span></span> <span data-ttu-id="7dadf-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="7dadf-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7dadf-192">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="7dadf-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="7dadf-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="7dadf-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7dadf-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7dadf-194">isAssigned</span></span>|<span data-ttu-id="7dadf-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dadf-195">Boolean</span></span>|<span data-ttu-id="7dadf-196">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="7dadf-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7dadf-197">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dadf-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dadf-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7dadf-198">roleScopeTagIds</span></span>|<span data-ttu-id="7dadf-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="7dadf-199">String collection</span></span>|<span data-ttu-id="7dadf-200">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="7dadf-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7dadf-201">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dadf-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dadf-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="7dadf-202">dependentAppCount</span></span>|<span data-ttu-id="7dadf-203">Int32</span><span class="sxs-lookup"><span data-stu-id="7dadf-203">Int32</span></span>|<span data-ttu-id="7dadf-204">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="7dadf-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="7dadf-205">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dadf-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dadf-206">packageId</span><span class="sxs-lookup"><span data-stu-id="7dadf-206">packageId</span></span>|<span data-ttu-id="7dadf-207">String</span><span class="sxs-lookup"><span data-stu-id="7dadf-207">String</span></span>|<span data-ttu-id="7dadf-208">包标识符。</span><span class="sxs-lookup"><span data-stu-id="7dadf-208">The package identifier.</span></span>|
|<span data-ttu-id="7dadf-209">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="7dadf-209">appIdentifier</span></span>|<span data-ttu-id="7dadf-210">String</span><span class="sxs-lookup"><span data-stu-id="7dadf-210">String</span></span>|<span data-ttu-id="7dadf-211">标识名称。</span><span class="sxs-lookup"><span data-stu-id="7dadf-211">The Identity Name.</span></span>|
|<span data-ttu-id="7dadf-212">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7dadf-212">usedLicenseCount</span></span>|<span data-ttu-id="7dadf-213">Int32</span><span class="sxs-lookup"><span data-stu-id="7dadf-213">Int32</span></span>|<span data-ttu-id="7dadf-214">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="7dadf-214">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="7dadf-215">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7dadf-215">totalLicenseCount</span></span>|<span data-ttu-id="7dadf-216">Int32</span><span class="sxs-lookup"><span data-stu-id="7dadf-216">Int32</span></span>|<span data-ttu-id="7dadf-217">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="7dadf-217">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="7dadf-218">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7dadf-218">appStoreUrl</span></span>|<span data-ttu-id="7dadf-219">String</span><span class="sxs-lookup"><span data-stu-id="7dadf-219">String</span></span>|<span data-ttu-id="7dadf-220">"播放工作商店" 应用程序 URL。</span><span class="sxs-lookup"><span data-stu-id="7dadf-220">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="7dadf-221">isPrivate</span><span class="sxs-lookup"><span data-stu-id="7dadf-221">isPrivate</span></span>|<span data-ttu-id="7dadf-222">布尔</span><span class="sxs-lookup"><span data-stu-id="7dadf-222">Boolean</span></span>|<span data-ttu-id="7dadf-223">指示应用程序是否仅适用于给定企业的用户。</span><span class="sxs-lookup"><span data-stu-id="7dadf-223">Indicates whether the app is only available to a given enterprise's users.</span></span>|
|<span data-ttu-id="7dadf-224">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="7dadf-224">isSystemApp</span></span>|<span data-ttu-id="7dadf-225">布尔</span><span class="sxs-lookup"><span data-stu-id="7dadf-225">Boolean</span></span>|<span data-ttu-id="7dadf-226">指示应用程序是否为预安装的系统应用程序。</span><span class="sxs-lookup"><span data-stu-id="7dadf-226">Indicates whether the app is a preinstalled system app.</span></span>|
|<span data-ttu-id="7dadf-227">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="7dadf-227">supportsOemConfig</span></span>|<span data-ttu-id="7dadf-228">布尔</span><span class="sxs-lookup"><span data-stu-id="7dadf-228">Boolean</span></span>|<span data-ttu-id="7dadf-229">此应用是否支持 OEMConfig 策略。</span><span class="sxs-lookup"><span data-stu-id="7dadf-229">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="7dadf-230">响应</span><span class="sxs-lookup"><span data-stu-id="7dadf-230">Response</span></span>
<span data-ttu-id="7dadf-231">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7dadf-231">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dadf-232">示例</span><span class="sxs-lookup"><span data-stu-id="7dadf-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="7dadf-233">请求</span><span class="sxs-lookup"><span data-stu-id="7dadf-233">Request</span></span>
<span data-ttu-id="7dadf-234">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7dadf-234">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 984

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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

### <a name="response"></a><span data-ttu-id="7dadf-235">响应</span><span class="sxs-lookup"><span data-stu-id="7dadf-235">Response</span></span>
<span data-ttu-id="7dadf-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7dadf-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1156

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
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





