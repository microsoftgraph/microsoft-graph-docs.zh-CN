---
title: 创建 microsoftStoreForBusinessApp
description: 创建新的 microsoftStoreForBusinessApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 20df45fe0e56c965a082909035db0d6774eec116
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143456"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="a0ab4-103">创建 microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="a0ab4-103">Create microsoftStoreForBusinessApp</span></span>

<span data-ttu-id="a0ab4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0ab4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0ab4-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0ab4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0ab4-107">创建新的 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-107">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0ab4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a0ab4-108">Prerequisites</span></span>
<span data-ttu-id="a0ab4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0ab4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0ab4-111">Permission type</span></span>|<span data-ttu-id="a0ab4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0ab4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0ab4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0ab4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0ab4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0ab4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a0ab4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0ab4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0ab4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-116">Not supported.</span></span>|
|<span data-ttu-id="a0ab4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0ab4-117">Application</span></span>|<span data-ttu-id="a0ab4-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0ab4-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0ab4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0ab4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a0ab4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0ab4-120">Request headers</span></span>
|<span data-ttu-id="a0ab4-121">标头</span><span class="sxs-lookup"><span data-stu-id="a0ab4-121">Header</span></span>|<span data-ttu-id="a0ab4-122">值</span><span class="sxs-lookup"><span data-stu-id="a0ab4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0ab4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0ab4-123">Authorization</span></span>|<span data-ttu-id="a0ab4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0ab4-125">接受</span><span class="sxs-lookup"><span data-stu-id="a0ab4-125">Accept</span></span>|<span data-ttu-id="a0ab4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0ab4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0ab4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0ab4-127">Request body</span></span>
<span data-ttu-id="a0ab4-128">在请求正文中，提供 microsoftStoreForBusinessApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-128">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="a0ab4-129">下表显示了创建 microsoftStoreForBusinessApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-129">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="a0ab4-130">属性</span><span class="sxs-lookup"><span data-stu-id="a0ab4-130">Property</span></span>|<span data-ttu-id="a0ab4-131">类型</span><span class="sxs-lookup"><span data-stu-id="a0ab4-131">Type</span></span>|<span data-ttu-id="a0ab4-132">说明</span><span class="sxs-lookup"><span data-stu-id="a0ab4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0ab4-133">id</span><span class="sxs-lookup"><span data-stu-id="a0ab4-133">id</span></span>|<span data-ttu-id="a0ab4-134">String</span><span class="sxs-lookup"><span data-stu-id="a0ab4-134">String</span></span>|<span data-ttu-id="a0ab4-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-135">Key of the entity.</span></span> <span data-ttu-id="a0ab4-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a0ab4-137">displayName</span></span>|<span data-ttu-id="a0ab4-138">String</span><span class="sxs-lookup"><span data-stu-id="a0ab4-138">String</span></span>|<span data-ttu-id="a0ab4-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a0ab4-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-141">说明</span><span class="sxs-lookup"><span data-stu-id="a0ab4-141">description</span></span>|<span data-ttu-id="a0ab4-142">String</span><span class="sxs-lookup"><span data-stu-id="a0ab4-142">String</span></span>|<span data-ttu-id="a0ab4-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-143">The description of the app.</span></span> <span data-ttu-id="a0ab4-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-145">publisher</span><span class="sxs-lookup"><span data-stu-id="a0ab4-145">publisher</span></span>|<span data-ttu-id="a0ab4-146">String</span><span class="sxs-lookup"><span data-stu-id="a0ab4-146">String</span></span>|<span data-ttu-id="a0ab4-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-147">The publisher of the app.</span></span> <span data-ttu-id="a0ab4-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a0ab4-149">largeIcon</span></span>|[<span data-ttu-id="a0ab4-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a0ab4-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a0ab4-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a0ab4-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0ab4-153">createdDateTime</span></span>|<span data-ttu-id="a0ab4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0ab4-154">DateTimeOffset</span></span>|<span data-ttu-id="a0ab4-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-155">The date and time the app was created.</span></span> <span data-ttu-id="a0ab4-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0ab4-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a0ab4-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0ab4-158">DateTimeOffset</span></span>|<span data-ttu-id="a0ab4-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-159">The date and time the app was last modified.</span></span> <span data-ttu-id="a0ab4-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a0ab4-161">isFeatured</span></span>|<span data-ttu-id="a0ab4-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0ab4-162">Boolean</span></span>|<span data-ttu-id="a0ab4-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a0ab4-164">privacyInformationUrl</span></span>|<span data-ttu-id="a0ab4-165">String</span><span class="sxs-lookup"><span data-stu-id="a0ab4-165">String</span></span>|<span data-ttu-id="a0ab4-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-166">The privacy statement Url.</span></span> <span data-ttu-id="a0ab4-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a0ab4-168">informationUrl</span></span>|<span data-ttu-id="a0ab4-169">String</span><span class="sxs-lookup"><span data-stu-id="a0ab4-169">String</span></span>|<span data-ttu-id="a0ab4-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-170">The more information Url.</span></span> <span data-ttu-id="a0ab4-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-172">owner</span><span class="sxs-lookup"><span data-stu-id="a0ab4-172">owner</span></span>|<span data-ttu-id="a0ab4-173">String</span><span class="sxs-lookup"><span data-stu-id="a0ab4-173">String</span></span>|<span data-ttu-id="a0ab4-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-174">The owner of the app.</span></span> <span data-ttu-id="a0ab4-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-176">developer</span><span class="sxs-lookup"><span data-stu-id="a0ab4-176">developer</span></span>|<span data-ttu-id="a0ab4-177">String</span><span class="sxs-lookup"><span data-stu-id="a0ab4-177">String</span></span>|<span data-ttu-id="a0ab4-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-178">The developer of the app.</span></span> <span data-ttu-id="a0ab4-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-180">notes</span><span class="sxs-lookup"><span data-stu-id="a0ab4-180">notes</span></span>|<span data-ttu-id="a0ab4-181">String</span><span class="sxs-lookup"><span data-stu-id="a0ab4-181">String</span></span>|<span data-ttu-id="a0ab4-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-182">Notes for the app.</span></span> <span data-ttu-id="a0ab4-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="a0ab4-184">uploadState</span></span>|<span data-ttu-id="a0ab4-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a0ab4-185">Int32</span></span>|<span data-ttu-id="a0ab4-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-186">The upload state.</span></span> <span data-ttu-id="a0ab4-187">可能的值是：0 - `Not Ready` 、1 - `Ready` 、2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="a0ab4-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="a0ab4-189">publishingState</span></span>|[<span data-ttu-id="a0ab4-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a0ab4-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a0ab4-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-191">The publishing state for the app.</span></span> <span data-ttu-id="a0ab4-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a0ab4-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="a0ab4-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a0ab4-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a0ab4-195">isAssigned</span></span>|<span data-ttu-id="a0ab4-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0ab4-196">Boolean</span></span>|<span data-ttu-id="a0ab4-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a0ab4-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a0ab4-199">roleScopeTagIds</span></span>|<span data-ttu-id="a0ab4-200">String collection</span><span class="sxs-lookup"><span data-stu-id="a0ab4-200">String collection</span></span>|<span data-ttu-id="a0ab4-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a0ab4-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="a0ab4-203">dependentAppCount</span></span>|<span data-ttu-id="a0ab4-204">Int32</span><span class="sxs-lookup"><span data-stu-id="a0ab4-204">Int32</span></span>|<span data-ttu-id="a0ab4-205">子应用具有的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="a0ab4-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="a0ab4-207">supersedingAppCount</span></span>|<span data-ttu-id="a0ab4-208">Int32</span><span class="sxs-lookup"><span data-stu-id="a0ab4-208">Int32</span></span>|<span data-ttu-id="a0ab4-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="a0ab4-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="a0ab4-211">supersededAppCount</span></span>|<span data-ttu-id="a0ab4-212">Int32</span><span class="sxs-lookup"><span data-stu-id="a0ab4-212">Int32</span></span>|<span data-ttu-id="a0ab4-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="a0ab4-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0ab4-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0ab4-215">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a0ab4-215">usedLicenseCount</span></span>|<span data-ttu-id="a0ab4-216">Int32</span><span class="sxs-lookup"><span data-stu-id="a0ab4-216">Int32</span></span>|<span data-ttu-id="a0ab4-217">使用中的适用于企业的 Microsoft Store 许可证数。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-217">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="a0ab4-218">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a0ab4-218">totalLicenseCount</span></span>|<span data-ttu-id="a0ab4-219">Int32</span><span class="sxs-lookup"><span data-stu-id="a0ab4-219">Int32</span></span>|<span data-ttu-id="a0ab4-220">适用于企业的 Microsoft Store 许可证总数。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-220">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="a0ab4-221">productKey</span><span class="sxs-lookup"><span data-stu-id="a0ab4-221">productKey</span></span>|<span data-ttu-id="a0ab4-222">String</span><span class="sxs-lookup"><span data-stu-id="a0ab4-222">String</span></span>|<span data-ttu-id="a0ab4-223">应用产品密钥</span><span class="sxs-lookup"><span data-stu-id="a0ab4-223">The app product key</span></span>|
|<span data-ttu-id="a0ab4-224">licenseType</span><span class="sxs-lookup"><span data-stu-id="a0ab4-224">licenseType</span></span>|[<span data-ttu-id="a0ab4-225">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="a0ab4-225">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="a0ab4-226">应用程序许可证类型。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-226">The app license type.</span></span> <span data-ttu-id="a0ab4-227">可取值为：`offline`、`online`。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-227">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="a0ab4-228">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="a0ab4-228">packageIdentityName</span></span>|<span data-ttu-id="a0ab4-229">String</span><span class="sxs-lookup"><span data-stu-id="a0ab4-229">String</span></span>|<span data-ttu-id="a0ab4-230">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="a0ab4-230">The app package identifier</span></span>|
|<span data-ttu-id="a0ab4-231">licensingType</span><span class="sxs-lookup"><span data-stu-id="a0ab4-231">licensingType</span></span>|[<span data-ttu-id="a0ab4-232">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="a0ab4-232">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="a0ab4-233">受支持的许可证类型。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-233">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="a0ab4-234">响应</span><span class="sxs-lookup"><span data-stu-id="a0ab4-234">Response</span></span>
<span data-ttu-id="a0ab4-235">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-235">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0ab4-236">示例</span><span class="sxs-lookup"><span data-stu-id="a0ab4-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0ab4-237">请求</span><span class="sxs-lookup"><span data-stu-id="a0ab4-237">Request</span></span>
<span data-ttu-id="a0ab4-238">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1189

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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

### <a name="response"></a><span data-ttu-id="a0ab4-239">响应</span><span class="sxs-lookup"><span data-stu-id="a0ab4-239">Response</span></span>
<span data-ttu-id="a0ab4-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0ab4-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1361

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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




