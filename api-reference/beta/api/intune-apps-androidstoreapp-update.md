---
title: 更新 androidStoreApp
description: 更新 androidStoreApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dc1406bf1c788ec819002b6958168718330b3e46
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140852"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="f0327-103">更新 androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="f0327-103">Update androidStoreApp</span></span>

<span data-ttu-id="f0327-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0327-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0327-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f0327-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0327-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0327-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0327-107">更新 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f0327-107">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0327-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f0327-108">Prerequisites</span></span>
<span data-ttu-id="f0327-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0327-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0327-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0327-111">Permission type</span></span>|<span data-ttu-id="f0327-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f0327-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0327-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0327-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0327-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0327-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f0327-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0327-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0327-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0327-116">Not supported.</span></span>|
|<span data-ttu-id="f0327-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0327-117">Application</span></span>|<span data-ttu-id="f0327-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0327-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0327-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0327-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f0327-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0327-120">Request headers</span></span>
|<span data-ttu-id="f0327-121">标头</span><span class="sxs-lookup"><span data-stu-id="f0327-121">Header</span></span>|<span data-ttu-id="f0327-122">值</span><span class="sxs-lookup"><span data-stu-id="f0327-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0327-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0327-123">Authorization</span></span>|<span data-ttu-id="f0327-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f0327-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0327-125">接受</span><span class="sxs-lookup"><span data-stu-id="f0327-125">Accept</span></span>|<span data-ttu-id="f0327-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0327-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0327-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0327-127">Request body</span></span>
<span data-ttu-id="f0327-128">在请求正文中，提供 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0327-128">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="f0327-129">下表显示了创建 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f0327-129">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="f0327-130">属性</span><span class="sxs-lookup"><span data-stu-id="f0327-130">Property</span></span>|<span data-ttu-id="f0327-131">类型</span><span class="sxs-lookup"><span data-stu-id="f0327-131">Type</span></span>|<span data-ttu-id="f0327-132">说明</span><span class="sxs-lookup"><span data-stu-id="f0327-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0327-133">id</span><span class="sxs-lookup"><span data-stu-id="f0327-133">id</span></span>|<span data-ttu-id="f0327-134">String</span><span class="sxs-lookup"><span data-stu-id="f0327-134">String</span></span>|<span data-ttu-id="f0327-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f0327-135">Key of the entity.</span></span> <span data-ttu-id="f0327-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f0327-137">displayName</span></span>|<span data-ttu-id="f0327-138">String</span><span class="sxs-lookup"><span data-stu-id="f0327-138">String</span></span>|<span data-ttu-id="f0327-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="f0327-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f0327-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-141">说明</span><span class="sxs-lookup"><span data-stu-id="f0327-141">description</span></span>|<span data-ttu-id="f0327-142">String</span><span class="sxs-lookup"><span data-stu-id="f0327-142">String</span></span>|<span data-ttu-id="f0327-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="f0327-143">The description of the app.</span></span> <span data-ttu-id="f0327-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-145">publisher</span><span class="sxs-lookup"><span data-stu-id="f0327-145">publisher</span></span>|<span data-ttu-id="f0327-146">String</span><span class="sxs-lookup"><span data-stu-id="f0327-146">String</span></span>|<span data-ttu-id="f0327-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="f0327-147">The publisher of the app.</span></span> <span data-ttu-id="f0327-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f0327-149">largeIcon</span></span>|[<span data-ttu-id="f0327-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f0327-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f0327-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="f0327-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f0327-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0327-153">createdDateTime</span></span>|<span data-ttu-id="f0327-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0327-154">DateTimeOffset</span></span>|<span data-ttu-id="f0327-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f0327-155">The date and time the app was created.</span></span> <span data-ttu-id="f0327-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0327-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f0327-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0327-158">DateTimeOffset</span></span>|<span data-ttu-id="f0327-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f0327-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f0327-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f0327-161">isFeatured</span></span>|<span data-ttu-id="f0327-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0327-162">Boolean</span></span>|<span data-ttu-id="f0327-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f0327-164">privacyInformationUrl</span></span>|<span data-ttu-id="f0327-165">String</span><span class="sxs-lookup"><span data-stu-id="f0327-165">String</span></span>|<span data-ttu-id="f0327-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="f0327-166">The privacy statement Url.</span></span> <span data-ttu-id="f0327-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f0327-168">informationUrl</span></span>|<span data-ttu-id="f0327-169">String</span><span class="sxs-lookup"><span data-stu-id="f0327-169">String</span></span>|<span data-ttu-id="f0327-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="f0327-170">The more information Url.</span></span> <span data-ttu-id="f0327-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-172">owner</span><span class="sxs-lookup"><span data-stu-id="f0327-172">owner</span></span>|<span data-ttu-id="f0327-173">String</span><span class="sxs-lookup"><span data-stu-id="f0327-173">String</span></span>|<span data-ttu-id="f0327-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="f0327-174">The owner of the app.</span></span> <span data-ttu-id="f0327-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-176">developer</span><span class="sxs-lookup"><span data-stu-id="f0327-176">developer</span></span>|<span data-ttu-id="f0327-177">String</span><span class="sxs-lookup"><span data-stu-id="f0327-177">String</span></span>|<span data-ttu-id="f0327-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="f0327-178">The developer of the app.</span></span> <span data-ttu-id="f0327-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-180">notes</span><span class="sxs-lookup"><span data-stu-id="f0327-180">notes</span></span>|<span data-ttu-id="f0327-181">String</span><span class="sxs-lookup"><span data-stu-id="f0327-181">String</span></span>|<span data-ttu-id="f0327-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="f0327-182">Notes for the app.</span></span> <span data-ttu-id="f0327-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f0327-184">uploadState</span></span>|<span data-ttu-id="f0327-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f0327-185">Int32</span></span>|<span data-ttu-id="f0327-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="f0327-186">The upload state.</span></span> <span data-ttu-id="f0327-187">可能的值是：0 - `Not Ready` 、1 - `Ready` 、2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="f0327-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="f0327-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="f0327-189">publishingState</span></span>|[<span data-ttu-id="f0327-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f0327-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f0327-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="f0327-191">The publishing state for the app.</span></span> <span data-ttu-id="f0327-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="f0327-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f0327-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="f0327-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="f0327-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="f0327-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f0327-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f0327-195">isAssigned</span></span>|<span data-ttu-id="f0327-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0327-196">Boolean</span></span>|<span data-ttu-id="f0327-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="f0327-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f0327-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f0327-199">roleScopeTagIds</span></span>|<span data-ttu-id="f0327-200">String collection</span><span class="sxs-lookup"><span data-stu-id="f0327-200">String collection</span></span>|<span data-ttu-id="f0327-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="f0327-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f0327-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="f0327-203">dependentAppCount</span></span>|<span data-ttu-id="f0327-204">Int32</span><span class="sxs-lookup"><span data-stu-id="f0327-204">Int32</span></span>|<span data-ttu-id="f0327-205">子应用具有的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="f0327-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f0327-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="f0327-207">supersedingAppCount</span></span>|<span data-ttu-id="f0327-208">Int32</span><span class="sxs-lookup"><span data-stu-id="f0327-208">Int32</span></span>|<span data-ttu-id="f0327-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="f0327-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="f0327-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="f0327-211">supersededAppCount</span></span>|<span data-ttu-id="f0327-212">Int32</span><span class="sxs-lookup"><span data-stu-id="f0327-212">Int32</span></span>|<span data-ttu-id="f0327-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="f0327-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="f0327-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0327-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0327-215">packageId</span><span class="sxs-lookup"><span data-stu-id="f0327-215">packageId</span></span>|<span data-ttu-id="f0327-216">String</span><span class="sxs-lookup"><span data-stu-id="f0327-216">String</span></span>|<span data-ttu-id="f0327-217">包标识符。</span><span class="sxs-lookup"><span data-stu-id="f0327-217">The package identifier.</span></span>|
|<span data-ttu-id="f0327-218">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="f0327-218">appIdentifier</span></span>|<span data-ttu-id="f0327-219">String</span><span class="sxs-lookup"><span data-stu-id="f0327-219">String</span></span>|<span data-ttu-id="f0327-220">标识名称。</span><span class="sxs-lookup"><span data-stu-id="f0327-220">The Identity Name.</span></span>|
|<span data-ttu-id="f0327-221">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f0327-221">appStoreUrl</span></span>|<span data-ttu-id="f0327-222">String</span><span class="sxs-lookup"><span data-stu-id="f0327-222">String</span></span>|<span data-ttu-id="f0327-223">Android 应用商店 URL。</span><span class="sxs-lookup"><span data-stu-id="f0327-223">The Android app store URL.</span></span>|
|<span data-ttu-id="f0327-224">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f0327-224">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f0327-225">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f0327-225">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="f0327-226">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="f0327-226">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="f0327-227">响应</span><span class="sxs-lookup"><span data-stu-id="f0327-227">Response</span></span>
<span data-ttu-id="f0327-228">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f0327-228">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0327-229">示例</span><span class="sxs-lookup"><span data-stu-id="f0327-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0327-230">请求</span><span class="sxs-lookup"><span data-stu-id="f0327-230">Request</span></span>
<span data-ttu-id="f0327-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f0327-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1327

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="f0327-232">响应</span><span class="sxs-lookup"><span data-stu-id="f0327-232">Response</span></span>
<span data-ttu-id="f0327-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0327-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1499

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  }
}
```




