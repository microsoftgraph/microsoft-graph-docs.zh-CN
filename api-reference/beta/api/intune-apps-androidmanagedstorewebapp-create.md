---
title: 创建 androidManagedStoreWebApp
description: 创建新的 androidManagedStoreWebApp 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bafc18f14063e3f6c78c7eaad99329b0c2bbcd0d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39926493"
---
# <a name="create-androidmanagedstorewebapp"></a><span data-ttu-id="e0615-103">创建 androidManagedStoreWebApp</span><span class="sxs-lookup"><span data-stu-id="e0615-103">Create androidManagedStoreWebApp</span></span>

> <span data-ttu-id="e0615-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e0615-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0615-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e0615-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0615-106">创建新的[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e0615-106">Create a new [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0615-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e0615-107">Prerequisites</span></span>
<span data-ttu-id="e0615-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0615-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0615-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0615-110">Permission type</span></span>|<span data-ttu-id="e0615-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e0615-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0615-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0615-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0615-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0615-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e0615-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0615-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0615-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0615-115">Not supported.</span></span>|
|<span data-ttu-id="e0615-116">Application</span><span class="sxs-lookup"><span data-stu-id="e0615-116">Application</span></span>|<span data-ttu-id="e0615-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0615-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0615-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0615-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e0615-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0615-119">Request headers</span></span>
|<span data-ttu-id="e0615-120">标头</span><span class="sxs-lookup"><span data-stu-id="e0615-120">Header</span></span>|<span data-ttu-id="e0615-121">值</span><span class="sxs-lookup"><span data-stu-id="e0615-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0615-122">授权</span><span class="sxs-lookup"><span data-stu-id="e0615-122">Authorization</span></span>|<span data-ttu-id="e0615-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e0615-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0615-124">接受</span><span class="sxs-lookup"><span data-stu-id="e0615-124">Accept</span></span>|<span data-ttu-id="e0615-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e0615-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0615-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0615-126">Request body</span></span>
<span data-ttu-id="e0615-127">在请求正文中，提供 androidManagedStoreWebApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0615-127">In the request body, supply a JSON representation for the androidManagedStoreWebApp object.</span></span>

<span data-ttu-id="e0615-128">下表显示创建 androidManagedStoreWebApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e0615-128">The following table shows the properties that are required when you create the androidManagedStoreWebApp.</span></span>

|<span data-ttu-id="e0615-129">属性</span><span class="sxs-lookup"><span data-stu-id="e0615-129">Property</span></span>|<span data-ttu-id="e0615-130">类型</span><span class="sxs-lookup"><span data-stu-id="e0615-130">Type</span></span>|<span data-ttu-id="e0615-131">说明</span><span class="sxs-lookup"><span data-stu-id="e0615-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0615-132">id</span><span class="sxs-lookup"><span data-stu-id="e0615-132">id</span></span>|<span data-ttu-id="e0615-133">字符串</span><span class="sxs-lookup"><span data-stu-id="e0615-133">String</span></span>|<span data-ttu-id="e0615-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e0615-134">Key of the entity.</span></span> <span data-ttu-id="e0615-135">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0615-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e0615-136">displayName</span></span>|<span data-ttu-id="e0615-137">字符串</span><span class="sxs-lookup"><span data-stu-id="e0615-137">String</span></span>|<span data-ttu-id="e0615-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="e0615-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e0615-139">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0615-140">说明</span><span class="sxs-lookup"><span data-stu-id="e0615-140">description</span></span>|<span data-ttu-id="e0615-141">字符串</span><span class="sxs-lookup"><span data-stu-id="e0615-141">String</span></span>|<span data-ttu-id="e0615-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="e0615-142">The description of the app.</span></span> <span data-ttu-id="e0615-143">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0615-144">publisher</span><span class="sxs-lookup"><span data-stu-id="e0615-144">publisher</span></span>|<span data-ttu-id="e0615-145">字符串</span><span class="sxs-lookup"><span data-stu-id="e0615-145">String</span></span>|<span data-ttu-id="e0615-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="e0615-146">The publisher of the app.</span></span> <span data-ttu-id="e0615-147">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0615-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e0615-148">largeIcon</span></span>|[<span data-ttu-id="e0615-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e0615-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e0615-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="e0615-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e0615-151">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0615-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0615-152">createdDateTime</span></span>|<span data-ttu-id="e0615-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0615-153">DateTimeOffset</span></span>|<span data-ttu-id="e0615-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e0615-154">The date and time the app was created.</span></span> <span data-ttu-id="e0615-155">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0615-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0615-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e0615-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0615-157">DateTimeOffset</span></span>|<span data-ttu-id="e0615-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e0615-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e0615-159">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0615-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e0615-160">isFeatured</span></span>|<span data-ttu-id="e0615-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0615-161">Boolean</span></span>|<span data-ttu-id="e0615-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0615-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e0615-163">privacyInformationUrl</span></span>|<span data-ttu-id="e0615-164">字符串</span><span class="sxs-lookup"><span data-stu-id="e0615-164">String</span></span>|<span data-ttu-id="e0615-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="e0615-165">The privacy statement Url.</span></span> <span data-ttu-id="e0615-166">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0615-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e0615-167">informationUrl</span></span>|<span data-ttu-id="e0615-168">字符串</span><span class="sxs-lookup"><span data-stu-id="e0615-168">String</span></span>|<span data-ttu-id="e0615-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="e0615-169">The more information Url.</span></span> <span data-ttu-id="e0615-170">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0615-171">owner</span><span class="sxs-lookup"><span data-stu-id="e0615-171">owner</span></span>|<span data-ttu-id="e0615-172">String</span><span class="sxs-lookup"><span data-stu-id="e0615-172">String</span></span>|<span data-ttu-id="e0615-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="e0615-173">The owner of the app.</span></span> <span data-ttu-id="e0615-174">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0615-175">developer</span><span class="sxs-lookup"><span data-stu-id="e0615-175">developer</span></span>|<span data-ttu-id="e0615-176">字符串</span><span class="sxs-lookup"><span data-stu-id="e0615-176">String</span></span>|<span data-ttu-id="e0615-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="e0615-177">The developer of the app.</span></span> <span data-ttu-id="e0615-178">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0615-179">notes</span><span class="sxs-lookup"><span data-stu-id="e0615-179">notes</span></span>|<span data-ttu-id="e0615-180">字符串</span><span class="sxs-lookup"><span data-stu-id="e0615-180">String</span></span>|<span data-ttu-id="e0615-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="e0615-181">Notes for the app.</span></span> <span data-ttu-id="e0615-182">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0615-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="e0615-183">uploadState</span></span>|<span data-ttu-id="e0615-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e0615-184">Int32</span></span>|<span data-ttu-id="e0615-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="e0615-185">The upload state.</span></span> <span data-ttu-id="e0615-186">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0615-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="e0615-187">publishingState</span></span>|[<span data-ttu-id="e0615-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e0615-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e0615-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="e0615-189">The publishing state for the app.</span></span> <span data-ttu-id="e0615-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="e0615-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e0615-191">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="e0615-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="e0615-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="e0615-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e0615-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e0615-193">isAssigned</span></span>|<span data-ttu-id="e0615-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0615-194">Boolean</span></span>|<span data-ttu-id="e0615-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="e0615-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e0615-196">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0615-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e0615-197">roleScopeTagIds</span></span>|<span data-ttu-id="e0615-198">String collection</span><span class="sxs-lookup"><span data-stu-id="e0615-198">String collection</span></span>|<span data-ttu-id="e0615-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="e0615-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e0615-200">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0615-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e0615-201">dependentAppCount</span></span>|<span data-ttu-id="e0615-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e0615-202">Int32</span></span>|<span data-ttu-id="e0615-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="e0615-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e0615-204">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0615-205">packageId</span><span class="sxs-lookup"><span data-stu-id="e0615-205">packageId</span></span>|<span data-ttu-id="e0615-206">字符串</span><span class="sxs-lookup"><span data-stu-id="e0615-206">String</span></span>|<span data-ttu-id="e0615-207">包标识符。</span><span class="sxs-lookup"><span data-stu-id="e0615-207">The package identifier.</span></span> <span data-ttu-id="e0615-208">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-208">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="e0615-209">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="e0615-209">appIdentifier</span></span>|<span data-ttu-id="e0615-210">String</span><span class="sxs-lookup"><span data-stu-id="e0615-210">String</span></span>|<span data-ttu-id="e0615-211">标识名称。</span><span class="sxs-lookup"><span data-stu-id="e0615-211">The Identity Name.</span></span> <span data-ttu-id="e0615-212">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-212">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="e0615-213">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e0615-213">usedLicenseCount</span></span>|<span data-ttu-id="e0615-214">Int32</span><span class="sxs-lookup"><span data-stu-id="e0615-214">Int32</span></span>|<span data-ttu-id="e0615-215">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="e0615-215">The number of VPP licenses in use.</span></span> <span data-ttu-id="e0615-216">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-216">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="e0615-217">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e0615-217">totalLicenseCount</span></span>|<span data-ttu-id="e0615-218">Int32</span><span class="sxs-lookup"><span data-stu-id="e0615-218">Int32</span></span>|<span data-ttu-id="e0615-219">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="e0615-219">The total number of VPP licenses.</span></span> <span data-ttu-id="e0615-220">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-220">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="e0615-221">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="e0615-221">appStoreUrl</span></span>|<span data-ttu-id="e0615-222">String</span><span class="sxs-lookup"><span data-stu-id="e0615-222">String</span></span>|<span data-ttu-id="e0615-223">"播放工作商店" 应用程序 URL。</span><span class="sxs-lookup"><span data-stu-id="e0615-223">The Play for Work Store app URL.</span></span> <span data-ttu-id="e0615-224">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-224">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="e0615-225">isPrivate</span><span class="sxs-lookup"><span data-stu-id="e0615-225">isPrivate</span></span>|<span data-ttu-id="e0615-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0615-226">Boolean</span></span>|<span data-ttu-id="e0615-227">指示应用程序是否仅适用于给定企业的用户。</span><span class="sxs-lookup"><span data-stu-id="e0615-227">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="e0615-228">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-228">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="e0615-229">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="e0615-229">isSystemApp</span></span>|<span data-ttu-id="e0615-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0615-230">Boolean</span></span>|<span data-ttu-id="e0615-231">指示应用程序是否为预安装的系统应用程序。</span><span class="sxs-lookup"><span data-stu-id="e0615-231">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="e0615-232">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-232">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="e0615-233">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="e0615-233">supportsOemConfig</span></span>|<span data-ttu-id="e0615-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0615-234">Boolean</span></span>|<span data-ttu-id="e0615-235">此应用是否支持 OEMConfig 策略。</span><span class="sxs-lookup"><span data-stu-id="e0615-235">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="e0615-236">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0615-236">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e0615-237">响应</span><span class="sxs-lookup"><span data-stu-id="e0615-237">Response</span></span>
<span data-ttu-id="e0615-238">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e0615-238">If successful, this method returns a `201 Created` response code and a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0615-239">示例</span><span class="sxs-lookup"><span data-stu-id="e0615-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0615-240">请求</span><span class="sxs-lookup"><span data-stu-id="e0615-240">Request</span></span>
<span data-ttu-id="e0615-241">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0615-241">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 987

{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="e0615-242">响应</span><span class="sxs-lookup"><span data-stu-id="e0615-242">Response</span></span>
<span data-ttu-id="e0615-p127">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e0615-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1159

{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
  "id": "e54aecbd-ecbd-e54a-bdec-4ae5bdec4ae5",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "supportsOemConfig": true
}
```





