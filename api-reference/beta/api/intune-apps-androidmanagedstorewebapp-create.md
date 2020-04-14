---
title: 创建 androidManagedStoreWebApp
description: 创建新的 androidManagedStoreWebApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c23d0df9033aa0f92c09ef6664776a154b3cfa3e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43417412"
---
# <a name="create-androidmanagedstorewebapp"></a><span data-ttu-id="d8e07-103">创建 androidManagedStoreWebApp</span><span class="sxs-lookup"><span data-stu-id="d8e07-103">Create androidManagedStoreWebApp</span></span>

<span data-ttu-id="d8e07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8e07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8e07-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d8e07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8e07-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d8e07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8e07-107">创建新的[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d8e07-107">Create a new [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8e07-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d8e07-108">Prerequisites</span></span>
<span data-ttu-id="d8e07-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8e07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8e07-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8e07-111">Permission type</span></span>|<span data-ttu-id="d8e07-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d8e07-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8e07-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8e07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8e07-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8e07-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d8e07-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8e07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8e07-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8e07-116">Not supported.</span></span>|
|<span data-ttu-id="d8e07-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8e07-117">Application</span></span>|<span data-ttu-id="d8e07-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8e07-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8e07-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8e07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d8e07-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8e07-120">Request headers</span></span>
|<span data-ttu-id="d8e07-121">标头</span><span class="sxs-lookup"><span data-stu-id="d8e07-121">Header</span></span>|<span data-ttu-id="d8e07-122">值</span><span class="sxs-lookup"><span data-stu-id="d8e07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8e07-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8e07-123">Authorization</span></span>|<span data-ttu-id="d8e07-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d8e07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8e07-125">接受</span><span class="sxs-lookup"><span data-stu-id="d8e07-125">Accept</span></span>|<span data-ttu-id="d8e07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8e07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8e07-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8e07-127">Request body</span></span>
<span data-ttu-id="d8e07-128">在请求正文中，提供 androidManagedStoreWebApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8e07-128">In the request body, supply a JSON representation for the androidManagedStoreWebApp object.</span></span>

<span data-ttu-id="d8e07-129">下表显示创建 androidManagedStoreWebApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d8e07-129">The following table shows the properties that are required when you create the androidManagedStoreWebApp.</span></span>

|<span data-ttu-id="d8e07-130">属性</span><span class="sxs-lookup"><span data-stu-id="d8e07-130">Property</span></span>|<span data-ttu-id="d8e07-131">类型</span><span class="sxs-lookup"><span data-stu-id="d8e07-131">Type</span></span>|<span data-ttu-id="d8e07-132">说明</span><span class="sxs-lookup"><span data-stu-id="d8e07-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8e07-133">id</span><span class="sxs-lookup"><span data-stu-id="d8e07-133">id</span></span>|<span data-ttu-id="d8e07-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d8e07-134">String</span></span>|<span data-ttu-id="d8e07-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d8e07-135">Key of the entity.</span></span> <span data-ttu-id="d8e07-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e07-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d8e07-137">displayName</span></span>|<span data-ttu-id="d8e07-138">String</span><span class="sxs-lookup"><span data-stu-id="d8e07-138">String</span></span>|<span data-ttu-id="d8e07-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="d8e07-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d8e07-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e07-141">description</span><span class="sxs-lookup"><span data-stu-id="d8e07-141">description</span></span>|<span data-ttu-id="d8e07-142">字符串</span><span class="sxs-lookup"><span data-stu-id="d8e07-142">String</span></span>|<span data-ttu-id="d8e07-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="d8e07-143">The description of the app.</span></span> <span data-ttu-id="d8e07-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e07-145">publisher</span><span class="sxs-lookup"><span data-stu-id="d8e07-145">publisher</span></span>|<span data-ttu-id="d8e07-146">String</span><span class="sxs-lookup"><span data-stu-id="d8e07-146">String</span></span>|<span data-ttu-id="d8e07-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="d8e07-147">The publisher of the app.</span></span> <span data-ttu-id="d8e07-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e07-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d8e07-149">largeIcon</span></span>|[<span data-ttu-id="d8e07-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d8e07-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d8e07-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="d8e07-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d8e07-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e07-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8e07-153">createdDateTime</span></span>|<span data-ttu-id="d8e07-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8e07-154">DateTimeOffset</span></span>|<span data-ttu-id="d8e07-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d8e07-155">The date and time the app was created.</span></span> <span data-ttu-id="d8e07-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e07-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8e07-157">lastModifiedDateTime</span></span>|<span data-ttu-id="d8e07-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8e07-158">DateTimeOffset</span></span>|<span data-ttu-id="d8e07-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d8e07-159">The date and time the app was last modified.</span></span> <span data-ttu-id="d8e07-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e07-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d8e07-161">isFeatured</span></span>|<span data-ttu-id="d8e07-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8e07-162">Boolean</span></span>|<span data-ttu-id="d8e07-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e07-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d8e07-164">privacyInformationUrl</span></span>|<span data-ttu-id="d8e07-165">String</span><span class="sxs-lookup"><span data-stu-id="d8e07-165">String</span></span>|<span data-ttu-id="d8e07-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="d8e07-166">The privacy statement Url.</span></span> <span data-ttu-id="d8e07-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e07-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d8e07-168">informationUrl</span></span>|<span data-ttu-id="d8e07-169">String</span><span class="sxs-lookup"><span data-stu-id="d8e07-169">String</span></span>|<span data-ttu-id="d8e07-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="d8e07-170">The more information Url.</span></span> <span data-ttu-id="d8e07-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e07-172">owner</span><span class="sxs-lookup"><span data-stu-id="d8e07-172">owner</span></span>|<span data-ttu-id="d8e07-173">String</span><span class="sxs-lookup"><span data-stu-id="d8e07-173">String</span></span>|<span data-ttu-id="d8e07-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="d8e07-174">The owner of the app.</span></span> <span data-ttu-id="d8e07-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e07-176">developer</span><span class="sxs-lookup"><span data-stu-id="d8e07-176">developer</span></span>|<span data-ttu-id="d8e07-177">String</span><span class="sxs-lookup"><span data-stu-id="d8e07-177">String</span></span>|<span data-ttu-id="d8e07-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="d8e07-178">The developer of the app.</span></span> <span data-ttu-id="d8e07-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e07-180">notes</span><span class="sxs-lookup"><span data-stu-id="d8e07-180">notes</span></span>|<span data-ttu-id="d8e07-181">String</span><span class="sxs-lookup"><span data-stu-id="d8e07-181">String</span></span>|<span data-ttu-id="d8e07-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="d8e07-182">Notes for the app.</span></span> <span data-ttu-id="d8e07-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e07-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="d8e07-184">uploadState</span></span>|<span data-ttu-id="d8e07-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d8e07-185">Int32</span></span>|<span data-ttu-id="d8e07-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="d8e07-186">The upload state.</span></span> <span data-ttu-id="d8e07-187">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e07-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="d8e07-188">publishingState</span></span>|[<span data-ttu-id="d8e07-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d8e07-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d8e07-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="d8e07-190">The publishing state for the app.</span></span> <span data-ttu-id="d8e07-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="d8e07-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d8e07-192">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="d8e07-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="d8e07-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="d8e07-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d8e07-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d8e07-194">isAssigned</span></span>|<span data-ttu-id="d8e07-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8e07-195">Boolean</span></span>|<span data-ttu-id="d8e07-196">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="d8e07-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d8e07-197">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e07-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d8e07-198">roleScopeTagIds</span></span>|<span data-ttu-id="d8e07-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="d8e07-199">String collection</span></span>|<span data-ttu-id="d8e07-200">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="d8e07-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d8e07-201">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e07-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="d8e07-202">dependentAppCount</span></span>|<span data-ttu-id="d8e07-203">Int32</span><span class="sxs-lookup"><span data-stu-id="d8e07-203">Int32</span></span>|<span data-ttu-id="d8e07-204">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="d8e07-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="d8e07-205">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e07-206">packageId</span><span class="sxs-lookup"><span data-stu-id="d8e07-206">packageId</span></span>|<span data-ttu-id="d8e07-207">String</span><span class="sxs-lookup"><span data-stu-id="d8e07-207">String</span></span>|<span data-ttu-id="d8e07-208">包标识符。</span><span class="sxs-lookup"><span data-stu-id="d8e07-208">The package identifier.</span></span> <span data-ttu-id="d8e07-209">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-209">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d8e07-210">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="d8e07-210">appIdentifier</span></span>|<span data-ttu-id="d8e07-211">String</span><span class="sxs-lookup"><span data-stu-id="d8e07-211">String</span></span>|<span data-ttu-id="d8e07-212">标识名称。</span><span class="sxs-lookup"><span data-stu-id="d8e07-212">The Identity Name.</span></span> <span data-ttu-id="d8e07-213">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-213">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d8e07-214">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d8e07-214">usedLicenseCount</span></span>|<span data-ttu-id="d8e07-215">Int32</span><span class="sxs-lookup"><span data-stu-id="d8e07-215">Int32</span></span>|<span data-ttu-id="d8e07-216">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="d8e07-216">The number of VPP licenses in use.</span></span> <span data-ttu-id="d8e07-217">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-217">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d8e07-218">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d8e07-218">totalLicenseCount</span></span>|<span data-ttu-id="d8e07-219">Int32</span><span class="sxs-lookup"><span data-stu-id="d8e07-219">Int32</span></span>|<span data-ttu-id="d8e07-220">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="d8e07-220">The total number of VPP licenses.</span></span> <span data-ttu-id="d8e07-221">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-221">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d8e07-222">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d8e07-222">appStoreUrl</span></span>|<span data-ttu-id="d8e07-223">String</span><span class="sxs-lookup"><span data-stu-id="d8e07-223">String</span></span>|<span data-ttu-id="d8e07-224">"播放工作商店" 应用程序 URL。</span><span class="sxs-lookup"><span data-stu-id="d8e07-224">The Play for Work Store app URL.</span></span> <span data-ttu-id="d8e07-225">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-225">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d8e07-226">isPrivate</span><span class="sxs-lookup"><span data-stu-id="d8e07-226">isPrivate</span></span>|<span data-ttu-id="d8e07-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8e07-227">Boolean</span></span>|<span data-ttu-id="d8e07-228">指示应用程序是否仅适用于给定企业的用户。</span><span class="sxs-lookup"><span data-stu-id="d8e07-228">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="d8e07-229">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-229">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d8e07-230">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="d8e07-230">isSystemApp</span></span>|<span data-ttu-id="d8e07-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8e07-231">Boolean</span></span>|<span data-ttu-id="d8e07-232">指示应用程序是否为预安装的系统应用程序。</span><span class="sxs-lookup"><span data-stu-id="d8e07-232">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="d8e07-233">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-233">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d8e07-234">appTracks</span><span class="sxs-lookup"><span data-stu-id="d8e07-234">appTracks</span></span>|<span data-ttu-id="d8e07-235">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md)集合</span><span class="sxs-lookup"><span data-stu-id="d8e07-235">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="d8e07-236">对此企业可见的曲目。</span><span class="sxs-lookup"><span data-stu-id="d8e07-236">The tracks that are visible to this enterprise.</span></span> <span data-ttu-id="d8e07-237">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-237">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d8e07-238">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="d8e07-238">supportsOemConfig</span></span>|<span data-ttu-id="d8e07-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8e07-239">Boolean</span></span>|<span data-ttu-id="d8e07-240">此应用是否支持 OEMConfig 策略。</span><span class="sxs-lookup"><span data-stu-id="d8e07-240">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="d8e07-241">继承自[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8e07-241">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d8e07-242">响应</span><span class="sxs-lookup"><span data-stu-id="d8e07-242">Response</span></span>
<span data-ttu-id="d8e07-243">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d8e07-243">If successful, this method returns a `201 Created` response code and a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8e07-244">示例</span><span class="sxs-lookup"><span data-stu-id="d8e07-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8e07-245">请求</span><span class="sxs-lookup"><span data-stu-id="d8e07-245">Request</span></span>
<span data-ttu-id="d8e07-246">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d8e07-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1171

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
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "Track Id value",
      "trackAlias": "Track Alias value"
    }
  ],
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="d8e07-247">响应</span><span class="sxs-lookup"><span data-stu-id="d8e07-247">Response</span></span>
<span data-ttu-id="d8e07-p128">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d8e07-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1343

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
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "Track Id value",
      "trackAlias": "Track Alias value"
    }
  ],
  "supportsOemConfig": true
}
```



