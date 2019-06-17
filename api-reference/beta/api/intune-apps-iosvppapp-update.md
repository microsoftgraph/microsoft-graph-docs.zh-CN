---
title: 更新 iosVppApp
description: 更新 iosVppApp 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ac57d3c4bfb7d6876e20259394d9f3595af6c468
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964925"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="5bd6a-103">更新 iosVppApp</span><span class="sxs-lookup"><span data-stu-id="5bd6a-103">Update iosVppApp</span></span>

> <span data-ttu-id="5bd6a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bd6a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bd6a-106">更新 [iosVppApp](../resources/intune-apps-iosvppapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-106">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bd6a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5bd6a-107">Prerequisites</span></span>
<span data-ttu-id="5bd6a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bd6a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5bd6a-110">Permission type</span></span>|<span data-ttu-id="5bd6a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5bd6a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bd6a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5bd6a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5bd6a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bd6a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5bd6a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5bd6a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bd6a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-115">Not supported.</span></span>|
|<span data-ttu-id="5bd6a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5bd6a-116">Application</span></span>|<span data-ttu-id="5bd6a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bd6a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5bd6a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="5bd6a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5bd6a-119">Request headers</span></span>
|<span data-ttu-id="5bd6a-120">标头</span><span class="sxs-lookup"><span data-stu-id="5bd6a-120">Header</span></span>|<span data-ttu-id="5bd6a-121">值</span><span class="sxs-lookup"><span data-stu-id="5bd6a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bd6a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bd6a-122">Authorization</span></span>|<span data-ttu-id="5bd6a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bd6a-124">接受</span><span class="sxs-lookup"><span data-stu-id="5bd6a-124">Accept</span></span>|<span data-ttu-id="5bd6a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5bd6a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bd6a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5bd6a-126">Request body</span></span>
<span data-ttu-id="5bd6a-127">在请求正文中，提供 [iosVppApp](../resources/intune-apps-iosvppapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-127">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="5bd6a-128">下表显示了创建 [iosVppApp](../resources/intune-apps-iosvppapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-128">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="5bd6a-129">属性</span><span class="sxs-lookup"><span data-stu-id="5bd6a-129">Property</span></span>|<span data-ttu-id="5bd6a-130">类型</span><span class="sxs-lookup"><span data-stu-id="5bd6a-130">Type</span></span>|<span data-ttu-id="5bd6a-131">说明</span><span class="sxs-lookup"><span data-stu-id="5bd6a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bd6a-132">id</span><span class="sxs-lookup"><span data-stu-id="5bd6a-132">id</span></span>|<span data-ttu-id="5bd6a-133">字符串</span><span class="sxs-lookup"><span data-stu-id="5bd6a-133">String</span></span>|<span data-ttu-id="5bd6a-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-134">Key of the entity.</span></span> <span data-ttu-id="5bd6a-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5bd6a-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5bd6a-136">displayName</span></span>|<span data-ttu-id="5bd6a-137">String</span><span class="sxs-lookup"><span data-stu-id="5bd6a-137">String</span></span>|<span data-ttu-id="5bd6a-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5bd6a-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5bd6a-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6a-140">说明</span><span class="sxs-lookup"><span data-stu-id="5bd6a-140">description</span></span>|<span data-ttu-id="5bd6a-141">字符串</span><span class="sxs-lookup"><span data-stu-id="5bd6a-141">String</span></span>|<span data-ttu-id="5bd6a-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-142">The description of the app.</span></span> <span data-ttu-id="5bd6a-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5bd6a-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6a-144">publisher</span><span class="sxs-lookup"><span data-stu-id="5bd6a-144">publisher</span></span>|<span data-ttu-id="5bd6a-145">String</span><span class="sxs-lookup"><span data-stu-id="5bd6a-145">String</span></span>|<span data-ttu-id="5bd6a-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-146">The publisher of the app.</span></span> <span data-ttu-id="5bd6a-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5bd6a-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5bd6a-148">largeIcon</span></span>|[<span data-ttu-id="5bd6a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5bd6a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5bd6a-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5bd6a-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5bd6a-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5bd6a-152">createdDateTime</span></span>|<span data-ttu-id="5bd6a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bd6a-153">DateTimeOffset</span></span>|<span data-ttu-id="5bd6a-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-154">The date and time the app was created.</span></span> <span data-ttu-id="5bd6a-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5bd6a-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5bd6a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="5bd6a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bd6a-157">DateTimeOffset</span></span>|<span data-ttu-id="5bd6a-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="5bd6a-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5bd6a-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5bd6a-160">isFeatured</span></span>|<span data-ttu-id="5bd6a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bd6a-161">Boolean</span></span>|<span data-ttu-id="5bd6a-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5bd6a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5bd6a-163">privacyInformationUrl</span></span>|<span data-ttu-id="5bd6a-164">String</span><span class="sxs-lookup"><span data-stu-id="5bd6a-164">String</span></span>|<span data-ttu-id="5bd6a-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-165">The privacy statement Url.</span></span> <span data-ttu-id="5bd6a-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5bd6a-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5bd6a-167">informationUrl</span></span>|<span data-ttu-id="5bd6a-168">String</span><span class="sxs-lookup"><span data-stu-id="5bd6a-168">String</span></span>|<span data-ttu-id="5bd6a-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-169">The more information Url.</span></span> <span data-ttu-id="5bd6a-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5bd6a-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6a-171">owner</span><span class="sxs-lookup"><span data-stu-id="5bd6a-171">owner</span></span>|<span data-ttu-id="5bd6a-172">String</span><span class="sxs-lookup"><span data-stu-id="5bd6a-172">String</span></span>|<span data-ttu-id="5bd6a-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-173">The owner of the app.</span></span> <span data-ttu-id="5bd6a-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5bd6a-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6a-175">developer</span><span class="sxs-lookup"><span data-stu-id="5bd6a-175">developer</span></span>|<span data-ttu-id="5bd6a-176">String</span><span class="sxs-lookup"><span data-stu-id="5bd6a-176">String</span></span>|<span data-ttu-id="5bd6a-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-177">The developer of the app.</span></span> <span data-ttu-id="5bd6a-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5bd6a-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6a-179">notes</span><span class="sxs-lookup"><span data-stu-id="5bd6a-179">notes</span></span>|<span data-ttu-id="5bd6a-180">String</span><span class="sxs-lookup"><span data-stu-id="5bd6a-180">String</span></span>|<span data-ttu-id="5bd6a-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-181">Notes for the app.</span></span> <span data-ttu-id="5bd6a-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5bd6a-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6a-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="5bd6a-183">uploadState</span></span>|<span data-ttu-id="5bd6a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="5bd6a-184">Int32</span></span>|<span data-ttu-id="5bd6a-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-185">The upload state.</span></span> <span data-ttu-id="5bd6a-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5bd6a-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6a-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="5bd6a-187">publishingState</span></span>|[<span data-ttu-id="5bd6a-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5bd6a-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5bd6a-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-189">The publishing state for the app.</span></span> <span data-ttu-id="5bd6a-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5bd6a-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5bd6a-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5bd6a-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5bd6a-193">isAssigned</span></span>|<span data-ttu-id="5bd6a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bd6a-194">Boolean</span></span>|<span data-ttu-id="5bd6a-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="5bd6a-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5bd6a-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6a-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5bd6a-197">roleScopeTagIds</span></span>|<span data-ttu-id="5bd6a-198">String collection</span><span class="sxs-lookup"><span data-stu-id="5bd6a-198">String collection</span></span>|<span data-ttu-id="5bd6a-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="5bd6a-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5bd6a-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6a-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="5bd6a-201">dependentAppCount</span></span>|<span data-ttu-id="5bd6a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="5bd6a-202">Int32</span></span>|<span data-ttu-id="5bd6a-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="5bd6a-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5bd6a-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6a-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="5bd6a-205">usedLicenseCount</span></span>|<span data-ttu-id="5bd6a-206">Int32</span><span class="sxs-lookup"><span data-stu-id="5bd6a-206">Int32</span></span>|<span data-ttu-id="5bd6a-207">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-207">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="5bd6a-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="5bd6a-208">totalLicenseCount</span></span>|<span data-ttu-id="5bd6a-209">Int32</span><span class="sxs-lookup"><span data-stu-id="5bd6a-209">Int32</span></span>|<span data-ttu-id="5bd6a-210">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-210">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="5bd6a-211">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="5bd6a-211">releaseDateTime</span></span>|<span data-ttu-id="5bd6a-212">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bd6a-212">DateTimeOffset</span></span>|<span data-ttu-id="5bd6a-213">VPP 应用程序的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-213">The VPP application release date and time.</span></span>|
|<span data-ttu-id="5bd6a-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="5bd6a-214">appStoreUrl</span></span>|<span data-ttu-id="5bd6a-215">String</span><span class="sxs-lookup"><span data-stu-id="5bd6a-215">String</span></span>|<span data-ttu-id="5bd6a-216">存储 URL。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-216">The store URL.</span></span>|
|<span data-ttu-id="5bd6a-217">licensingType</span><span class="sxs-lookup"><span data-stu-id="5bd6a-217">licensingType</span></span>|[<span data-ttu-id="5bd6a-218">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="5bd6a-218">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="5bd6a-219">受支持的许可证类型。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-219">The supported License Type.</span></span>|
|<span data-ttu-id="5bd6a-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="5bd6a-220">applicableDeviceType</span></span>|[<span data-ttu-id="5bd6a-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="5bd6a-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="5bd6a-222">适用的 iOS 设备类型。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-222">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="5bd6a-223">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="5bd6a-223">vppTokenOrganizationName</span></span>|<span data-ttu-id="5bd6a-224">String</span><span class="sxs-lookup"><span data-stu-id="5bd6a-224">String</span></span>|<span data-ttu-id="5bd6a-225">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="5bd6a-225">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="5bd6a-226">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="5bd6a-226">vppTokenAccountType</span></span>|[<span data-ttu-id="5bd6a-227">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="5bd6a-227">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="5bd6a-228">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-228">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="5bd6a-229">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-229">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="5bd6a-230">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-230">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="5bd6a-231">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="5bd6a-231">vppTokenAppleId</span></span>|<span data-ttu-id="5bd6a-232">String</span><span class="sxs-lookup"><span data-stu-id="5bd6a-232">String</span></span>|<span data-ttu-id="5bd6a-233">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-233">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="5bd6a-234">bundleId</span><span class="sxs-lookup"><span data-stu-id="5bd6a-234">bundleId</span></span>|<span data-ttu-id="5bd6a-235">String</span><span class="sxs-lookup"><span data-stu-id="5bd6a-235">String</span></span>|<span data-ttu-id="5bd6a-236">标识名称。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-236">The Identity Name.</span></span>|
|<span data-ttu-id="5bd6a-237">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="5bd6a-237">vppTokenId</span></span>|<span data-ttu-id="5bd6a-238">String</span><span class="sxs-lookup"><span data-stu-id="5bd6a-238">String</span></span>|<span data-ttu-id="5bd6a-239">与此应用程序关联的 VPP 令牌的标识符。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-239">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="5bd6a-240">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="5bd6a-240">revokeLicenseActionResults</span></span>|<span data-ttu-id="5bd6a-241">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="5bd6a-241">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="5bd6a-242">对此应用吊销许可证操作的结果。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-242">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="5bd6a-243">响应</span><span class="sxs-lookup"><span data-stu-id="5bd6a-243">Response</span></span>
<span data-ttu-id="5bd6a-244">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppApp](../resources/intune-apps-iosvppapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-244">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bd6a-245">示例</span><span class="sxs-lookup"><span data-stu-id="5bd6a-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bd6a-246">请求</span><span class="sxs-lookup"><span data-stu-id="5bd6a-246">Request</span></span>
<span data-ttu-id="5bd6a-247">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-247">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5bd6a-248">响应</span><span class="sxs-lookup"><span data-stu-id="5bd6a-248">Response</span></span>
<span data-ttu-id="5bd6a-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5bd6a-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





