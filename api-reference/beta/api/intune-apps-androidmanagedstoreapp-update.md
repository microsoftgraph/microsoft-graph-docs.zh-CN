---
title: 更新 androidManagedStoreApp
description: 更新 androidManagedStoreApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc103c8f23548b9ba6c97cb00e03e01b72e3006a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700645"
---
# <a name="update-androidmanagedstoreapp"></a><span data-ttu-id="6078b-103">更新 androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="6078b-103">Update androidManagedStoreApp</span></span>

<span data-ttu-id="6078b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6078b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6078b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6078b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6078b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6078b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6078b-107">更新 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6078b-107">Update the properties of a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6078b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6078b-108">Prerequisites</span></span>
<span data-ttu-id="6078b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6078b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6078b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6078b-111">Permission type</span></span>|<span data-ttu-id="6078b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6078b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6078b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6078b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6078b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6078b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6078b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6078b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6078b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6078b-116">Not supported.</span></span>|
|<span data-ttu-id="6078b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6078b-117">Application</span></span>|<span data-ttu-id="6078b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6078b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6078b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6078b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="6078b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6078b-120">Request headers</span></span>
|<span data-ttu-id="6078b-121">标头</span><span class="sxs-lookup"><span data-stu-id="6078b-121">Header</span></span>|<span data-ttu-id="6078b-122">值</span><span class="sxs-lookup"><span data-stu-id="6078b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6078b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6078b-123">Authorization</span></span>|<span data-ttu-id="6078b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6078b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6078b-125">接受</span><span class="sxs-lookup"><span data-stu-id="6078b-125">Accept</span></span>|<span data-ttu-id="6078b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6078b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6078b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6078b-127">Request body</span></span>
<span data-ttu-id="6078b-128">在请求正文中，提供 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6078b-128">In the request body, supply a JSON representation for the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

<span data-ttu-id="6078b-129">下表显示创建 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6078b-129">The following table shows the properties that are required when you create the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span></span>

