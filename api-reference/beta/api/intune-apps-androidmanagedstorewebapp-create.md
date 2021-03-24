---
title: 创建 androidManagedStoreWebApp
description: 创建新的 androidManagedStoreWebApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02c2ef44ea107529e40dd4a3f0d0ed0767f25979
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144380"
---
# <a name="create-androidmanagedstorewebapp"></a><span data-ttu-id="07a6a-103">创建 androidManagedStoreWebApp</span><span class="sxs-lookup"><span data-stu-id="07a6a-103">Create androidManagedStoreWebApp</span></span>

<span data-ttu-id="07a6a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07a6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07a6a-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="07a6a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07a6a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07a6a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07a6a-107">创建新的 [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07a6a-107">Create a new [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07a6a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="07a6a-108">Prerequisites</span></span>
<span data-ttu-id="07a6a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07a6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07a6a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="07a6a-111">Permission type</span></span>|<span data-ttu-id="07a6a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07a6a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07a6a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07a6a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07a6a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07a6a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="07a6a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07a6a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07a6a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="07a6a-116">Not supported.</span></span>|
|<span data-ttu-id="07a6a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="07a6a-117">Application</span></span>|<span data-ttu-id="07a6a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07a6a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07a6a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07a6a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="07a6a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="07a6a-120">Request headers</span></span>
|<span data-ttu-id="07a6a-121">标头</span><span class="sxs-lookup"><span data-stu-id="07a6a-121">Header</span></span>|<span data-ttu-id="07a6a-122">值</span><span class="sxs-lookup"><span data-stu-id="07a6a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07a6a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="07a6a-123">Authorization</span></span>|<span data-ttu-id="07a6a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="07a6a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07a6a-125">接受</span><span class="sxs-lookup"><span data-stu-id="07a6a-125">Accept</span></span>|<span data-ttu-id="07a6a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07a6a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07a6a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="07a6a-127">Request body</span></span>
<span data-ttu-id="07a6a-128">在请求正文中，提供 androidManagedStoreWebApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07a6a-128">In the request body, supply a JSON representation for the androidManagedStoreWebApp object.</span></span>

<span data-ttu-id="07a6a-129">下表显示创建 androidManagedStoreWebApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="07a6a-129">The following table shows the properties that are required when you create the androidManagedStoreWebApp.</span></span>

|<span data-ttu-id="07a6a-130">属性</span><span class="sxs-lookup"><span data-stu-id="07a6a-130">Property</span></span>|<span data-ttu-id="07a6a-131">类型</span><span class="sxs-lookup"><span data-stu-id="07a6a-131">Type</span></span>|<span data-ttu-id="07a6a-132">说明</span><span class="sxs-lookup"><span data-stu-id="07a6a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07a6a-133">id</span><span class="sxs-lookup"><span data-stu-id="07a6a-133">id</span></span>|<span data-ttu-id="07a6a-134">String</span><span class="sxs-lookup"><span data-stu-id="07a6a-134">String</span></span>|<span data-ttu-id="07a6a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="07a6a-135">Key of the entity.</span></span> <span data-ttu-id="07a6a-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="07a6a-137">displayName</span></span>|<span data-ttu-id="07a6a-138">String</span><span class="sxs-lookup"><span data-stu-id="07a6a-138">String</span></span>|<span data-ttu-id="07a6a-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="07a6a-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="07a6a-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-141">说明</span><span class="sxs-lookup"><span data-stu-id="07a6a-141">description</span></span>|<span data-ttu-id="07a6a-142">String</span><span class="sxs-lookup"><span data-stu-id="07a6a-142">String</span></span>|<span data-ttu-id="07a6a-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="07a6a-143">The description of the app.</span></span> <span data-ttu-id="07a6a-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-145">publisher</span><span class="sxs-lookup"><span data-stu-id="07a6a-145">publisher</span></span>|<span data-ttu-id="07a6a-146">String</span><span class="sxs-lookup"><span data-stu-id="07a6a-146">String</span></span>|<span data-ttu-id="07a6a-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="07a6a-147">The publisher of the app.</span></span> <span data-ttu-id="07a6a-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="07a6a-149">largeIcon</span></span>|[<span data-ttu-id="07a6a-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="07a6a-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="07a6a-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="07a6a-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="07a6a-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07a6a-153">createdDateTime</span></span>|<span data-ttu-id="07a6a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07a6a-154">DateTimeOffset</span></span>|<span data-ttu-id="07a6a-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="07a6a-155">The date and time the app was created.</span></span> <span data-ttu-id="07a6a-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07a6a-157">lastModifiedDateTime</span></span>|<span data-ttu-id="07a6a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07a6a-158">DateTimeOffset</span></span>|<span data-ttu-id="07a6a-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="07a6a-159">The date and time the app was last modified.</span></span> <span data-ttu-id="07a6a-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="07a6a-161">isFeatured</span></span>|<span data-ttu-id="07a6a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="07a6a-162">Boolean</span></span>|<span data-ttu-id="07a6a-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="07a6a-164">privacyInformationUrl</span></span>|<span data-ttu-id="07a6a-165">String</span><span class="sxs-lookup"><span data-stu-id="07a6a-165">String</span></span>|<span data-ttu-id="07a6a-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="07a6a-166">The privacy statement Url.</span></span> <span data-ttu-id="07a6a-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="07a6a-168">informationUrl</span></span>|<span data-ttu-id="07a6a-169">String</span><span class="sxs-lookup"><span data-stu-id="07a6a-169">String</span></span>|<span data-ttu-id="07a6a-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="07a6a-170">The more information Url.</span></span> <span data-ttu-id="07a6a-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-172">owner</span><span class="sxs-lookup"><span data-stu-id="07a6a-172">owner</span></span>|<span data-ttu-id="07a6a-173">String</span><span class="sxs-lookup"><span data-stu-id="07a6a-173">String</span></span>|<span data-ttu-id="07a6a-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="07a6a-174">The owner of the app.</span></span> <span data-ttu-id="07a6a-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-176">developer</span><span class="sxs-lookup"><span data-stu-id="07a6a-176">developer</span></span>|<span data-ttu-id="07a6a-177">String</span><span class="sxs-lookup"><span data-stu-id="07a6a-177">String</span></span>|<span data-ttu-id="07a6a-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="07a6a-178">The developer of the app.</span></span> <span data-ttu-id="07a6a-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-180">notes</span><span class="sxs-lookup"><span data-stu-id="07a6a-180">notes</span></span>|<span data-ttu-id="07a6a-181">String</span><span class="sxs-lookup"><span data-stu-id="07a6a-181">String</span></span>|<span data-ttu-id="07a6a-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="07a6a-182">Notes for the app.</span></span> <span data-ttu-id="07a6a-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="07a6a-184">uploadState</span></span>|<span data-ttu-id="07a6a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="07a6a-185">Int32</span></span>|<span data-ttu-id="07a6a-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="07a6a-186">The upload state.</span></span> <span data-ttu-id="07a6a-187">可能的值是：0 - `Not Ready` 、1 - `Ready` 、2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="07a6a-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="07a6a-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="07a6a-189">publishingState</span></span>|[<span data-ttu-id="07a6a-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="07a6a-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="07a6a-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="07a6a-191">The publishing state for the app.</span></span> <span data-ttu-id="07a6a-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="07a6a-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="07a6a-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="07a6a-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="07a6a-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="07a6a-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="07a6a-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="07a6a-195">isAssigned</span></span>|<span data-ttu-id="07a6a-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="07a6a-196">Boolean</span></span>|<span data-ttu-id="07a6a-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="07a6a-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="07a6a-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="07a6a-199">roleScopeTagIds</span></span>|<span data-ttu-id="07a6a-200">String collection</span><span class="sxs-lookup"><span data-stu-id="07a6a-200">String collection</span></span>|<span data-ttu-id="07a6a-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="07a6a-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="07a6a-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="07a6a-203">dependentAppCount</span></span>|<span data-ttu-id="07a6a-204">Int32</span><span class="sxs-lookup"><span data-stu-id="07a6a-204">Int32</span></span>|<span data-ttu-id="07a6a-205">子应用具有的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="07a6a-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="07a6a-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="07a6a-207">supersedingAppCount</span></span>|<span data-ttu-id="07a6a-208">Int32</span><span class="sxs-lookup"><span data-stu-id="07a6a-208">Int32</span></span>|<span data-ttu-id="07a6a-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="07a6a-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="07a6a-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="07a6a-211">supersededAppCount</span></span>|<span data-ttu-id="07a6a-212">Int32</span><span class="sxs-lookup"><span data-stu-id="07a6a-212">Int32</span></span>|<span data-ttu-id="07a6a-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="07a6a-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="07a6a-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07a6a-215">packageId</span><span class="sxs-lookup"><span data-stu-id="07a6a-215">packageId</span></span>|<span data-ttu-id="07a6a-216">String</span><span class="sxs-lookup"><span data-stu-id="07a6a-216">String</span></span>|<span data-ttu-id="07a6a-217">包标识符。</span><span class="sxs-lookup"><span data-stu-id="07a6a-217">The package identifier.</span></span> <span data-ttu-id="07a6a-218">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-218">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="07a6a-219">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="07a6a-219">appIdentifier</span></span>|<span data-ttu-id="07a6a-220">String</span><span class="sxs-lookup"><span data-stu-id="07a6a-220">String</span></span>|<span data-ttu-id="07a6a-221">标识名称。</span><span class="sxs-lookup"><span data-stu-id="07a6a-221">The Identity Name.</span></span> <span data-ttu-id="07a6a-222">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-222">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="07a6a-223">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="07a6a-223">usedLicenseCount</span></span>|<span data-ttu-id="07a6a-224">Int32</span><span class="sxs-lookup"><span data-stu-id="07a6a-224">Int32</span></span>|<span data-ttu-id="07a6a-225">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="07a6a-225">The number of VPP licenses in use.</span></span> <span data-ttu-id="07a6a-226">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-226">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="07a6a-227">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="07a6a-227">totalLicenseCount</span></span>|<span data-ttu-id="07a6a-228">Int32</span><span class="sxs-lookup"><span data-stu-id="07a6a-228">Int32</span></span>|<span data-ttu-id="07a6a-229">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="07a6a-229">The total number of VPP licenses.</span></span> <span data-ttu-id="07a6a-230">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-230">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="07a6a-231">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="07a6a-231">appStoreUrl</span></span>|<span data-ttu-id="07a6a-232">String</span><span class="sxs-lookup"><span data-stu-id="07a6a-232">String</span></span>|<span data-ttu-id="07a6a-233">"播放工作商店"应用 URL。</span><span class="sxs-lookup"><span data-stu-id="07a6a-233">The Play for Work Store app URL.</span></span> <span data-ttu-id="07a6a-234">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-234">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="07a6a-235">isPrivate</span><span class="sxs-lookup"><span data-stu-id="07a6a-235">isPrivate</span></span>|<span data-ttu-id="07a6a-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="07a6a-236">Boolean</span></span>|<span data-ttu-id="07a6a-237">指示应用是否仅适用于给定企业的用户。</span><span class="sxs-lookup"><span data-stu-id="07a6a-237">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="07a6a-238">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-238">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="07a6a-239">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="07a6a-239">isSystemApp</span></span>|<span data-ttu-id="07a6a-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="07a6a-240">Boolean</span></span>|<span data-ttu-id="07a6a-241">指示应用是否是预安装的系统应用。</span><span class="sxs-lookup"><span data-stu-id="07a6a-241">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="07a6a-242">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-242">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="07a6a-243">appTracks</span><span class="sxs-lookup"><span data-stu-id="07a6a-243">appTracks</span></span>|<span data-ttu-id="07a6a-244">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) 集合</span><span class="sxs-lookup"><span data-stu-id="07a6a-244">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="07a6a-245">此企业可见的轨。</span><span class="sxs-lookup"><span data-stu-id="07a6a-245">The tracks that are visible to this enterprise.</span></span> <span data-ttu-id="07a6a-246">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-246">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="07a6a-247">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="07a6a-247">supportsOemConfig</span></span>|<span data-ttu-id="07a6a-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="07a6a-248">Boolean</span></span>|<span data-ttu-id="07a6a-249">此应用是否支持 OEMConfig 策略。</span><span class="sxs-lookup"><span data-stu-id="07a6a-249">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="07a6a-250">继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="07a6a-250">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="07a6a-251">响应</span><span class="sxs-lookup"><span data-stu-id="07a6a-251">Response</span></span>
<span data-ttu-id="07a6a-252">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07a6a-252">If successful, this method returns a `201 Created` response code and a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07a6a-253">示例</span><span class="sxs-lookup"><span data-stu-id="07a6a-253">Example</span></span>

### <a name="request"></a><span data-ttu-id="07a6a-254">请求</span><span class="sxs-lookup"><span data-stu-id="07a6a-254">Request</span></span>
<span data-ttu-id="07a6a-255">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="07a6a-255">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1228

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

### <a name="response"></a><span data-ttu-id="07a6a-256">响应</span><span class="sxs-lookup"><span data-stu-id="07a6a-256">Response</span></span>
<span data-ttu-id="07a6a-p130">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="07a6a-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1400

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




