---
title: 更新 androidManagedStoreWebApp
description: 更新 androidManagedStoreWebApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11a011e018211d706f0dd340ac5a32137f2ea55f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144366"
---
# <a name="update-androidmanagedstorewebapp"></a><span data-ttu-id="fc514-103">更新 androidManagedStoreWebApp</span><span class="sxs-lookup"><span data-stu-id="fc514-103">Update androidManagedStoreWebApp</span></span>

<span data-ttu-id="fc514-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc514-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc514-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fc514-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc514-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc514-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc514-107">更新 [androidManagedStoreWebApp 对象](../resources/intune-apps-androidmanagedstorewebapp.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="fc514-107">Update the properties of a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc514-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fc514-108">Prerequisites</span></span>
<span data-ttu-id="fc514-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc514-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc514-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc514-111">Permission type</span></span>|<span data-ttu-id="fc514-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc514-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc514-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc514-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc514-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc514-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fc514-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc514-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc514-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc514-116">Not supported.</span></span>|
|<span data-ttu-id="fc514-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc514-117">Application</span></span>|<span data-ttu-id="fc514-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc514-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc514-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc514-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="fc514-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc514-120">Request headers</span></span>
|<span data-ttu-id="fc514-121">标头</span><span class="sxs-lookup"><span data-stu-id="fc514-121">Header</span></span>|<span data-ttu-id="fc514-122">值</span><span class="sxs-lookup"><span data-stu-id="fc514-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc514-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc514-123">Authorization</span></span>|<span data-ttu-id="fc514-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fc514-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc514-125">接受</span><span class="sxs-lookup"><span data-stu-id="fc514-125">Accept</span></span>|<span data-ttu-id="fc514-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc514-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc514-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc514-127">Request body</span></span>
<span data-ttu-id="fc514-128">在请求正文中，提供 [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc514-128">In the request body, supply a JSON representation for the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

<span data-ttu-id="fc514-129">下表显示创建 [androidManagedStoreWebApp 时所需的属性](../resources/intune-apps-androidmanagedstorewebapp.md)。</span><span class="sxs-lookup"><span data-stu-id="fc514-129">The following table shows the properties that are required when you create the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).</span></span>

|<span data-ttu-id="fc514-130">属性</span><span class="sxs-lookup"><span data-stu-id="fc514-130">Property</span></span>|<span data-ttu-id="fc514-131">类型</span><span class="sxs-lookup"><span data-stu-id="fc514-131">Type</span></span>|<span data-ttu-id="fc514-132">说明</span><span class="sxs-lookup"><span data-stu-id="fc514-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc514-133">id</span><span class="sxs-lookup"><span data-stu-id="fc514-133">id</span></span>|<span data-ttu-id="fc514-134">String</span><span class="sxs-lookup"><span data-stu-id="fc514-134">String</span></span>|<span data-ttu-id="fc514-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fc514-135">Key of the entity.</span></span> <span data-ttu-id="fc514-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-137">displayName</span><span class="sxs-lookup"><span data-stu-id="fc514-137">displayName</span></span>|<span data-ttu-id="fc514-138">String</span><span class="sxs-lookup"><span data-stu-id="fc514-138">String</span></span>|<span data-ttu-id="fc514-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="fc514-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fc514-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-141">说明</span><span class="sxs-lookup"><span data-stu-id="fc514-141">description</span></span>|<span data-ttu-id="fc514-142">String</span><span class="sxs-lookup"><span data-stu-id="fc514-142">String</span></span>|<span data-ttu-id="fc514-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="fc514-143">The description of the app.</span></span> <span data-ttu-id="fc514-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-145">publisher</span><span class="sxs-lookup"><span data-stu-id="fc514-145">publisher</span></span>|<span data-ttu-id="fc514-146">String</span><span class="sxs-lookup"><span data-stu-id="fc514-146">String</span></span>|<span data-ttu-id="fc514-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="fc514-147">The publisher of the app.</span></span> <span data-ttu-id="fc514-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fc514-149">largeIcon</span></span>|[<span data-ttu-id="fc514-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fc514-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fc514-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="fc514-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fc514-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fc514-153">createdDateTime</span></span>|<span data-ttu-id="fc514-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc514-154">DateTimeOffset</span></span>|<span data-ttu-id="fc514-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fc514-155">The date and time the app was created.</span></span> <span data-ttu-id="fc514-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc514-157">lastModifiedDateTime</span></span>|<span data-ttu-id="fc514-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc514-158">DateTimeOffset</span></span>|<span data-ttu-id="fc514-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fc514-159">The date and time the app was last modified.</span></span> <span data-ttu-id="fc514-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fc514-161">isFeatured</span></span>|<span data-ttu-id="fc514-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc514-162">Boolean</span></span>|<span data-ttu-id="fc514-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fc514-164">privacyInformationUrl</span></span>|<span data-ttu-id="fc514-165">String</span><span class="sxs-lookup"><span data-stu-id="fc514-165">String</span></span>|<span data-ttu-id="fc514-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="fc514-166">The privacy statement Url.</span></span> <span data-ttu-id="fc514-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fc514-168">informationUrl</span></span>|<span data-ttu-id="fc514-169">String</span><span class="sxs-lookup"><span data-stu-id="fc514-169">String</span></span>|<span data-ttu-id="fc514-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="fc514-170">The more information Url.</span></span> <span data-ttu-id="fc514-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-172">owner</span><span class="sxs-lookup"><span data-stu-id="fc514-172">owner</span></span>|<span data-ttu-id="fc514-173">String</span><span class="sxs-lookup"><span data-stu-id="fc514-173">String</span></span>|<span data-ttu-id="fc514-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="fc514-174">The owner of the app.</span></span> <span data-ttu-id="fc514-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-176">developer</span><span class="sxs-lookup"><span data-stu-id="fc514-176">developer</span></span>|<span data-ttu-id="fc514-177">String</span><span class="sxs-lookup"><span data-stu-id="fc514-177">String</span></span>|<span data-ttu-id="fc514-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="fc514-178">The developer of the app.</span></span> <span data-ttu-id="fc514-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-180">notes</span><span class="sxs-lookup"><span data-stu-id="fc514-180">notes</span></span>|<span data-ttu-id="fc514-181">String</span><span class="sxs-lookup"><span data-stu-id="fc514-181">String</span></span>|<span data-ttu-id="fc514-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="fc514-182">Notes for the app.</span></span> <span data-ttu-id="fc514-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="fc514-184">uploadState</span></span>|<span data-ttu-id="fc514-185">Int32</span><span class="sxs-lookup"><span data-stu-id="fc514-185">Int32</span></span>|<span data-ttu-id="fc514-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="fc514-186">The upload state.</span></span> <span data-ttu-id="fc514-187">可能的值是：0 - `Not Ready` 、1 - `Ready` 、2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="fc514-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="fc514-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="fc514-189">publishingState</span></span>|[<span data-ttu-id="fc514-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="fc514-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="fc514-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="fc514-191">The publishing state for the app.</span></span> <span data-ttu-id="fc514-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="fc514-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fc514-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="fc514-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="fc514-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="fc514-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fc514-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fc514-195">isAssigned</span></span>|<span data-ttu-id="fc514-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc514-196">Boolean</span></span>|<span data-ttu-id="fc514-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="fc514-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="fc514-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fc514-199">roleScopeTagIds</span></span>|<span data-ttu-id="fc514-200">String collection</span><span class="sxs-lookup"><span data-stu-id="fc514-200">String collection</span></span>|<span data-ttu-id="fc514-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="fc514-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="fc514-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="fc514-203">dependentAppCount</span></span>|<span data-ttu-id="fc514-204">Int32</span><span class="sxs-lookup"><span data-stu-id="fc514-204">Int32</span></span>|<span data-ttu-id="fc514-205">子应用具有的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="fc514-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="fc514-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="fc514-207">supersedingAppCount</span></span>|<span data-ttu-id="fc514-208">Int32</span><span class="sxs-lookup"><span data-stu-id="fc514-208">Int32</span></span>|<span data-ttu-id="fc514-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="fc514-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="fc514-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="fc514-211">supersededAppCount</span></span>|<span data-ttu-id="fc514-212">Int32</span><span class="sxs-lookup"><span data-stu-id="fc514-212">Int32</span></span>|<span data-ttu-id="fc514-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="fc514-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="fc514-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fc514-215">packageId</span><span class="sxs-lookup"><span data-stu-id="fc514-215">packageId</span></span>|<span data-ttu-id="fc514-216">String</span><span class="sxs-lookup"><span data-stu-id="fc514-216">String</span></span>|<span data-ttu-id="fc514-217">包标识符。</span><span class="sxs-lookup"><span data-stu-id="fc514-217">The package identifier.</span></span> <span data-ttu-id="fc514-218">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-218">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="fc514-219">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="fc514-219">appIdentifier</span></span>|<span data-ttu-id="fc514-220">String</span><span class="sxs-lookup"><span data-stu-id="fc514-220">String</span></span>|<span data-ttu-id="fc514-221">标识名称。</span><span class="sxs-lookup"><span data-stu-id="fc514-221">The Identity Name.</span></span> <span data-ttu-id="fc514-222">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-222">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="fc514-223">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="fc514-223">usedLicenseCount</span></span>|<span data-ttu-id="fc514-224">Int32</span><span class="sxs-lookup"><span data-stu-id="fc514-224">Int32</span></span>|<span data-ttu-id="fc514-225">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="fc514-225">The number of VPP licenses in use.</span></span> <span data-ttu-id="fc514-226">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-226">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="fc514-227">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="fc514-227">totalLicenseCount</span></span>|<span data-ttu-id="fc514-228">Int32</span><span class="sxs-lookup"><span data-stu-id="fc514-228">Int32</span></span>|<span data-ttu-id="fc514-229">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="fc514-229">The total number of VPP licenses.</span></span> <span data-ttu-id="fc514-230">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-230">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="fc514-231">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="fc514-231">appStoreUrl</span></span>|<span data-ttu-id="fc514-232">String</span><span class="sxs-lookup"><span data-stu-id="fc514-232">String</span></span>|<span data-ttu-id="fc514-233">"播放工作商店"应用 URL。</span><span class="sxs-lookup"><span data-stu-id="fc514-233">The Play for Work Store app URL.</span></span> <span data-ttu-id="fc514-234">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-234">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="fc514-235">isPrivate</span><span class="sxs-lookup"><span data-stu-id="fc514-235">isPrivate</span></span>|<span data-ttu-id="fc514-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc514-236">Boolean</span></span>|<span data-ttu-id="fc514-237">指示应用是否仅适用于给定企业的用户。</span><span class="sxs-lookup"><span data-stu-id="fc514-237">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="fc514-238">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-238">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="fc514-239">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="fc514-239">isSystemApp</span></span>|<span data-ttu-id="fc514-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc514-240">Boolean</span></span>|<span data-ttu-id="fc514-241">指示应用是否是预安装的系统应用。</span><span class="sxs-lookup"><span data-stu-id="fc514-241">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="fc514-242">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-242">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="fc514-243">appTracks</span><span class="sxs-lookup"><span data-stu-id="fc514-243">appTracks</span></span>|<span data-ttu-id="fc514-244">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fc514-244">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="fc514-245">此企业可见的轨。</span><span class="sxs-lookup"><span data-stu-id="fc514-245">The tracks that are visible to this enterprise.</span></span> <span data-ttu-id="fc514-246">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-246">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="fc514-247">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="fc514-247">supportsOemConfig</span></span>|<span data-ttu-id="fc514-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc514-248">Boolean</span></span>|<span data-ttu-id="fc514-249">此应用是否支持 OEMConfig 策略。</span><span class="sxs-lookup"><span data-stu-id="fc514-249">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="fc514-250">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc514-250">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="fc514-251">响应</span><span class="sxs-lookup"><span data-stu-id="fc514-251">Response</span></span>
<span data-ttu-id="fc514-252">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fc514-252">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc514-253">示例</span><span class="sxs-lookup"><span data-stu-id="fc514-253">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc514-254">请求</span><span class="sxs-lookup"><span data-stu-id="fc514-254">Request</span></span>
<span data-ttu-id="fc514-255">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc514-255">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1228

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "Track Id value",
      "trackAlias": "Track Alias value"
    }
  ],
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="fc514-256">响应</span><span class="sxs-lookup"><span data-stu-id="fc514-256">Response</span></span>
<span data-ttu-id="fc514-p130">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fc514-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1400

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "Track Id value",
      "trackAlias": "Track Alias value"
    }
  ],
  "supportsOemConfig": true
}
```