|<span data-ttu-id="6078b-130">属性</span><span class="sxs-lookup"><span data-stu-id="6078b-130">Property</span></span>|<span data-ttu-id="6078b-131">类型</span><span class="sxs-lookup"><span data-stu-id="6078b-131">Type</span></span>|<span data-ttu-id="6078b-132">说明</span><span class="sxs-lookup"><span data-stu-id="6078b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6078b-133">id</span><span class="sxs-lookup"><span data-stu-id="6078b-133">id</span></span>|<span data-ttu-id="6078b-134">String</span><span class="sxs-lookup"><span data-stu-id="6078b-134">String</span></span>|<span data-ttu-id="6078b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6078b-135">Key of the entity.</span></span> <span data-ttu-id="6078b-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6078b-137">displayName</span></span>|<span data-ttu-id="6078b-138">String</span><span class="sxs-lookup"><span data-stu-id="6078b-138">String</span></span>|<span data-ttu-id="6078b-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="6078b-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6078b-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-141">说明</span><span class="sxs-lookup"><span data-stu-id="6078b-141">description</span></span>|<span data-ttu-id="6078b-142">String</span><span class="sxs-lookup"><span data-stu-id="6078b-142">String</span></span>|<span data-ttu-id="6078b-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="6078b-143">The description of the app.</span></span> <span data-ttu-id="6078b-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-145">publisher</span><span class="sxs-lookup"><span data-stu-id="6078b-145">publisher</span></span>|<span data-ttu-id="6078b-146">String</span><span class="sxs-lookup"><span data-stu-id="6078b-146">String</span></span>|<span data-ttu-id="6078b-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="6078b-147">The publisher of the app.</span></span> <span data-ttu-id="6078b-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6078b-149">largeIcon</span></span>|[<span data-ttu-id="6078b-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6078b-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6078b-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="6078b-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6078b-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6078b-153">createdDateTime</span></span>|<span data-ttu-id="6078b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6078b-154">DateTimeOffset</span></span>|<span data-ttu-id="6078b-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6078b-155">The date and time the app was created.</span></span> <span data-ttu-id="6078b-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6078b-157">lastModifiedDateTime</span></span>|<span data-ttu-id="6078b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6078b-158">DateTimeOffset</span></span>|<span data-ttu-id="6078b-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6078b-159">The date and time the app was last modified.</span></span> <span data-ttu-id="6078b-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6078b-161">isFeatured</span></span>|<span data-ttu-id="6078b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="6078b-162">Boolean</span></span>|<span data-ttu-id="6078b-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6078b-164">privacyInformationUrl</span></span>|<span data-ttu-id="6078b-165">String</span><span class="sxs-lookup"><span data-stu-id="6078b-165">String</span></span>|<span data-ttu-id="6078b-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="6078b-166">The privacy statement Url.</span></span> <span data-ttu-id="6078b-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6078b-168">informationUrl</span></span>|<span data-ttu-id="6078b-169">String</span><span class="sxs-lookup"><span data-stu-id="6078b-169">String</span></span>|<span data-ttu-id="6078b-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="6078b-170">The more information Url.</span></span> <span data-ttu-id="6078b-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-172">owner</span><span class="sxs-lookup"><span data-stu-id="6078b-172">owner</span></span>|<span data-ttu-id="6078b-173">String</span><span class="sxs-lookup"><span data-stu-id="6078b-173">String</span></span>|<span data-ttu-id="6078b-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="6078b-174">The owner of the app.</span></span> <span data-ttu-id="6078b-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-176">developer</span><span class="sxs-lookup"><span data-stu-id="6078b-176">developer</span></span>|<span data-ttu-id="6078b-177">String</span><span class="sxs-lookup"><span data-stu-id="6078b-177">String</span></span>|<span data-ttu-id="6078b-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="6078b-178">The developer of the app.</span></span> <span data-ttu-id="6078b-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-180">notes</span><span class="sxs-lookup"><span data-stu-id="6078b-180">notes</span></span>|<span data-ttu-id="6078b-181">String</span><span class="sxs-lookup"><span data-stu-id="6078b-181">String</span></span>|<span data-ttu-id="6078b-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="6078b-182">Notes for the app.</span></span> <span data-ttu-id="6078b-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="6078b-184">uploadState</span></span>|<span data-ttu-id="6078b-185">Int32</span><span class="sxs-lookup"><span data-stu-id="6078b-185">Int32</span></span>|<span data-ttu-id="6078b-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="6078b-186">The upload state.</span></span> <span data-ttu-id="6078b-187">可能的值包括： 0- `Not Ready` 、1- `Ready` 、2- `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="6078b-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="6078b-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="6078b-189">publishingState</span></span>|[<span data-ttu-id="6078b-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6078b-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6078b-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="6078b-191">The publishing state for the app.</span></span> <span data-ttu-id="6078b-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="6078b-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6078b-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="6078b-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="6078b-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="6078b-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6078b-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6078b-195">isAssigned</span></span>|<span data-ttu-id="6078b-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="6078b-196">Boolean</span></span>|<span data-ttu-id="6078b-197">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="6078b-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="6078b-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6078b-199">roleScopeTagIds</span></span>|<span data-ttu-id="6078b-200">String collection</span><span class="sxs-lookup"><span data-stu-id="6078b-200">String collection</span></span>|<span data-ttu-id="6078b-201">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="6078b-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="6078b-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="6078b-203">dependentAppCount</span></span>|<span data-ttu-id="6078b-204">Int32</span><span class="sxs-lookup"><span data-stu-id="6078b-204">Int32</span></span>|<span data-ttu-id="6078b-205">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="6078b-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="6078b-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="6078b-207">supersedingAppCount</span></span>|<span data-ttu-id="6078b-208">Int32</span><span class="sxs-lookup"><span data-stu-id="6078b-208">Int32</span></span>|<span data-ttu-id="6078b-209">此应用程序直接或间接取代的应用程序总数量。</span><span class="sxs-lookup"><span data-stu-id="6078b-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="6078b-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="6078b-211">supersededAppCount</span></span>|<span data-ttu-id="6078b-212">Int32</span><span class="sxs-lookup"><span data-stu-id="6078b-212">Int32</span></span>|<span data-ttu-id="6078b-213">此应用程序直接或间接取代的应用程序总数量。</span><span class="sxs-lookup"><span data-stu-id="6078b-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="6078b-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6078b-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6078b-215">packageId</span><span class="sxs-lookup"><span data-stu-id="6078b-215">packageId</span></span>|<span data-ttu-id="6078b-216">String</span><span class="sxs-lookup"><span data-stu-id="6078b-216">String</span></span>|<span data-ttu-id="6078b-217">包标识符。</span><span class="sxs-lookup"><span data-stu-id="6078b-217">The package identifier.</span></span>|
|<span data-ttu-id="6078b-218">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="6078b-218">appIdentifier</span></span>|<span data-ttu-id="6078b-219">String</span><span class="sxs-lookup"><span data-stu-id="6078b-219">String</span></span>|<span data-ttu-id="6078b-220">标识名称。</span><span class="sxs-lookup"><span data-stu-id="6078b-220">The Identity Name.</span></span>|
|<span data-ttu-id="6078b-221">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6078b-221">usedLicenseCount</span></span>|<span data-ttu-id="6078b-222">Int32</span><span class="sxs-lookup"><span data-stu-id="6078b-222">Int32</span></span>|<span data-ttu-id="6078b-223">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="6078b-223">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="6078b-224">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6078b-224">totalLicenseCount</span></span>|<span data-ttu-id="6078b-225">Int32</span><span class="sxs-lookup"><span data-stu-id="6078b-225">Int32</span></span>|<span data-ttu-id="6078b-226">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="6078b-226">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="6078b-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6078b-227">appStoreUrl</span></span>|<span data-ttu-id="6078b-228">String</span><span class="sxs-lookup"><span data-stu-id="6078b-228">String</span></span>|<span data-ttu-id="6078b-229">"播放工作商店" 应用程序 URL。</span><span class="sxs-lookup"><span data-stu-id="6078b-229">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="6078b-230">isPrivate</span><span class="sxs-lookup"><span data-stu-id="6078b-230">isPrivate</span></span>|<span data-ttu-id="6078b-231">布尔</span><span class="sxs-lookup"><span data-stu-id="6078b-231">Boolean</span></span>|<span data-ttu-id="6078b-232">指示应用程序是否仅适用于给定企业的用户。</span><span class="sxs-lookup"><span data-stu-id="6078b-232">Indicates whether the app is only available to a given enterprise's users.</span></span>|
|<span data-ttu-id="6078b-233">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="6078b-233">isSystemApp</span></span>|<span data-ttu-id="6078b-234">布尔</span><span class="sxs-lookup"><span data-stu-id="6078b-234">Boolean</span></span>|<span data-ttu-id="6078b-235">指示应用程序是否为预安装的系统应用程序。</span><span class="sxs-lookup"><span data-stu-id="6078b-235">Indicates whether the app is a preinstalled system app.</span></span>|
|<span data-ttu-id="6078b-236">appTracks</span><span class="sxs-lookup"><span data-stu-id="6078b-236">appTracks</span></span>|<span data-ttu-id="6078b-237">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6078b-237">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="6078b-238">对此企业可见的曲目。</span><span class="sxs-lookup"><span data-stu-id="6078b-238">The tracks that are visible to this enterprise.</span></span>|
|<span data-ttu-id="6078b-239">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="6078b-239">supportsOemConfig</span></span>|<span data-ttu-id="6078b-240">布尔</span><span class="sxs-lookup"><span data-stu-id="6078b-240">Boolean</span></span>|<span data-ttu-id="6078b-241">此应用是否支持 OEMConfig 策略。</span><span class="sxs-lookup"><span data-stu-id="6078b-241">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="6078b-242">响应</span><span class="sxs-lookup"><span data-stu-id="6078b-242">Response</span></span>
<span data-ttu-id="6078b-243">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6078b-243">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6078b-244">示例</span><span class="sxs-lookup"><span data-stu-id="6078b-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="6078b-245">请求</span><span class="sxs-lookup"><span data-stu-id="6078b-245">Request</span></span>
<span data-ttu-id="6078b-246">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6078b-246">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1225

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

### <a name="response"></a><span data-ttu-id="6078b-247">响应</span><span class="sxs-lookup"><span data-stu-id="6078b-247">Response</span></span>
<span data-ttu-id="6078b-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6078b-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1397

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





