---
title: 更新 managedIOSStoreApp
description: 更新 managedIOSStoreApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8943f032f55fc19831d2828d22aea332f049c8e8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140012"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="3affb-103">更新 managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="3affb-103">Update managedIOSStoreApp</span></span>

<span data-ttu-id="3affb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3affb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3affb-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3affb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3affb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3affb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3affb-107">更新 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3affb-107">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3affb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3affb-108">Prerequisites</span></span>
<span data-ttu-id="3affb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3affb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3affb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3affb-111">Permission type</span></span>|<span data-ttu-id="3affb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3affb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3affb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3affb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3affb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3affb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3affb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3affb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3affb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3affb-116">Not supported.</span></span>|
|<span data-ttu-id="3affb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3affb-117">Application</span></span>|<span data-ttu-id="3affb-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3affb-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3affb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3affb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="3affb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3affb-120">Request headers</span></span>
|<span data-ttu-id="3affb-121">标头</span><span class="sxs-lookup"><span data-stu-id="3affb-121">Header</span></span>|<span data-ttu-id="3affb-122">值</span><span class="sxs-lookup"><span data-stu-id="3affb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3affb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3affb-123">Authorization</span></span>|<span data-ttu-id="3affb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3affb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3affb-125">接受</span><span class="sxs-lookup"><span data-stu-id="3affb-125">Accept</span></span>|<span data-ttu-id="3affb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3affb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3affb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3affb-127">Request body</span></span>
<span data-ttu-id="3affb-128">在请求正文中，提供 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3affb-128">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="3affb-129">下表显示创建 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3affb-129">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="3affb-130">属性</span><span class="sxs-lookup"><span data-stu-id="3affb-130">Property</span></span>|<span data-ttu-id="3affb-131">类型</span><span class="sxs-lookup"><span data-stu-id="3affb-131">Type</span></span>|<span data-ttu-id="3affb-132">说明</span><span class="sxs-lookup"><span data-stu-id="3affb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3affb-133">id</span><span class="sxs-lookup"><span data-stu-id="3affb-133">id</span></span>|<span data-ttu-id="3affb-134">String</span><span class="sxs-lookup"><span data-stu-id="3affb-134">String</span></span>|<span data-ttu-id="3affb-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3affb-135">Key of the entity.</span></span> <span data-ttu-id="3affb-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3affb-137">displayName</span></span>|<span data-ttu-id="3affb-138">String</span><span class="sxs-lookup"><span data-stu-id="3affb-138">String</span></span>|<span data-ttu-id="3affb-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="3affb-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3affb-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-141">说明</span><span class="sxs-lookup"><span data-stu-id="3affb-141">description</span></span>|<span data-ttu-id="3affb-142">String</span><span class="sxs-lookup"><span data-stu-id="3affb-142">String</span></span>|<span data-ttu-id="3affb-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="3affb-143">The description of the app.</span></span> <span data-ttu-id="3affb-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-145">publisher</span><span class="sxs-lookup"><span data-stu-id="3affb-145">publisher</span></span>|<span data-ttu-id="3affb-146">String</span><span class="sxs-lookup"><span data-stu-id="3affb-146">String</span></span>|<span data-ttu-id="3affb-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="3affb-147">The publisher of the app.</span></span> <span data-ttu-id="3affb-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3affb-149">largeIcon</span></span>|[<span data-ttu-id="3affb-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3affb-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3affb-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="3affb-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3affb-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3affb-153">createdDateTime</span></span>|<span data-ttu-id="3affb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3affb-154">DateTimeOffset</span></span>|<span data-ttu-id="3affb-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3affb-155">The date and time the app was created.</span></span> <span data-ttu-id="3affb-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3affb-157">lastModifiedDateTime</span></span>|<span data-ttu-id="3affb-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3affb-158">DateTimeOffset</span></span>|<span data-ttu-id="3affb-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3affb-159">The date and time the app was last modified.</span></span> <span data-ttu-id="3affb-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3affb-161">isFeatured</span></span>|<span data-ttu-id="3affb-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3affb-162">Boolean</span></span>|<span data-ttu-id="3affb-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3affb-164">privacyInformationUrl</span></span>|<span data-ttu-id="3affb-165">String</span><span class="sxs-lookup"><span data-stu-id="3affb-165">String</span></span>|<span data-ttu-id="3affb-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="3affb-166">The privacy statement Url.</span></span> <span data-ttu-id="3affb-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3affb-168">informationUrl</span></span>|<span data-ttu-id="3affb-169">String</span><span class="sxs-lookup"><span data-stu-id="3affb-169">String</span></span>|<span data-ttu-id="3affb-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="3affb-170">The more information Url.</span></span> <span data-ttu-id="3affb-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-172">owner</span><span class="sxs-lookup"><span data-stu-id="3affb-172">owner</span></span>|<span data-ttu-id="3affb-173">String</span><span class="sxs-lookup"><span data-stu-id="3affb-173">String</span></span>|<span data-ttu-id="3affb-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="3affb-174">The owner of the app.</span></span> <span data-ttu-id="3affb-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-176">developer</span><span class="sxs-lookup"><span data-stu-id="3affb-176">developer</span></span>|<span data-ttu-id="3affb-177">String</span><span class="sxs-lookup"><span data-stu-id="3affb-177">String</span></span>|<span data-ttu-id="3affb-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="3affb-178">The developer of the app.</span></span> <span data-ttu-id="3affb-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-180">notes</span><span class="sxs-lookup"><span data-stu-id="3affb-180">notes</span></span>|<span data-ttu-id="3affb-181">String</span><span class="sxs-lookup"><span data-stu-id="3affb-181">String</span></span>|<span data-ttu-id="3affb-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="3affb-182">Notes for the app.</span></span> <span data-ttu-id="3affb-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="3affb-184">uploadState</span></span>|<span data-ttu-id="3affb-185">Int32</span><span class="sxs-lookup"><span data-stu-id="3affb-185">Int32</span></span>|<span data-ttu-id="3affb-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="3affb-186">The upload state.</span></span> <span data-ttu-id="3affb-187">可能的值是：0 - `Not Ready` 、1 - `Ready` 、2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="3affb-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="3affb-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="3affb-189">publishingState</span></span>|[<span data-ttu-id="3affb-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3affb-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3affb-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="3affb-191">The publishing state for the app.</span></span> <span data-ttu-id="3affb-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="3affb-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3affb-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="3affb-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="3affb-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="3affb-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3affb-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3affb-195">isAssigned</span></span>|<span data-ttu-id="3affb-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="3affb-196">Boolean</span></span>|<span data-ttu-id="3affb-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="3affb-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="3affb-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3affb-199">roleScopeTagIds</span></span>|<span data-ttu-id="3affb-200">String collection</span><span class="sxs-lookup"><span data-stu-id="3affb-200">String collection</span></span>|<span data-ttu-id="3affb-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="3affb-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="3affb-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="3affb-203">dependentAppCount</span></span>|<span data-ttu-id="3affb-204">Int32</span><span class="sxs-lookup"><span data-stu-id="3affb-204">Int32</span></span>|<span data-ttu-id="3affb-205">子应用具有的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="3affb-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="3affb-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="3affb-207">supersedingAppCount</span></span>|<span data-ttu-id="3affb-208">Int32</span><span class="sxs-lookup"><span data-stu-id="3affb-208">Int32</span></span>|<span data-ttu-id="3affb-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="3affb-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="3affb-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="3affb-211">supersededAppCount</span></span>|<span data-ttu-id="3affb-212">Int32</span><span class="sxs-lookup"><span data-stu-id="3affb-212">Int32</span></span>|<span data-ttu-id="3affb-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="3affb-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="3affb-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3affb-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="3affb-215">appAvailability</span></span>|[<span data-ttu-id="3affb-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="3affb-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="3affb-217">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="3affb-217">The Application's availability.</span></span> <span data-ttu-id="3affb-218">继承自 [managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="3affb-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="3affb-219">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="3affb-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="3affb-220">version</span><span class="sxs-lookup"><span data-stu-id="3affb-220">version</span></span>|<span data-ttu-id="3affb-221">String</span><span class="sxs-lookup"><span data-stu-id="3affb-221">String</span></span>|<span data-ttu-id="3affb-222">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="3affb-222">The Application's version.</span></span> <span data-ttu-id="3affb-223">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="3affb-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="3affb-224">bundleId</span><span class="sxs-lookup"><span data-stu-id="3affb-224">bundleId</span></span>|<span data-ttu-id="3affb-225">String</span><span class="sxs-lookup"><span data-stu-id="3affb-225">String</span></span>|<span data-ttu-id="3affb-226">应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="3affb-226">The app's Bundle ID.</span></span>|
|<span data-ttu-id="3affb-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="3affb-227">appStoreUrl</span></span>|<span data-ttu-id="3affb-228">String</span><span class="sxs-lookup"><span data-stu-id="3affb-228">String</span></span>|<span data-ttu-id="3affb-229">Apple AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="3affb-229">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="3affb-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="3affb-230">applicableDeviceType</span></span>|[<span data-ttu-id="3affb-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="3affb-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="3affb-232">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="3affb-232">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="3affb-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3affb-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3affb-234">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3affb-234">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="3affb-235">最低受支持操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="3affb-235">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="3affb-236">响应</span><span class="sxs-lookup"><span data-stu-id="3affb-236">Response</span></span>
<span data-ttu-id="3affb-237">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3affb-237">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3affb-238">示例</span><span class="sxs-lookup"><span data-stu-id="3affb-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="3affb-239">请求</span><span class="sxs-lookup"><span data-stu-id="3affb-239">Request</span></span>
<span data-ttu-id="3affb-240">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3affb-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1315

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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
    "v13_0": true,
    "v14_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="3affb-241">响应</span><span class="sxs-lookup"><span data-stu-id="3affb-241">Response</span></span>
<span data-ttu-id="3affb-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3affb-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1487

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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
    "v13_0": true,
    "v14_0": true
  }
}
```




