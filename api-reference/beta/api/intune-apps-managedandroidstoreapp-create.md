---
title: 创建 managedAndroidStoreApp
description: 创建新的 managedAndroidStoreApp 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 272c2805d48cdf787b253a2e7a2ded81d8505739
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34974991"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="22bc2-103">创建 managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="22bc2-103">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="22bc2-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="22bc2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22bc2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22bc2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22bc2-106">创建新的 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="22bc2-106">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22bc2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="22bc2-107">Prerequisites</span></span>
<span data-ttu-id="22bc2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22bc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22bc2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="22bc2-110">Permission type</span></span>|<span data-ttu-id="22bc2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="22bc2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22bc2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22bc2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22bc2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22bc2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="22bc2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22bc2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22bc2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="22bc2-115">Not supported.</span></span>|
|<span data-ttu-id="22bc2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="22bc2-116">Application</span></span>|<span data-ttu-id="22bc2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="22bc2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22bc2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22bc2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="22bc2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="22bc2-119">Request headers</span></span>
|<span data-ttu-id="22bc2-120">标头</span><span class="sxs-lookup"><span data-stu-id="22bc2-120">Header</span></span>|<span data-ttu-id="22bc2-121">值</span><span class="sxs-lookup"><span data-stu-id="22bc2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22bc2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="22bc2-122">Authorization</span></span>|<span data-ttu-id="22bc2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="22bc2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22bc2-124">接受</span><span class="sxs-lookup"><span data-stu-id="22bc2-124">Accept</span></span>|<span data-ttu-id="22bc2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="22bc2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22bc2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="22bc2-126">Request body</span></span>
<span data-ttu-id="22bc2-127">在请求正文中，提供 managedAndroidStoreApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22bc2-127">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="22bc2-128">下表显示了创建 managedAndroidStoreApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="22bc2-128">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="22bc2-129">属性</span><span class="sxs-lookup"><span data-stu-id="22bc2-129">Property</span></span>|<span data-ttu-id="22bc2-130">类型</span><span class="sxs-lookup"><span data-stu-id="22bc2-130">Type</span></span>|<span data-ttu-id="22bc2-131">说明</span><span class="sxs-lookup"><span data-stu-id="22bc2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22bc2-132">id</span><span class="sxs-lookup"><span data-stu-id="22bc2-132">id</span></span>|<span data-ttu-id="22bc2-133">字符串</span><span class="sxs-lookup"><span data-stu-id="22bc2-133">String</span></span>|<span data-ttu-id="22bc2-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="22bc2-134">Key of the entity.</span></span> <span data-ttu-id="22bc2-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22bc2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="22bc2-136">displayName</span></span>|<span data-ttu-id="22bc2-137">String</span><span class="sxs-lookup"><span data-stu-id="22bc2-137">String</span></span>|<span data-ttu-id="22bc2-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="22bc2-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="22bc2-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22bc2-140">说明</span><span class="sxs-lookup"><span data-stu-id="22bc2-140">description</span></span>|<span data-ttu-id="22bc2-141">字符串</span><span class="sxs-lookup"><span data-stu-id="22bc2-141">String</span></span>|<span data-ttu-id="22bc2-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="22bc2-142">The description of the app.</span></span> <span data-ttu-id="22bc2-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22bc2-144">publisher</span><span class="sxs-lookup"><span data-stu-id="22bc2-144">publisher</span></span>|<span data-ttu-id="22bc2-145">String</span><span class="sxs-lookup"><span data-stu-id="22bc2-145">String</span></span>|<span data-ttu-id="22bc2-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="22bc2-146">The publisher of the app.</span></span> <span data-ttu-id="22bc2-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22bc2-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="22bc2-148">largeIcon</span></span>|[<span data-ttu-id="22bc2-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="22bc2-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="22bc2-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="22bc2-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="22bc2-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22bc2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22bc2-152">createdDateTime</span></span>|<span data-ttu-id="22bc2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22bc2-153">DateTimeOffset</span></span>|<span data-ttu-id="22bc2-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="22bc2-154">The date and time the app was created.</span></span> <span data-ttu-id="22bc2-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22bc2-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22bc2-156">lastModifiedDateTime</span></span>|<span data-ttu-id="22bc2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22bc2-157">DateTimeOffset</span></span>|<span data-ttu-id="22bc2-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="22bc2-158">The date and time the app was last modified.</span></span> <span data-ttu-id="22bc2-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22bc2-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="22bc2-160">isFeatured</span></span>|<span data-ttu-id="22bc2-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="22bc2-161">Boolean</span></span>|<span data-ttu-id="22bc2-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22bc2-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="22bc2-163">privacyInformationUrl</span></span>|<span data-ttu-id="22bc2-164">String</span><span class="sxs-lookup"><span data-stu-id="22bc2-164">String</span></span>|<span data-ttu-id="22bc2-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="22bc2-165">The privacy statement Url.</span></span> <span data-ttu-id="22bc2-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22bc2-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="22bc2-167">informationUrl</span></span>|<span data-ttu-id="22bc2-168">String</span><span class="sxs-lookup"><span data-stu-id="22bc2-168">String</span></span>|<span data-ttu-id="22bc2-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="22bc2-169">The more information Url.</span></span> <span data-ttu-id="22bc2-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22bc2-171">owner</span><span class="sxs-lookup"><span data-stu-id="22bc2-171">owner</span></span>|<span data-ttu-id="22bc2-172">String</span><span class="sxs-lookup"><span data-stu-id="22bc2-172">String</span></span>|<span data-ttu-id="22bc2-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="22bc2-173">The owner of the app.</span></span> <span data-ttu-id="22bc2-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22bc2-175">developer</span><span class="sxs-lookup"><span data-stu-id="22bc2-175">developer</span></span>|<span data-ttu-id="22bc2-176">String</span><span class="sxs-lookup"><span data-stu-id="22bc2-176">String</span></span>|<span data-ttu-id="22bc2-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="22bc2-177">The developer of the app.</span></span> <span data-ttu-id="22bc2-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22bc2-179">notes</span><span class="sxs-lookup"><span data-stu-id="22bc2-179">notes</span></span>|<span data-ttu-id="22bc2-180">String</span><span class="sxs-lookup"><span data-stu-id="22bc2-180">String</span></span>|<span data-ttu-id="22bc2-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="22bc2-181">Notes for the app.</span></span> <span data-ttu-id="22bc2-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22bc2-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="22bc2-183">uploadState</span></span>|<span data-ttu-id="22bc2-184">Int32</span><span class="sxs-lookup"><span data-stu-id="22bc2-184">Int32</span></span>|<span data-ttu-id="22bc2-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="22bc2-185">The upload state.</span></span> <span data-ttu-id="22bc2-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22bc2-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="22bc2-187">publishingState</span></span>|[<span data-ttu-id="22bc2-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="22bc2-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="22bc2-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="22bc2-189">The publishing state for the app.</span></span> <span data-ttu-id="22bc2-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="22bc2-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="22bc2-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="22bc2-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="22bc2-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="22bc2-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="22bc2-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="22bc2-193">isAssigned</span></span>|<span data-ttu-id="22bc2-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="22bc2-194">Boolean</span></span>|<span data-ttu-id="22bc2-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="22bc2-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="22bc2-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22bc2-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="22bc2-197">roleScopeTagIds</span></span>|<span data-ttu-id="22bc2-198">String collection</span><span class="sxs-lookup"><span data-stu-id="22bc2-198">String collection</span></span>|<span data-ttu-id="22bc2-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="22bc2-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="22bc2-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22bc2-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="22bc2-201">dependentAppCount</span></span>|<span data-ttu-id="22bc2-202">Int32</span><span class="sxs-lookup"><span data-stu-id="22bc2-202">Int32</span></span>|<span data-ttu-id="22bc2-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="22bc2-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="22bc2-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22bc2-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="22bc2-205">appAvailability</span></span>|[<span data-ttu-id="22bc2-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="22bc2-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="22bc2-207">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="22bc2-207">The Application's availability.</span></span> <span data-ttu-id="22bc2-208">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="22bc2-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="22bc2-209">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="22bc2-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="22bc2-210">version</span><span class="sxs-lookup"><span data-stu-id="22bc2-210">version</span></span>|<span data-ttu-id="22bc2-211">String</span><span class="sxs-lookup"><span data-stu-id="22bc2-211">String</span></span>|<span data-ttu-id="22bc2-212">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="22bc2-212">The Application's version.</span></span> <span data-ttu-id="22bc2-213">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="22bc2-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="22bc2-214">packageId</span><span class="sxs-lookup"><span data-stu-id="22bc2-214">packageId</span></span>|<span data-ttu-id="22bc2-215">String</span><span class="sxs-lookup"><span data-stu-id="22bc2-215">String</span></span>|<span data-ttu-id="22bc2-216">应用的包 ID。</span><span class="sxs-lookup"><span data-stu-id="22bc2-216">The app's package ID.</span></span>|
|<span data-ttu-id="22bc2-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="22bc2-217">appStoreUrl</span></span>|<span data-ttu-id="22bc2-218">String</span><span class="sxs-lookup"><span data-stu-id="22bc2-218">String</span></span>|<span data-ttu-id="22bc2-219">Android AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="22bc2-219">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="22bc2-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="22bc2-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="22bc2-221">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="22bc2-221">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="22bc2-222">最低受支持操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="22bc2-222">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="22bc2-223">响应</span><span class="sxs-lookup"><span data-stu-id="22bc2-223">Response</span></span>
<span data-ttu-id="22bc2-224">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="22bc2-224">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22bc2-225">示例</span><span class="sxs-lookup"><span data-stu-id="22bc2-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="22bc2-226">请求</span><span class="sxs-lookup"><span data-stu-id="22bc2-226">Request</span></span>
<span data-ttu-id="22bc2-227">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="22bc2-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1264

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
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
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="22bc2-228">响应</span><span class="sxs-lookup"><span data-stu-id="22bc2-228">Response</span></span>
<span data-ttu-id="22bc2-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="22bc2-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1436

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
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
    "v9_0": true
  }
}
```





