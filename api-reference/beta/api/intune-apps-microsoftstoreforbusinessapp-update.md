---
title: 更新 microsoftStoreForBusinessApp
description: 更新 microsoftStoreForBusinessApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 44e6d282610f2cd836689a6d68d77e33714ae20b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32490981"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="2e443-103">更新 microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="2e443-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="2e443-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2e443-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e443-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2e443-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e443-106">更新 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2e443-106">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e443-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2e443-107">Prerequisites</span></span>
<span data-ttu-id="2e443-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e443-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e443-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e443-110">Permission type</span></span>|<span data-ttu-id="2e443-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2e443-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e443-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e443-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2e443-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e443-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2e443-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e443-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e443-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e443-115">Not supported.</span></span>|
|<span data-ttu-id="2e443-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e443-116">Application</span></span>|<span data-ttu-id="2e443-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e443-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e443-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e443-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="2e443-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e443-119">Request headers</span></span>
|<span data-ttu-id="2e443-120">标头</span><span class="sxs-lookup"><span data-stu-id="2e443-120">Header</span></span>|<span data-ttu-id="2e443-121">值</span><span class="sxs-lookup"><span data-stu-id="2e443-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e443-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e443-122">Authorization</span></span>|<span data-ttu-id="2e443-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2e443-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e443-124">接受</span><span class="sxs-lookup"><span data-stu-id="2e443-124">Accept</span></span>|<span data-ttu-id="2e443-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2e443-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e443-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e443-126">Request body</span></span>
<span data-ttu-id="2e443-127">在请求正文中，提供 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e443-127">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="2e443-128">下表显示了创建 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2e443-128">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="2e443-129">属性</span><span class="sxs-lookup"><span data-stu-id="2e443-129">Property</span></span>|<span data-ttu-id="2e443-130">类型</span><span class="sxs-lookup"><span data-stu-id="2e443-130">Type</span></span>|<span data-ttu-id="2e443-131">说明</span><span class="sxs-lookup"><span data-stu-id="2e443-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e443-132">id</span><span class="sxs-lookup"><span data-stu-id="2e443-132">id</span></span>|<span data-ttu-id="2e443-133">String</span><span class="sxs-lookup"><span data-stu-id="2e443-133">String</span></span>|<span data-ttu-id="2e443-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2e443-134">Key of the entity.</span></span> <span data-ttu-id="2e443-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e443-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e443-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2e443-136">displayName</span></span>|<span data-ttu-id="2e443-137">字符串</span><span class="sxs-lookup"><span data-stu-id="2e443-137">String</span></span>|<span data-ttu-id="2e443-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="2e443-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2e443-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e443-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e443-140">description</span><span class="sxs-lookup"><span data-stu-id="2e443-140">description</span></span>|<span data-ttu-id="2e443-141">字符串</span><span class="sxs-lookup"><span data-stu-id="2e443-141">String</span></span>|<span data-ttu-id="2e443-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="2e443-142">The description of the app.</span></span> <span data-ttu-id="2e443-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e443-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e443-144">publisher</span><span class="sxs-lookup"><span data-stu-id="2e443-144">publisher</span></span>|<span data-ttu-id="2e443-145">字符串</span><span class="sxs-lookup"><span data-stu-id="2e443-145">String</span></span>|<span data-ttu-id="2e443-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="2e443-146">The publisher of the app.</span></span> <span data-ttu-id="2e443-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e443-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e443-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2e443-148">largeIcon</span></span>|[<span data-ttu-id="2e443-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2e443-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2e443-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="2e443-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2e443-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e443-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e443-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2e443-152">createdDateTime</span></span>|<span data-ttu-id="2e443-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e443-153">DateTimeOffset</span></span>|<span data-ttu-id="2e443-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2e443-154">The date and time the app was created.</span></span> <span data-ttu-id="2e443-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e443-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e443-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e443-156">lastModifiedDateTime</span></span>|<span data-ttu-id="2e443-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e443-157">DateTimeOffset</span></span>|<span data-ttu-id="2e443-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2e443-158">The date and time the app was last modified.</span></span> <span data-ttu-id="2e443-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e443-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e443-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2e443-160">isFeatured</span></span>|<span data-ttu-id="2e443-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e443-161">Boolean</span></span>|<span data-ttu-id="2e443-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e443-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e443-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2e443-163">privacyInformationUrl</span></span>|<span data-ttu-id="2e443-164">字符串</span><span class="sxs-lookup"><span data-stu-id="2e443-164">String</span></span>|<span data-ttu-id="2e443-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="2e443-165">The privacy statement Url.</span></span> <span data-ttu-id="2e443-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e443-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e443-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2e443-167">informationUrl</span></span>|<span data-ttu-id="2e443-168">字符串</span><span class="sxs-lookup"><span data-stu-id="2e443-168">String</span></span>|<span data-ttu-id="2e443-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="2e443-169">The more information Url.</span></span> <span data-ttu-id="2e443-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e443-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e443-171">owner</span><span class="sxs-lookup"><span data-stu-id="2e443-171">owner</span></span>|<span data-ttu-id="2e443-172">字符串</span><span class="sxs-lookup"><span data-stu-id="2e443-172">String</span></span>|<span data-ttu-id="2e443-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="2e443-173">The owner of the app.</span></span> <span data-ttu-id="2e443-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e443-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e443-175">developer</span><span class="sxs-lookup"><span data-stu-id="2e443-175">developer</span></span>|<span data-ttu-id="2e443-176">字符串</span><span class="sxs-lookup"><span data-stu-id="2e443-176">String</span></span>|<span data-ttu-id="2e443-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="2e443-177">The developer of the app.</span></span> <span data-ttu-id="2e443-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e443-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e443-179">notes</span><span class="sxs-lookup"><span data-stu-id="2e443-179">notes</span></span>|<span data-ttu-id="2e443-180">字符串</span><span class="sxs-lookup"><span data-stu-id="2e443-180">String</span></span>|<span data-ttu-id="2e443-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="2e443-181">Notes for the app.</span></span> <span data-ttu-id="2e443-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e443-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e443-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="2e443-183">uploadState</span></span>|<span data-ttu-id="2e443-184">Int32</span><span class="sxs-lookup"><span data-stu-id="2e443-184">Int32</span></span>|<span data-ttu-id="2e443-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="2e443-185">The upload state.</span></span> <span data-ttu-id="2e443-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e443-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e443-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="2e443-187">publishingState</span></span>|[<span data-ttu-id="2e443-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2e443-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2e443-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="2e443-189">The publishing state for the app.</span></span> <span data-ttu-id="2e443-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="2e443-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2e443-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="2e443-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2e443-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="2e443-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2e443-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2e443-193">isAssigned</span></span>|<span data-ttu-id="2e443-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e443-194">Boolean</span></span>|<span data-ttu-id="2e443-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="2e443-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="2e443-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e443-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e443-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2e443-197">roleScopeTagIds</span></span>|<span data-ttu-id="2e443-198">String collection</span><span class="sxs-lookup"><span data-stu-id="2e443-198">String collection</span></span>|<span data-ttu-id="2e443-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="2e443-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="2e443-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e443-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e443-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="2e443-201">dependentAppCount</span></span>|<span data-ttu-id="2e443-202">Int32</span><span class="sxs-lookup"><span data-stu-id="2e443-202">Int32</span></span>|<span data-ttu-id="2e443-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="2e443-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="2e443-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2e443-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2e443-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2e443-205">usedLicenseCount</span></span>|<span data-ttu-id="2e443-206">Int32</span><span class="sxs-lookup"><span data-stu-id="2e443-206">Int32</span></span>|<span data-ttu-id="2e443-207">使用中的适用于企业的 Microsoft Store 许可证数。</span><span class="sxs-lookup"><span data-stu-id="2e443-207">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="2e443-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2e443-208">totalLicenseCount</span></span>|<span data-ttu-id="2e443-209">Int32</span><span class="sxs-lookup"><span data-stu-id="2e443-209">Int32</span></span>|<span data-ttu-id="2e443-210">适用于企业的 Microsoft Store 许可证总数。</span><span class="sxs-lookup"><span data-stu-id="2e443-210">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="2e443-211">productKey</span><span class="sxs-lookup"><span data-stu-id="2e443-211">productKey</span></span>|<span data-ttu-id="2e443-212">字串符号</span><span class="sxs-lookup"><span data-stu-id="2e443-212">String</span></span>|<span data-ttu-id="2e443-213">应用产品密钥</span><span class="sxs-lookup"><span data-stu-id="2e443-213">The app product key</span></span>|
|<span data-ttu-id="2e443-214">licenseType</span><span class="sxs-lookup"><span data-stu-id="2e443-214">licenseType</span></span>|[<span data-ttu-id="2e443-215">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="2e443-215">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="2e443-216">应用程序许可证类型。</span><span class="sxs-lookup"><span data-stu-id="2e443-216">The app license type.</span></span> <span data-ttu-id="2e443-217">可取值为：`offline`、`online`。</span><span class="sxs-lookup"><span data-stu-id="2e443-217">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="2e443-218">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="2e443-218">packageIdentityName</span></span>|<span data-ttu-id="2e443-219">String</span><span class="sxs-lookup"><span data-stu-id="2e443-219">String</span></span>|<span data-ttu-id="2e443-220">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="2e443-220">The app package identifier</span></span>|
|<span data-ttu-id="2e443-221">licensingType</span><span class="sxs-lookup"><span data-stu-id="2e443-221">licensingType</span></span>|[<span data-ttu-id="2e443-222">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="2e443-222">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="2e443-223">受支持的许可证类型。</span><span class="sxs-lookup"><span data-stu-id="2e443-223">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="2e443-224">响应</span><span class="sxs-lookup"><span data-stu-id="2e443-224">Response</span></span>
<span data-ttu-id="2e443-225">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2e443-225">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e443-226">示例</span><span class="sxs-lookup"><span data-stu-id="2e443-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e443-227">请求</span><span class="sxs-lookup"><span data-stu-id="2e443-227">Request</span></span>
<span data-ttu-id="2e443-228">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2e443-228">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2e443-229">响应</span><span class="sxs-lookup"><span data-stu-id="2e443-229">Response</span></span>
<span data-ttu-id="2e443-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2e443-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





