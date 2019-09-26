---
title: 更新 microsoftStoreForBusinessApp
description: 更新 microsoftStoreForBusinessApp 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a1d42ce964e05f8822a19243788ce41da28b5301
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37177267"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="cb063-103">更新 microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="cb063-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="cb063-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cb063-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb063-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cb063-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb063-106">更新 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cb063-106">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb063-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cb063-107">Prerequisites</span></span>
<span data-ttu-id="cb063-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb063-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb063-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb063-110">Permission type</span></span>|<span data-ttu-id="cb063-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cb063-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb063-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb063-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb063-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb063-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cb063-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb063-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb063-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb063-115">Not supported.</span></span>|
|<span data-ttu-id="cb063-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb063-116">Application</span></span>|<span data-ttu-id="cb063-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb063-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb063-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb063-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="cb063-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb063-119">Request headers</span></span>
|<span data-ttu-id="cb063-120">标头</span><span class="sxs-lookup"><span data-stu-id="cb063-120">Header</span></span>|<span data-ttu-id="cb063-121">值</span><span class="sxs-lookup"><span data-stu-id="cb063-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb063-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb063-122">Authorization</span></span>|<span data-ttu-id="cb063-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cb063-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb063-124">接受</span><span class="sxs-lookup"><span data-stu-id="cb063-124">Accept</span></span>|<span data-ttu-id="cb063-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cb063-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb063-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb063-126">Request body</span></span>
<span data-ttu-id="cb063-127">在请求正文中，提供 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb063-127">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="cb063-128">下表显示了创建 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cb063-128">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="cb063-129">属性</span><span class="sxs-lookup"><span data-stu-id="cb063-129">Property</span></span>|<span data-ttu-id="cb063-130">类型</span><span class="sxs-lookup"><span data-stu-id="cb063-130">Type</span></span>|<span data-ttu-id="cb063-131">说明</span><span class="sxs-lookup"><span data-stu-id="cb063-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb063-132">id</span><span class="sxs-lookup"><span data-stu-id="cb063-132">id</span></span>|<span data-ttu-id="cb063-133">字符串</span><span class="sxs-lookup"><span data-stu-id="cb063-133">String</span></span>|<span data-ttu-id="cb063-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cb063-134">Key of the entity.</span></span> <span data-ttu-id="cb063-135">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb063-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb063-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cb063-136">displayName</span></span>|<span data-ttu-id="cb063-137">String</span><span class="sxs-lookup"><span data-stu-id="cb063-137">String</span></span>|<span data-ttu-id="cb063-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="cb063-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cb063-139">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb063-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb063-140">说明</span><span class="sxs-lookup"><span data-stu-id="cb063-140">description</span></span>|<span data-ttu-id="cb063-141">String</span><span class="sxs-lookup"><span data-stu-id="cb063-141">String</span></span>|<span data-ttu-id="cb063-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="cb063-142">The description of the app.</span></span> <span data-ttu-id="cb063-143">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb063-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb063-144">publisher</span><span class="sxs-lookup"><span data-stu-id="cb063-144">publisher</span></span>|<span data-ttu-id="cb063-145">String</span><span class="sxs-lookup"><span data-stu-id="cb063-145">String</span></span>|<span data-ttu-id="cb063-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="cb063-146">The publisher of the app.</span></span> <span data-ttu-id="cb063-147">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb063-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb063-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cb063-148">largeIcon</span></span>|[<span data-ttu-id="cb063-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cb063-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cb063-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="cb063-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cb063-151">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb063-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb063-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb063-152">createdDateTime</span></span>|<span data-ttu-id="cb063-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb063-153">DateTimeOffset</span></span>|<span data-ttu-id="cb063-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cb063-154">The date and time the app was created.</span></span> <span data-ttu-id="cb063-155">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb063-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb063-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb063-156">lastModifiedDateTime</span></span>|<span data-ttu-id="cb063-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb063-157">DateTimeOffset</span></span>|<span data-ttu-id="cb063-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cb063-158">The date and time the app was last modified.</span></span> <span data-ttu-id="cb063-159">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb063-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb063-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cb063-160">isFeatured</span></span>|<span data-ttu-id="cb063-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb063-161">Boolean</span></span>|<span data-ttu-id="cb063-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb063-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb063-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cb063-163">privacyInformationUrl</span></span>|<span data-ttu-id="cb063-164">String</span><span class="sxs-lookup"><span data-stu-id="cb063-164">String</span></span>|<span data-ttu-id="cb063-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="cb063-165">The privacy statement Url.</span></span> <span data-ttu-id="cb063-166">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb063-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb063-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cb063-167">informationUrl</span></span>|<span data-ttu-id="cb063-168">String</span><span class="sxs-lookup"><span data-stu-id="cb063-168">String</span></span>|<span data-ttu-id="cb063-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="cb063-169">The more information Url.</span></span> <span data-ttu-id="cb063-170">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb063-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb063-171">owner</span><span class="sxs-lookup"><span data-stu-id="cb063-171">owner</span></span>|<span data-ttu-id="cb063-172">String</span><span class="sxs-lookup"><span data-stu-id="cb063-172">String</span></span>|<span data-ttu-id="cb063-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="cb063-173">The owner of the app.</span></span> <span data-ttu-id="cb063-174">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb063-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb063-175">developer</span><span class="sxs-lookup"><span data-stu-id="cb063-175">developer</span></span>|<span data-ttu-id="cb063-176">String</span><span class="sxs-lookup"><span data-stu-id="cb063-176">String</span></span>|<span data-ttu-id="cb063-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="cb063-177">The developer of the app.</span></span> <span data-ttu-id="cb063-178">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb063-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb063-179">notes</span><span class="sxs-lookup"><span data-stu-id="cb063-179">notes</span></span>|<span data-ttu-id="cb063-180">String</span><span class="sxs-lookup"><span data-stu-id="cb063-180">String</span></span>|<span data-ttu-id="cb063-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="cb063-181">Notes for the app.</span></span> <span data-ttu-id="cb063-182">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb063-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb063-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="cb063-183">uploadState</span></span>|<span data-ttu-id="cb063-184">Int32</span><span class="sxs-lookup"><span data-stu-id="cb063-184">Int32</span></span>|<span data-ttu-id="cb063-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="cb063-185">The upload state.</span></span> <span data-ttu-id="cb063-186">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb063-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb063-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="cb063-187">publishingState</span></span>|[<span data-ttu-id="cb063-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cb063-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cb063-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="cb063-189">The publishing state for the app.</span></span> <span data-ttu-id="cb063-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="cb063-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cb063-191">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="cb063-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="cb063-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="cb063-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cb063-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="cb063-193">isAssigned</span></span>|<span data-ttu-id="cb063-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb063-194">Boolean</span></span>|<span data-ttu-id="cb063-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="cb063-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="cb063-196">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb063-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb063-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cb063-197">roleScopeTagIds</span></span>|<span data-ttu-id="cb063-198">String collection</span><span class="sxs-lookup"><span data-stu-id="cb063-198">String collection</span></span>|<span data-ttu-id="cb063-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="cb063-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="cb063-200">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb063-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb063-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="cb063-201">dependentAppCount</span></span>|<span data-ttu-id="cb063-202">Int32</span><span class="sxs-lookup"><span data-stu-id="cb063-202">Int32</span></span>|<span data-ttu-id="cb063-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="cb063-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="cb063-204">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb063-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb063-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="cb063-205">usedLicenseCount</span></span>|<span data-ttu-id="cb063-206">Int32</span><span class="sxs-lookup"><span data-stu-id="cb063-206">Int32</span></span>|<span data-ttu-id="cb063-207">使用中的适用于企业的 Microsoft Store 许可证数。</span><span class="sxs-lookup"><span data-stu-id="cb063-207">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="cb063-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="cb063-208">totalLicenseCount</span></span>|<span data-ttu-id="cb063-209">Int32</span><span class="sxs-lookup"><span data-stu-id="cb063-209">Int32</span></span>|<span data-ttu-id="cb063-210">适用于企业的 Microsoft Store 许可证总数。</span><span class="sxs-lookup"><span data-stu-id="cb063-210">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="cb063-211">productKey</span><span class="sxs-lookup"><span data-stu-id="cb063-211">productKey</span></span>|<span data-ttu-id="cb063-212">字符串</span><span class="sxs-lookup"><span data-stu-id="cb063-212">String</span></span>|<span data-ttu-id="cb063-213">应用产品密钥</span><span class="sxs-lookup"><span data-stu-id="cb063-213">The app product key</span></span>|
|<span data-ttu-id="cb063-214">licenseType</span><span class="sxs-lookup"><span data-stu-id="cb063-214">licenseType</span></span>|[<span data-ttu-id="cb063-215">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="cb063-215">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="cb063-216">应用程序许可证类型。</span><span class="sxs-lookup"><span data-stu-id="cb063-216">The app license type.</span></span> <span data-ttu-id="cb063-217">可取值为：`offline`、`online`。</span><span class="sxs-lookup"><span data-stu-id="cb063-217">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="cb063-218">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="cb063-218">packageIdentityName</span></span>|<span data-ttu-id="cb063-219">String</span><span class="sxs-lookup"><span data-stu-id="cb063-219">String</span></span>|<span data-ttu-id="cb063-220">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="cb063-220">The app package identifier</span></span>|
|<span data-ttu-id="cb063-221">licensingType</span><span class="sxs-lookup"><span data-stu-id="cb063-221">licensingType</span></span>|[<span data-ttu-id="cb063-222">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="cb063-222">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="cb063-223">受支持的许可证类型。</span><span class="sxs-lookup"><span data-stu-id="cb063-223">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="cb063-224">响应</span><span class="sxs-lookup"><span data-stu-id="cb063-224">Response</span></span>
<span data-ttu-id="cb063-225">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cb063-225">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb063-226">示例</span><span class="sxs-lookup"><span data-stu-id="cb063-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb063-227">请求</span><span class="sxs-lookup"><span data-stu-id="cb063-227">Request</span></span>
<span data-ttu-id="cb063-228">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cb063-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1132

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```

### <a name="response"></a><span data-ttu-id="cb063-229">响应</span><span class="sxs-lookup"><span data-stu-id="cb063-229">Response</span></span>
<span data-ttu-id="cb063-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cb063-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1304

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```




