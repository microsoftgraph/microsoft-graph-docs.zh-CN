---
title: 更新 iosVppApp
description: 更新 iosVppApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f7d3f27c4304fa7b2becd5ed3db4801b80a3c963
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43416728"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="06ed3-103">更新 iosVppApp</span><span class="sxs-lookup"><span data-stu-id="06ed3-103">Update iosVppApp</span></span>

<span data-ttu-id="06ed3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06ed3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06ed3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="06ed3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06ed3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06ed3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06ed3-107">更新 [iosVppApp](../resources/intune-apps-iosvppapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="06ed3-107">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06ed3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="06ed3-108">Prerequisites</span></span>
<span data-ttu-id="06ed3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06ed3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06ed3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="06ed3-111">Permission type</span></span>|<span data-ttu-id="06ed3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="06ed3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06ed3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06ed3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06ed3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06ed3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="06ed3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06ed3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06ed3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="06ed3-116">Not supported.</span></span>|
|<span data-ttu-id="06ed3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="06ed3-117">Application</span></span>|<span data-ttu-id="06ed3-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06ed3-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06ed3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06ed3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="06ed3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="06ed3-120">Request headers</span></span>
|<span data-ttu-id="06ed3-121">标头</span><span class="sxs-lookup"><span data-stu-id="06ed3-121">Header</span></span>|<span data-ttu-id="06ed3-122">值</span><span class="sxs-lookup"><span data-stu-id="06ed3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06ed3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06ed3-123">Authorization</span></span>|<span data-ttu-id="06ed3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="06ed3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06ed3-125">接受</span><span class="sxs-lookup"><span data-stu-id="06ed3-125">Accept</span></span>|<span data-ttu-id="06ed3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06ed3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06ed3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="06ed3-127">Request body</span></span>
<span data-ttu-id="06ed3-128">在请求正文中，提供 [iosVppApp](../resources/intune-apps-iosvppapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06ed3-128">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="06ed3-129">下表显示了创建 [iosVppApp](../resources/intune-apps-iosvppapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="06ed3-129">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="06ed3-130">属性</span><span class="sxs-lookup"><span data-stu-id="06ed3-130">Property</span></span>|<span data-ttu-id="06ed3-131">类型</span><span class="sxs-lookup"><span data-stu-id="06ed3-131">Type</span></span>|<span data-ttu-id="06ed3-132">说明</span><span class="sxs-lookup"><span data-stu-id="06ed3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06ed3-133">id</span><span class="sxs-lookup"><span data-stu-id="06ed3-133">id</span></span>|<span data-ttu-id="06ed3-134">字符串</span><span class="sxs-lookup"><span data-stu-id="06ed3-134">String</span></span>|<span data-ttu-id="06ed3-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="06ed3-135">Key of the entity.</span></span> <span data-ttu-id="06ed3-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ed3-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06ed3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="06ed3-137">displayName</span></span>|<span data-ttu-id="06ed3-138">String</span><span class="sxs-lookup"><span data-stu-id="06ed3-138">String</span></span>|<span data-ttu-id="06ed3-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="06ed3-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="06ed3-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ed3-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06ed3-141">description</span><span class="sxs-lookup"><span data-stu-id="06ed3-141">description</span></span>|<span data-ttu-id="06ed3-142">字符串</span><span class="sxs-lookup"><span data-stu-id="06ed3-142">String</span></span>|<span data-ttu-id="06ed3-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="06ed3-143">The description of the app.</span></span> <span data-ttu-id="06ed3-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ed3-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06ed3-145">publisher</span><span class="sxs-lookup"><span data-stu-id="06ed3-145">publisher</span></span>|<span data-ttu-id="06ed3-146">String</span><span class="sxs-lookup"><span data-stu-id="06ed3-146">String</span></span>|<span data-ttu-id="06ed3-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="06ed3-147">The publisher of the app.</span></span> <span data-ttu-id="06ed3-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ed3-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06ed3-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="06ed3-149">largeIcon</span></span>|[<span data-ttu-id="06ed3-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="06ed3-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="06ed3-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="06ed3-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="06ed3-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ed3-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06ed3-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06ed3-153">createdDateTime</span></span>|<span data-ttu-id="06ed3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06ed3-154">DateTimeOffset</span></span>|<span data-ttu-id="06ed3-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="06ed3-155">The date and time the app was created.</span></span> <span data-ttu-id="06ed3-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ed3-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06ed3-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06ed3-157">lastModifiedDateTime</span></span>|<span data-ttu-id="06ed3-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06ed3-158">DateTimeOffset</span></span>|<span data-ttu-id="06ed3-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="06ed3-159">The date and time the app was last modified.</span></span> <span data-ttu-id="06ed3-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ed3-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06ed3-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="06ed3-161">isFeatured</span></span>|<span data-ttu-id="06ed3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="06ed3-162">Boolean</span></span>|<span data-ttu-id="06ed3-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ed3-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06ed3-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="06ed3-164">privacyInformationUrl</span></span>|<span data-ttu-id="06ed3-165">String</span><span class="sxs-lookup"><span data-stu-id="06ed3-165">String</span></span>|<span data-ttu-id="06ed3-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="06ed3-166">The privacy statement Url.</span></span> <span data-ttu-id="06ed3-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ed3-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06ed3-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="06ed3-168">informationUrl</span></span>|<span data-ttu-id="06ed3-169">String</span><span class="sxs-lookup"><span data-stu-id="06ed3-169">String</span></span>|<span data-ttu-id="06ed3-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="06ed3-170">The more information Url.</span></span> <span data-ttu-id="06ed3-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ed3-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06ed3-172">owner</span><span class="sxs-lookup"><span data-stu-id="06ed3-172">owner</span></span>|<span data-ttu-id="06ed3-173">String</span><span class="sxs-lookup"><span data-stu-id="06ed3-173">String</span></span>|<span data-ttu-id="06ed3-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="06ed3-174">The owner of the app.</span></span> <span data-ttu-id="06ed3-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ed3-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06ed3-176">developer</span><span class="sxs-lookup"><span data-stu-id="06ed3-176">developer</span></span>|<span data-ttu-id="06ed3-177">String</span><span class="sxs-lookup"><span data-stu-id="06ed3-177">String</span></span>|<span data-ttu-id="06ed3-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="06ed3-178">The developer of the app.</span></span> <span data-ttu-id="06ed3-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ed3-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06ed3-180">notes</span><span class="sxs-lookup"><span data-stu-id="06ed3-180">notes</span></span>|<span data-ttu-id="06ed3-181">String</span><span class="sxs-lookup"><span data-stu-id="06ed3-181">String</span></span>|<span data-ttu-id="06ed3-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="06ed3-182">Notes for the app.</span></span> <span data-ttu-id="06ed3-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ed3-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06ed3-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="06ed3-184">uploadState</span></span>|<span data-ttu-id="06ed3-185">Int32</span><span class="sxs-lookup"><span data-stu-id="06ed3-185">Int32</span></span>|<span data-ttu-id="06ed3-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="06ed3-186">The upload state.</span></span> <span data-ttu-id="06ed3-187">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ed3-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06ed3-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="06ed3-188">publishingState</span></span>|[<span data-ttu-id="06ed3-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="06ed3-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="06ed3-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="06ed3-190">The publishing state for the app.</span></span> <span data-ttu-id="06ed3-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="06ed3-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="06ed3-192">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="06ed3-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="06ed3-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="06ed3-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="06ed3-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="06ed3-194">isAssigned</span></span>|<span data-ttu-id="06ed3-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="06ed3-195">Boolean</span></span>|<span data-ttu-id="06ed3-196">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="06ed3-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="06ed3-197">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ed3-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06ed3-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="06ed3-198">roleScopeTagIds</span></span>|<span data-ttu-id="06ed3-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="06ed3-199">String collection</span></span>|<span data-ttu-id="06ed3-200">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="06ed3-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="06ed3-201">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ed3-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06ed3-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="06ed3-202">dependentAppCount</span></span>|<span data-ttu-id="06ed3-203">Int32</span><span class="sxs-lookup"><span data-stu-id="06ed3-203">Int32</span></span>|<span data-ttu-id="06ed3-204">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="06ed3-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="06ed3-205">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ed3-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06ed3-206">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="06ed3-206">usedLicenseCount</span></span>|<span data-ttu-id="06ed3-207">Int32</span><span class="sxs-lookup"><span data-stu-id="06ed3-207">Int32</span></span>|<span data-ttu-id="06ed3-208">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="06ed3-208">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="06ed3-209">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="06ed3-209">totalLicenseCount</span></span>|<span data-ttu-id="06ed3-210">Int32</span><span class="sxs-lookup"><span data-stu-id="06ed3-210">Int32</span></span>|<span data-ttu-id="06ed3-211">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="06ed3-211">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="06ed3-212">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="06ed3-212">releaseDateTime</span></span>|<span data-ttu-id="06ed3-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06ed3-213">DateTimeOffset</span></span>|<span data-ttu-id="06ed3-214">VPP 应用程序的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="06ed3-214">The VPP application release date and time.</span></span>|
|<span data-ttu-id="06ed3-215">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="06ed3-215">appStoreUrl</span></span>|<span data-ttu-id="06ed3-216">String</span><span class="sxs-lookup"><span data-stu-id="06ed3-216">String</span></span>|<span data-ttu-id="06ed3-217">存储 URL。</span><span class="sxs-lookup"><span data-stu-id="06ed3-217">The store URL.</span></span>|
|<span data-ttu-id="06ed3-218">licensingType</span><span class="sxs-lookup"><span data-stu-id="06ed3-218">licensingType</span></span>|[<span data-ttu-id="06ed3-219">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="06ed3-219">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="06ed3-220">受支持的许可证类型。</span><span class="sxs-lookup"><span data-stu-id="06ed3-220">The supported License Type.</span></span>|
|<span data-ttu-id="06ed3-221">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="06ed3-221">applicableDeviceType</span></span>|[<span data-ttu-id="06ed3-222">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="06ed3-222">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="06ed3-223">适用的 iOS 设备类型。</span><span class="sxs-lookup"><span data-stu-id="06ed3-223">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="06ed3-224">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="06ed3-224">vppTokenOrganizationName</span></span>|<span data-ttu-id="06ed3-225">String</span><span class="sxs-lookup"><span data-stu-id="06ed3-225">String</span></span>|<span data-ttu-id="06ed3-226">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="06ed3-226">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="06ed3-227">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="06ed3-227">vppTokenAccountType</span></span>|[<span data-ttu-id="06ed3-228">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="06ed3-228">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="06ed3-229">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="06ed3-229">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="06ed3-230">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="06ed3-230">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="06ed3-231">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="06ed3-231">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="06ed3-232">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="06ed3-232">vppTokenAppleId</span></span>|<span data-ttu-id="06ed3-233">String</span><span class="sxs-lookup"><span data-stu-id="06ed3-233">String</span></span>|<span data-ttu-id="06ed3-234">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="06ed3-234">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="06ed3-235">bundleId</span><span class="sxs-lookup"><span data-stu-id="06ed3-235">bundleId</span></span>|<span data-ttu-id="06ed3-236">String</span><span class="sxs-lookup"><span data-stu-id="06ed3-236">String</span></span>|<span data-ttu-id="06ed3-237">标识名称。</span><span class="sxs-lookup"><span data-stu-id="06ed3-237">The Identity Name.</span></span>|
|<span data-ttu-id="06ed3-238">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="06ed3-238">vppTokenId</span></span>|<span data-ttu-id="06ed3-239">String</span><span class="sxs-lookup"><span data-stu-id="06ed3-239">String</span></span>|<span data-ttu-id="06ed3-240">与此应用程序关联的 VPP 令牌的标识符。</span><span class="sxs-lookup"><span data-stu-id="06ed3-240">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="06ed3-241">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="06ed3-241">revokeLicenseActionResults</span></span>|<span data-ttu-id="06ed3-242">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="06ed3-242">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="06ed3-243">对此应用吊销许可证操作的结果。</span><span class="sxs-lookup"><span data-stu-id="06ed3-243">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="06ed3-244">响应</span><span class="sxs-lookup"><span data-stu-id="06ed3-244">Response</span></span>
<span data-ttu-id="06ed3-245">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppApp](../resources/intune-apps-iosvppapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06ed3-245">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06ed3-246">示例</span><span class="sxs-lookup"><span data-stu-id="06ed3-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="06ed3-247">请求</span><span class="sxs-lookup"><span data-stu-id="06ed3-247">Request</span></span>
<span data-ttu-id="06ed3-248">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="06ed3-248">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1999

{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
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

### <a name="response"></a><span data-ttu-id="06ed3-249">响应</span><span class="sxs-lookup"><span data-stu-id="06ed3-249">Response</span></span>
<span data-ttu-id="06ed3-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="06ed3-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2171

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
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



