---
title: 更新 macOsVppApp
description: 更新 macOsVppApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 674ba7373c43f1ec0baa44a51f02ca5cd29bc29f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143813"
---
# <a name="update-macosvppapp"></a><span data-ttu-id="1ba64-103">更新 macOsVppApp</span><span class="sxs-lookup"><span data-stu-id="1ba64-103">Update macOsVppApp</span></span>

<span data-ttu-id="1ba64-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ba64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ba64-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1ba64-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ba64-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1ba64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ba64-107">更新 [macOsVppApp 对象](../resources/intune-apps-macosvppapp.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="1ba64-107">Update the properties of a [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ba64-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1ba64-108">Prerequisites</span></span>
<span data-ttu-id="1ba64-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ba64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ba64-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ba64-111">Permission type</span></span>|<span data-ttu-id="1ba64-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ba64-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ba64-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ba64-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ba64-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ba64-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1ba64-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ba64-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ba64-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ba64-116">Not supported.</span></span>|
|<span data-ttu-id="1ba64-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ba64-117">Application</span></span>|<span data-ttu-id="1ba64-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ba64-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ba64-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ba64-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="1ba64-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ba64-120">Request headers</span></span>
|<span data-ttu-id="1ba64-121">标头</span><span class="sxs-lookup"><span data-stu-id="1ba64-121">Header</span></span>|<span data-ttu-id="1ba64-122">值</span><span class="sxs-lookup"><span data-stu-id="1ba64-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ba64-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ba64-123">Authorization</span></span>|<span data-ttu-id="1ba64-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1ba64-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ba64-125">接受</span><span class="sxs-lookup"><span data-stu-id="1ba64-125">Accept</span></span>|<span data-ttu-id="1ba64-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ba64-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ba64-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ba64-127">Request body</span></span>
<span data-ttu-id="1ba64-128">在请求正文中，提供 [macOsVppApp](../resources/intune-apps-macosvppapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ba64-128">In the request body, supply a JSON representation for the [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

<span data-ttu-id="1ba64-129">下表显示创建 [macOsVppApp](../resources/intune-apps-macosvppapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1ba64-129">The following table shows the properties that are required when you create the [macOsVppApp](../resources/intune-apps-macosvppapp.md).</span></span>

|<span data-ttu-id="1ba64-130">属性</span><span class="sxs-lookup"><span data-stu-id="1ba64-130">Property</span></span>|<span data-ttu-id="1ba64-131">类型</span><span class="sxs-lookup"><span data-stu-id="1ba64-131">Type</span></span>|<span data-ttu-id="1ba64-132">说明</span><span class="sxs-lookup"><span data-stu-id="1ba64-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ba64-133">id</span><span class="sxs-lookup"><span data-stu-id="1ba64-133">id</span></span>|<span data-ttu-id="1ba64-134">String</span><span class="sxs-lookup"><span data-stu-id="1ba64-134">String</span></span>|<span data-ttu-id="1ba64-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1ba64-135">Key of the entity.</span></span> <span data-ttu-id="1ba64-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1ba64-137">displayName</span></span>|<span data-ttu-id="1ba64-138">String</span><span class="sxs-lookup"><span data-stu-id="1ba64-138">String</span></span>|<span data-ttu-id="1ba64-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="1ba64-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1ba64-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-141">说明</span><span class="sxs-lookup"><span data-stu-id="1ba64-141">description</span></span>|<span data-ttu-id="1ba64-142">String</span><span class="sxs-lookup"><span data-stu-id="1ba64-142">String</span></span>|<span data-ttu-id="1ba64-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="1ba64-143">The description of the app.</span></span> <span data-ttu-id="1ba64-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-145">publisher</span><span class="sxs-lookup"><span data-stu-id="1ba64-145">publisher</span></span>|<span data-ttu-id="1ba64-146">String</span><span class="sxs-lookup"><span data-stu-id="1ba64-146">String</span></span>|<span data-ttu-id="1ba64-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="1ba64-147">The publisher of the app.</span></span> <span data-ttu-id="1ba64-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1ba64-149">largeIcon</span></span>|[<span data-ttu-id="1ba64-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1ba64-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1ba64-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="1ba64-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1ba64-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ba64-153">createdDateTime</span></span>|<span data-ttu-id="1ba64-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ba64-154">DateTimeOffset</span></span>|<span data-ttu-id="1ba64-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1ba64-155">The date and time the app was created.</span></span> <span data-ttu-id="1ba64-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ba64-157">lastModifiedDateTime</span></span>|<span data-ttu-id="1ba64-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ba64-158">DateTimeOffset</span></span>|<span data-ttu-id="1ba64-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1ba64-159">The date and time the app was last modified.</span></span> <span data-ttu-id="1ba64-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1ba64-161">isFeatured</span></span>|<span data-ttu-id="1ba64-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ba64-162">Boolean</span></span>|<span data-ttu-id="1ba64-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1ba64-164">privacyInformationUrl</span></span>|<span data-ttu-id="1ba64-165">String</span><span class="sxs-lookup"><span data-stu-id="1ba64-165">String</span></span>|<span data-ttu-id="1ba64-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="1ba64-166">The privacy statement Url.</span></span> <span data-ttu-id="1ba64-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1ba64-168">informationUrl</span></span>|<span data-ttu-id="1ba64-169">String</span><span class="sxs-lookup"><span data-stu-id="1ba64-169">String</span></span>|<span data-ttu-id="1ba64-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="1ba64-170">The more information Url.</span></span> <span data-ttu-id="1ba64-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-172">owner</span><span class="sxs-lookup"><span data-stu-id="1ba64-172">owner</span></span>|<span data-ttu-id="1ba64-173">String</span><span class="sxs-lookup"><span data-stu-id="1ba64-173">String</span></span>|<span data-ttu-id="1ba64-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="1ba64-174">The owner of the app.</span></span> <span data-ttu-id="1ba64-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-176">developer</span><span class="sxs-lookup"><span data-stu-id="1ba64-176">developer</span></span>|<span data-ttu-id="1ba64-177">String</span><span class="sxs-lookup"><span data-stu-id="1ba64-177">String</span></span>|<span data-ttu-id="1ba64-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="1ba64-178">The developer of the app.</span></span> <span data-ttu-id="1ba64-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-180">notes</span><span class="sxs-lookup"><span data-stu-id="1ba64-180">notes</span></span>|<span data-ttu-id="1ba64-181">String</span><span class="sxs-lookup"><span data-stu-id="1ba64-181">String</span></span>|<span data-ttu-id="1ba64-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="1ba64-182">Notes for the app.</span></span> <span data-ttu-id="1ba64-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="1ba64-184">uploadState</span></span>|<span data-ttu-id="1ba64-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1ba64-185">Int32</span></span>|<span data-ttu-id="1ba64-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="1ba64-186">The upload state.</span></span> <span data-ttu-id="1ba64-187">可能的值是：0 - `Not Ready` 、1 - `Ready` 、2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="1ba64-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="1ba64-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="1ba64-189">publishingState</span></span>|[<span data-ttu-id="1ba64-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1ba64-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1ba64-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="1ba64-191">The publishing state for the app.</span></span> <span data-ttu-id="1ba64-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="1ba64-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1ba64-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="1ba64-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="1ba64-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="1ba64-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1ba64-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1ba64-195">isAssigned</span></span>|<span data-ttu-id="1ba64-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ba64-196">Boolean</span></span>|<span data-ttu-id="1ba64-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="1ba64-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1ba64-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1ba64-199">roleScopeTagIds</span></span>|<span data-ttu-id="1ba64-200">String collection</span><span class="sxs-lookup"><span data-stu-id="1ba64-200">String collection</span></span>|<span data-ttu-id="1ba64-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="1ba64-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1ba64-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="1ba64-203">dependentAppCount</span></span>|<span data-ttu-id="1ba64-204">Int32</span><span class="sxs-lookup"><span data-stu-id="1ba64-204">Int32</span></span>|<span data-ttu-id="1ba64-205">子应用具有的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="1ba64-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="1ba64-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="1ba64-207">supersedingAppCount</span></span>|<span data-ttu-id="1ba64-208">Int32</span><span class="sxs-lookup"><span data-stu-id="1ba64-208">Int32</span></span>|<span data-ttu-id="1ba64-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="1ba64-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="1ba64-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="1ba64-211">supersededAppCount</span></span>|<span data-ttu-id="1ba64-212">Int32</span><span class="sxs-lookup"><span data-stu-id="1ba64-212">Int32</span></span>|<span data-ttu-id="1ba64-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="1ba64-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="1ba64-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ba64-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ba64-215">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1ba64-215">usedLicenseCount</span></span>|<span data-ttu-id="1ba64-216">Int32</span><span class="sxs-lookup"><span data-stu-id="1ba64-216">Int32</span></span>|<span data-ttu-id="1ba64-217">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="1ba64-217">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="1ba64-218">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1ba64-218">totalLicenseCount</span></span>|<span data-ttu-id="1ba64-219">Int32</span><span class="sxs-lookup"><span data-stu-id="1ba64-219">Int32</span></span>|<span data-ttu-id="1ba64-220">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="1ba64-220">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="1ba64-221">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="1ba64-221">releaseDateTime</span></span>|<span data-ttu-id="1ba64-222">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ba64-222">DateTimeOffset</span></span>|<span data-ttu-id="1ba64-223">VPP 应用程序的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1ba64-223">The VPP application release date and time.</span></span>|
|<span data-ttu-id="1ba64-224">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1ba64-224">appStoreUrl</span></span>|<span data-ttu-id="1ba64-225">String</span><span class="sxs-lookup"><span data-stu-id="1ba64-225">String</span></span>|<span data-ttu-id="1ba64-226">存储 URL。</span><span class="sxs-lookup"><span data-stu-id="1ba64-226">The store URL.</span></span>|
|<span data-ttu-id="1ba64-227">licensingType</span><span class="sxs-lookup"><span data-stu-id="1ba64-227">licensingType</span></span>|[<span data-ttu-id="1ba64-228">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="1ba64-228">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="1ba64-229">受支持的许可证类型。</span><span class="sxs-lookup"><span data-stu-id="1ba64-229">The supported License Type.</span></span>|
|<span data-ttu-id="1ba64-230">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="1ba64-230">vppTokenOrganizationName</span></span>|<span data-ttu-id="1ba64-231">String</span><span class="sxs-lookup"><span data-stu-id="1ba64-231">String</span></span>|<span data-ttu-id="1ba64-232">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="1ba64-232">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="1ba64-233">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="1ba64-233">vppTokenAccountType</span></span>|[<span data-ttu-id="1ba64-234">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="1ba64-234">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="1ba64-235">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="1ba64-235">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="1ba64-236">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="1ba64-236">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="1ba64-237">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="1ba64-237">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="1ba64-238">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="1ba64-238">vppTokenAppleId</span></span>|<span data-ttu-id="1ba64-239">String</span><span class="sxs-lookup"><span data-stu-id="1ba64-239">String</span></span>|<span data-ttu-id="1ba64-240">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="1ba64-240">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="1ba64-241">bundleId</span><span class="sxs-lookup"><span data-stu-id="1ba64-241">bundleId</span></span>|<span data-ttu-id="1ba64-242">String</span><span class="sxs-lookup"><span data-stu-id="1ba64-242">String</span></span>|<span data-ttu-id="1ba64-243">标识名称。</span><span class="sxs-lookup"><span data-stu-id="1ba64-243">The Identity Name.</span></span>|
|<span data-ttu-id="1ba64-244">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="1ba64-244">vppTokenId</span></span>|<span data-ttu-id="1ba64-245">String</span><span class="sxs-lookup"><span data-stu-id="1ba64-245">String</span></span>|<span data-ttu-id="1ba64-246">与此应用关联的 VPP 令牌的标识符。</span><span class="sxs-lookup"><span data-stu-id="1ba64-246">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="1ba64-247">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="1ba64-247">revokeLicenseActionResults</span></span>|<span data-ttu-id="1ba64-248">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ba64-248">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="1ba64-249">撤销此应用许可证操作的结果。</span><span class="sxs-lookup"><span data-stu-id="1ba64-249">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="1ba64-250">响应</span><span class="sxs-lookup"><span data-stu-id="1ba64-250">Response</span></span>
<span data-ttu-id="1ba64-251">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [macOsVppApp](../resources/intune-apps-macosvppapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1ba64-251">If successful, this method returns a `200 OK` response code and an updated [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ba64-252">示例</span><span class="sxs-lookup"><span data-stu-id="1ba64-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ba64-253">请求</span><span class="sxs-lookup"><span data-stu-id="1ba64-253">Request</span></span>
<span data-ttu-id="1ba64-254">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ba64-254">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1926

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1ba64-255">响应</span><span class="sxs-lookup"><span data-stu-id="1ba64-255">Response</span></span>
<span data-ttu-id="1ba64-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1ba64-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2098

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
  "id": "10b95265-5265-10b9-6552-b9106552b910",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```




