---
title: 更新 macOsVppApp
description: 更新 macOsVppApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b43aa666a5594f8352fb4db6c85f11dbec37d80a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970784"
---
# <a name="update-macosvppapp"></a><span data-ttu-id="4191e-103">更新 macOsVppApp</span><span class="sxs-lookup"><span data-stu-id="4191e-103">Update macOsVppApp</span></span>

> <span data-ttu-id="4191e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4191e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4191e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4191e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4191e-106">更新[macOsVppApp](../resources/intune-apps-macosvppapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4191e-106">Update the properties of a [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4191e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4191e-107">Prerequisites</span></span>
<span data-ttu-id="4191e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4191e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4191e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4191e-110">Permission type</span></span>|<span data-ttu-id="4191e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4191e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4191e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4191e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4191e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4191e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4191e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4191e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4191e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4191e-115">Not supported.</span></span>|
|<span data-ttu-id="4191e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4191e-116">Application</span></span>|<span data-ttu-id="4191e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4191e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4191e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4191e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4191e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4191e-119">Request headers</span></span>
|<span data-ttu-id="4191e-120">标头</span><span class="sxs-lookup"><span data-stu-id="4191e-120">Header</span></span>|<span data-ttu-id="4191e-121">值</span><span class="sxs-lookup"><span data-stu-id="4191e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4191e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4191e-122">Authorization</span></span>|<span data-ttu-id="4191e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4191e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4191e-124">接受</span><span class="sxs-lookup"><span data-stu-id="4191e-124">Accept</span></span>|<span data-ttu-id="4191e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4191e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4191e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4191e-126">Request body</span></span>
<span data-ttu-id="4191e-127">在请求正文中, 提供[macOsVppApp](../resources/intune-apps-macosvppapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4191e-127">In the request body, supply a JSON representation for the [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

<span data-ttu-id="4191e-128">下表显示创建[macOsVppApp](../resources/intune-apps-macosvppapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4191e-128">The following table shows the properties that are required when you create the [macOsVppApp](../resources/intune-apps-macosvppapp.md).</span></span>

|<span data-ttu-id="4191e-129">属性</span><span class="sxs-lookup"><span data-stu-id="4191e-129">Property</span></span>|<span data-ttu-id="4191e-130">类型</span><span class="sxs-lookup"><span data-stu-id="4191e-130">Type</span></span>|<span data-ttu-id="4191e-131">说明</span><span class="sxs-lookup"><span data-stu-id="4191e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4191e-132">id</span><span class="sxs-lookup"><span data-stu-id="4191e-132">id</span></span>|<span data-ttu-id="4191e-133">String</span><span class="sxs-lookup"><span data-stu-id="4191e-133">String</span></span>|<span data-ttu-id="4191e-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4191e-134">Key of the entity.</span></span> <span data-ttu-id="4191e-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4191e-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4191e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4191e-136">displayName</span></span>|<span data-ttu-id="4191e-137">String</span><span class="sxs-lookup"><span data-stu-id="4191e-137">String</span></span>|<span data-ttu-id="4191e-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="4191e-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4191e-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4191e-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4191e-140">description</span><span class="sxs-lookup"><span data-stu-id="4191e-140">description</span></span>|<span data-ttu-id="4191e-141">String</span><span class="sxs-lookup"><span data-stu-id="4191e-141">String</span></span>|<span data-ttu-id="4191e-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="4191e-142">The description of the app.</span></span> <span data-ttu-id="4191e-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4191e-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4191e-144">publisher</span><span class="sxs-lookup"><span data-stu-id="4191e-144">publisher</span></span>|<span data-ttu-id="4191e-145">String</span><span class="sxs-lookup"><span data-stu-id="4191e-145">String</span></span>|<span data-ttu-id="4191e-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="4191e-146">The publisher of the app.</span></span> <span data-ttu-id="4191e-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4191e-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4191e-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4191e-148">largeIcon</span></span>|[<span data-ttu-id="4191e-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4191e-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4191e-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="4191e-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4191e-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4191e-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4191e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4191e-152">createdDateTime</span></span>|<span data-ttu-id="4191e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4191e-153">DateTimeOffset</span></span>|<span data-ttu-id="4191e-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4191e-154">The date and time the app was created.</span></span> <span data-ttu-id="4191e-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4191e-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4191e-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4191e-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4191e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4191e-157">DateTimeOffset</span></span>|<span data-ttu-id="4191e-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4191e-158">The date and time the app was last modified.</span></span> <span data-ttu-id="4191e-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4191e-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4191e-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4191e-160">isFeatured</span></span>|<span data-ttu-id="4191e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4191e-161">Boolean</span></span>|<span data-ttu-id="4191e-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4191e-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4191e-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4191e-163">privacyInformationUrl</span></span>|<span data-ttu-id="4191e-164">String</span><span class="sxs-lookup"><span data-stu-id="4191e-164">String</span></span>|<span data-ttu-id="4191e-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="4191e-165">The privacy statement Url.</span></span> <span data-ttu-id="4191e-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4191e-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4191e-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4191e-167">informationUrl</span></span>|<span data-ttu-id="4191e-168">String</span><span class="sxs-lookup"><span data-stu-id="4191e-168">String</span></span>|<span data-ttu-id="4191e-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="4191e-169">The more information Url.</span></span> <span data-ttu-id="4191e-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4191e-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4191e-171">owner</span><span class="sxs-lookup"><span data-stu-id="4191e-171">owner</span></span>|<span data-ttu-id="4191e-172">字符串</span><span class="sxs-lookup"><span data-stu-id="4191e-172">String</span></span>|<span data-ttu-id="4191e-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="4191e-173">The owner of the app.</span></span> <span data-ttu-id="4191e-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4191e-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4191e-175">developer</span><span class="sxs-lookup"><span data-stu-id="4191e-175">developer</span></span>|<span data-ttu-id="4191e-176">String</span><span class="sxs-lookup"><span data-stu-id="4191e-176">String</span></span>|<span data-ttu-id="4191e-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="4191e-177">The developer of the app.</span></span> <span data-ttu-id="4191e-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4191e-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4191e-179">notes</span><span class="sxs-lookup"><span data-stu-id="4191e-179">notes</span></span>|<span data-ttu-id="4191e-180">String</span><span class="sxs-lookup"><span data-stu-id="4191e-180">String</span></span>|<span data-ttu-id="4191e-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="4191e-181">Notes for the app.</span></span> <span data-ttu-id="4191e-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4191e-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4191e-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="4191e-183">uploadState</span></span>|<span data-ttu-id="4191e-184">Int32</span><span class="sxs-lookup"><span data-stu-id="4191e-184">Int32</span></span>|<span data-ttu-id="4191e-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="4191e-185">The upload state.</span></span> <span data-ttu-id="4191e-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4191e-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4191e-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="4191e-187">publishingState</span></span>|[<span data-ttu-id="4191e-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4191e-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4191e-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="4191e-189">The publishing state for the app.</span></span> <span data-ttu-id="4191e-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="4191e-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4191e-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="4191e-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4191e-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="4191e-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4191e-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4191e-193">isAssigned</span></span>|<span data-ttu-id="4191e-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4191e-194">Boolean</span></span>|<span data-ttu-id="4191e-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="4191e-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4191e-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4191e-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4191e-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4191e-197">roleScopeTagIds</span></span>|<span data-ttu-id="4191e-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="4191e-198">String collection</span></span>|<span data-ttu-id="4191e-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="4191e-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4191e-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4191e-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4191e-201">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4191e-201">usedLicenseCount</span></span>|<span data-ttu-id="4191e-202">Int32</span><span class="sxs-lookup"><span data-stu-id="4191e-202">Int32</span></span>|<span data-ttu-id="4191e-203">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="4191e-203">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="4191e-204">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4191e-204">totalLicenseCount</span></span>|<span data-ttu-id="4191e-205">Int32</span><span class="sxs-lookup"><span data-stu-id="4191e-205">Int32</span></span>|<span data-ttu-id="4191e-206">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="4191e-206">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="4191e-207">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="4191e-207">releaseDateTime</span></span>|<span data-ttu-id="4191e-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4191e-208">DateTimeOffset</span></span>|<span data-ttu-id="4191e-209">VPP 应用程序的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4191e-209">The VPP application release date and time.</span></span>|
|<span data-ttu-id="4191e-210">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4191e-210">appStoreUrl</span></span>|<span data-ttu-id="4191e-211">String</span><span class="sxs-lookup"><span data-stu-id="4191e-211">String</span></span>|<span data-ttu-id="4191e-212">存储 URL。</span><span class="sxs-lookup"><span data-stu-id="4191e-212">The store URL.</span></span>|
|<span data-ttu-id="4191e-213">licensingType</span><span class="sxs-lookup"><span data-stu-id="4191e-213">licensingType</span></span>|[<span data-ttu-id="4191e-214">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="4191e-214">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="4191e-215">受支持的许可证类型。</span><span class="sxs-lookup"><span data-stu-id="4191e-215">The supported License Type.</span></span>|
|<span data-ttu-id="4191e-216">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="4191e-216">vppTokenOrganizationName</span></span>|<span data-ttu-id="4191e-217">String</span><span class="sxs-lookup"><span data-stu-id="4191e-217">String</span></span>|<span data-ttu-id="4191e-218">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="4191e-218">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="4191e-219">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="4191e-219">vppTokenAccountType</span></span>|[<span data-ttu-id="4191e-220">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="4191e-220">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="4191e-221">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="4191e-221">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="4191e-222">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="4191e-222">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="4191e-223">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="4191e-223">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="4191e-224">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="4191e-224">vppTokenAppleId</span></span>|<span data-ttu-id="4191e-225">String</span><span class="sxs-lookup"><span data-stu-id="4191e-225">String</span></span>|<span data-ttu-id="4191e-226">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="4191e-226">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="4191e-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="4191e-227">bundleId</span></span>|<span data-ttu-id="4191e-228">String</span><span class="sxs-lookup"><span data-stu-id="4191e-228">String</span></span>|<span data-ttu-id="4191e-229">标识名称。</span><span class="sxs-lookup"><span data-stu-id="4191e-229">The Identity Name.</span></span>|
|<span data-ttu-id="4191e-230">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="4191e-230">vppTokenId</span></span>|<span data-ttu-id="4191e-231">String</span><span class="sxs-lookup"><span data-stu-id="4191e-231">String</span></span>|<span data-ttu-id="4191e-232">与此应用程序关联的 VPP 令牌的标识符。</span><span class="sxs-lookup"><span data-stu-id="4191e-232">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="4191e-233">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="4191e-233">revokeLicenseActionResults</span></span>|<span data-ttu-id="4191e-234">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="4191e-234">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="4191e-235">对此应用吊销许可证操作的结果。</span><span class="sxs-lookup"><span data-stu-id="4191e-235">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="4191e-236">响应</span><span class="sxs-lookup"><span data-stu-id="4191e-236">Response</span></span>
<span data-ttu-id="4191e-237">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[macOsVppApp](../resources/intune-apps-macosvppapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4191e-237">If successful, this method returns a `200 OK` response code and an updated [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4191e-238">示例</span><span class="sxs-lookup"><span data-stu-id="4191e-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="4191e-239">请求</span><span class="sxs-lookup"><span data-stu-id="4191e-239">Request</span></span>
<span data-ttu-id="4191e-240">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4191e-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1842

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

### <a name="response"></a><span data-ttu-id="4191e-241">响应</span><span class="sxs-lookup"><span data-stu-id="4191e-241">Response</span></span>
<span data-ttu-id="4191e-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4191e-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2014

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




