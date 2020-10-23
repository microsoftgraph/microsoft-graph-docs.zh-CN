---
title: 创建 androidManagedStoreApp
description: 创建新的 androidManagedStoreApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6a75c85bd3f1e32bebff614f7a4eb19aa75e2af9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700680"
---
# <a name="create-androidmanagedstoreapp"></a><span data-ttu-id="61235-103">创建 androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="61235-103">Create androidManagedStoreApp</span></span>

<span data-ttu-id="61235-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61235-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61235-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="61235-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61235-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="61235-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61235-107">创建新的 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="61235-107">Create a new [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61235-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="61235-108">Prerequisites</span></span>
<span data-ttu-id="61235-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="61235-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61235-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="61235-111">Permission type</span></span>|<span data-ttu-id="61235-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="61235-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61235-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61235-113">Delegated (work or school account)</span></span>|<span data-ttu-id="61235-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61235-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="61235-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61235-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61235-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="61235-116">Not supported.</span></span>|
|<span data-ttu-id="61235-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="61235-117">Application</span></span>|<span data-ttu-id="61235-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61235-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61235-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61235-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="61235-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="61235-120">Request headers</span></span>
|<span data-ttu-id="61235-121">标头</span><span class="sxs-lookup"><span data-stu-id="61235-121">Header</span></span>|<span data-ttu-id="61235-122">值</span><span class="sxs-lookup"><span data-stu-id="61235-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61235-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="61235-123">Authorization</span></span>|<span data-ttu-id="61235-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="61235-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61235-125">接受</span><span class="sxs-lookup"><span data-stu-id="61235-125">Accept</span></span>|<span data-ttu-id="61235-126">application/json</span><span class="sxs-lookup"><span data-stu-id="61235-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61235-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="61235-127">Request body</span></span>
<span data-ttu-id="61235-128">在请求正文中，提供 androidManagedStoreApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61235-128">In the request body, supply a JSON representation for the androidManagedStoreApp object.</span></span>

<span data-ttu-id="61235-129">下表显示创建 androidManagedStoreApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="61235-129">The following table shows the properties that are required when you create the androidManagedStoreApp.</span></span>

|<span data-ttu-id="61235-130">属性</span><span class="sxs-lookup"><span data-stu-id="61235-130">Property</span></span>|<span data-ttu-id="61235-131">类型</span><span class="sxs-lookup"><span data-stu-id="61235-131">Type</span></span>|<span data-ttu-id="61235-132">说明</span><span class="sxs-lookup"><span data-stu-id="61235-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61235-133">id</span><span class="sxs-lookup"><span data-stu-id="61235-133">id</span></span>|<span data-ttu-id="61235-134">String</span><span class="sxs-lookup"><span data-stu-id="61235-134">String</span></span>|<span data-ttu-id="61235-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="61235-135">Key of the entity.</span></span> <span data-ttu-id="61235-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-137">displayName</span><span class="sxs-lookup"><span data-stu-id="61235-137">displayName</span></span>|<span data-ttu-id="61235-138">String</span><span class="sxs-lookup"><span data-stu-id="61235-138">String</span></span>|<span data-ttu-id="61235-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="61235-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="61235-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-141">说明</span><span class="sxs-lookup"><span data-stu-id="61235-141">description</span></span>|<span data-ttu-id="61235-142">String</span><span class="sxs-lookup"><span data-stu-id="61235-142">String</span></span>|<span data-ttu-id="61235-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="61235-143">The description of the app.</span></span> <span data-ttu-id="61235-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-145">publisher</span><span class="sxs-lookup"><span data-stu-id="61235-145">publisher</span></span>|<span data-ttu-id="61235-146">String</span><span class="sxs-lookup"><span data-stu-id="61235-146">String</span></span>|<span data-ttu-id="61235-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="61235-147">The publisher of the app.</span></span> <span data-ttu-id="61235-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="61235-149">largeIcon</span></span>|[<span data-ttu-id="61235-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="61235-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="61235-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="61235-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="61235-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61235-153">createdDateTime</span></span>|<span data-ttu-id="61235-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61235-154">DateTimeOffset</span></span>|<span data-ttu-id="61235-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="61235-155">The date and time the app was created.</span></span> <span data-ttu-id="61235-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61235-157">lastModifiedDateTime</span></span>|<span data-ttu-id="61235-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61235-158">DateTimeOffset</span></span>|<span data-ttu-id="61235-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="61235-159">The date and time the app was last modified.</span></span> <span data-ttu-id="61235-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="61235-161">isFeatured</span></span>|<span data-ttu-id="61235-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="61235-162">Boolean</span></span>|<span data-ttu-id="61235-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="61235-164">privacyInformationUrl</span></span>|<span data-ttu-id="61235-165">String</span><span class="sxs-lookup"><span data-stu-id="61235-165">String</span></span>|<span data-ttu-id="61235-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="61235-166">The privacy statement Url.</span></span> <span data-ttu-id="61235-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="61235-168">informationUrl</span></span>|<span data-ttu-id="61235-169">String</span><span class="sxs-lookup"><span data-stu-id="61235-169">String</span></span>|<span data-ttu-id="61235-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="61235-170">The more information Url.</span></span> <span data-ttu-id="61235-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-172">owner</span><span class="sxs-lookup"><span data-stu-id="61235-172">owner</span></span>|<span data-ttu-id="61235-173">String</span><span class="sxs-lookup"><span data-stu-id="61235-173">String</span></span>|<span data-ttu-id="61235-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="61235-174">The owner of the app.</span></span> <span data-ttu-id="61235-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-176">developer</span><span class="sxs-lookup"><span data-stu-id="61235-176">developer</span></span>|<span data-ttu-id="61235-177">String</span><span class="sxs-lookup"><span data-stu-id="61235-177">String</span></span>|<span data-ttu-id="61235-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="61235-178">The developer of the app.</span></span> <span data-ttu-id="61235-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-180">notes</span><span class="sxs-lookup"><span data-stu-id="61235-180">notes</span></span>|<span data-ttu-id="61235-181">String</span><span class="sxs-lookup"><span data-stu-id="61235-181">String</span></span>|<span data-ttu-id="61235-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="61235-182">Notes for the app.</span></span> <span data-ttu-id="61235-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="61235-184">uploadState</span></span>|<span data-ttu-id="61235-185">Int32</span><span class="sxs-lookup"><span data-stu-id="61235-185">Int32</span></span>|<span data-ttu-id="61235-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="61235-186">The upload state.</span></span> <span data-ttu-id="61235-187">可能的值包括： 0- `Not Ready` 、1- `Ready` 、2- `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="61235-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="61235-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="61235-189">publishingState</span></span>|[<span data-ttu-id="61235-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="61235-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="61235-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="61235-191">The publishing state for the app.</span></span> <span data-ttu-id="61235-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="61235-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="61235-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="61235-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="61235-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="61235-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="61235-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="61235-195">isAssigned</span></span>|<span data-ttu-id="61235-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="61235-196">Boolean</span></span>|<span data-ttu-id="61235-197">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="61235-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="61235-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="61235-199">roleScopeTagIds</span></span>|<span data-ttu-id="61235-200">String collection</span><span class="sxs-lookup"><span data-stu-id="61235-200">String collection</span></span>|<span data-ttu-id="61235-201">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="61235-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="61235-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="61235-203">dependentAppCount</span></span>|<span data-ttu-id="61235-204">Int32</span><span class="sxs-lookup"><span data-stu-id="61235-204">Int32</span></span>|<span data-ttu-id="61235-205">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="61235-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="61235-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="61235-207">supersedingAppCount</span></span>|<span data-ttu-id="61235-208">Int32</span><span class="sxs-lookup"><span data-stu-id="61235-208">Int32</span></span>|<span data-ttu-id="61235-209">此应用程序直接或间接取代的应用程序总数量。</span><span class="sxs-lookup"><span data-stu-id="61235-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="61235-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="61235-211">supersededAppCount</span></span>|<span data-ttu-id="61235-212">Int32</span><span class="sxs-lookup"><span data-stu-id="61235-212">Int32</span></span>|<span data-ttu-id="61235-213">此应用程序直接或间接取代的应用程序总数量。</span><span class="sxs-lookup"><span data-stu-id="61235-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="61235-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61235-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61235-215">packageId</span><span class="sxs-lookup"><span data-stu-id="61235-215">packageId</span></span>|<span data-ttu-id="61235-216">String</span><span class="sxs-lookup"><span data-stu-id="61235-216">String</span></span>|<span data-ttu-id="61235-217">包标识符。</span><span class="sxs-lookup"><span data-stu-id="61235-217">The package identifier.</span></span>|
|<span data-ttu-id="61235-218">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="61235-218">appIdentifier</span></span>|<span data-ttu-id="61235-219">String</span><span class="sxs-lookup"><span data-stu-id="61235-219">String</span></span>|<span data-ttu-id="61235-220">标识名称。</span><span class="sxs-lookup"><span data-stu-id="61235-220">The Identity Name.</span></span>|
|<span data-ttu-id="61235-221">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="61235-221">usedLicenseCount</span></span>|<span data-ttu-id="61235-222">Int32</span><span class="sxs-lookup"><span data-stu-id="61235-222">Int32</span></span>|<span data-ttu-id="61235-223">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="61235-223">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="61235-224">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="61235-224">totalLicenseCount</span></span>|<span data-ttu-id="61235-225">Int32</span><span class="sxs-lookup"><span data-stu-id="61235-225">Int32</span></span>|<span data-ttu-id="61235-226">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="61235-226">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="61235-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="61235-227">appStoreUrl</span></span>|<span data-ttu-id="61235-228">String</span><span class="sxs-lookup"><span data-stu-id="61235-228">String</span></span>|<span data-ttu-id="61235-229">"播放工作商店" 应用程序 URL。</span><span class="sxs-lookup"><span data-stu-id="61235-229">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="61235-230">isPrivate</span><span class="sxs-lookup"><span data-stu-id="61235-230">isPrivate</span></span>|<span data-ttu-id="61235-231">布尔</span><span class="sxs-lookup"><span data-stu-id="61235-231">Boolean</span></span>|<span data-ttu-id="61235-232">指示应用程序是否仅适用于给定企业的用户。</span><span class="sxs-lookup"><span data-stu-id="61235-232">Indicates whether the app is only available to a given enterprise's users.</span></span>|
|<span data-ttu-id="61235-233">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="61235-233">isSystemApp</span></span>|<span data-ttu-id="61235-234">布尔</span><span class="sxs-lookup"><span data-stu-id="61235-234">Boolean</span></span>|<span data-ttu-id="61235-235">指示应用程序是否为预安装的系统应用程序。</span><span class="sxs-lookup"><span data-stu-id="61235-235">Indicates whether the app is a preinstalled system app.</span></span>|
|<span data-ttu-id="61235-236">appTracks</span><span class="sxs-lookup"><span data-stu-id="61235-236">appTracks</span></span>|<span data-ttu-id="61235-237">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) 集合</span><span class="sxs-lookup"><span data-stu-id="61235-237">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="61235-238">对此企业可见的曲目。</span><span class="sxs-lookup"><span data-stu-id="61235-238">The tracks that are visible to this enterprise.</span></span>|
|<span data-ttu-id="61235-239">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="61235-239">supportsOemConfig</span></span>|<span data-ttu-id="61235-240">布尔</span><span class="sxs-lookup"><span data-stu-id="61235-240">Boolean</span></span>|<span data-ttu-id="61235-241">此应用是否支持 OEMConfig 策略。</span><span class="sxs-lookup"><span data-stu-id="61235-241">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="61235-242">响应</span><span class="sxs-lookup"><span data-stu-id="61235-242">Response</span></span>
<span data-ttu-id="61235-243">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="61235-243">If successful, this method returns a `201 Created` response code and a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61235-244">示例</span><span class="sxs-lookup"><span data-stu-id="61235-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="61235-245">请求</span><span class="sxs-lookup"><span data-stu-id="61235-245">Request</span></span>
<span data-ttu-id="61235-246">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="61235-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1225

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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

### <a name="response"></a><span data-ttu-id="61235-247">响应</span><span class="sxs-lookup"><span data-stu-id="61235-247">Response</span></span>
<span data-ttu-id="61235-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="61235-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1397

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
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





