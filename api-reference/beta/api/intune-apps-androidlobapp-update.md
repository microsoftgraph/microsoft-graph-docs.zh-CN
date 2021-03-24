---
title: 更新 androidLobApp
description: 更新 androidLobApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 535cb37ea2ff4ad3e11ea11d03fafbf5ea3a6801
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140992"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="d9e49-103">更新 androidLobApp</span><span class="sxs-lookup"><span data-stu-id="d9e49-103">Update androidLobApp</span></span>

<span data-ttu-id="d9e49-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9e49-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9e49-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d9e49-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9e49-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d9e49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9e49-107">更新 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d9e49-107">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9e49-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d9e49-108">Prerequisites</span></span>
<span data-ttu-id="d9e49-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9e49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9e49-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9e49-111">Permission type</span></span>|<span data-ttu-id="d9e49-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d9e49-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9e49-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9e49-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9e49-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9e49-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d9e49-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9e49-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9e49-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9e49-116">Not supported.</span></span>|
|<span data-ttu-id="d9e49-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9e49-117">Application</span></span>|<span data-ttu-id="d9e49-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9e49-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9e49-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9e49-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="d9e49-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9e49-120">Request headers</span></span>
|<span data-ttu-id="d9e49-121">标头</span><span class="sxs-lookup"><span data-stu-id="d9e49-121">Header</span></span>|<span data-ttu-id="d9e49-122">值</span><span class="sxs-lookup"><span data-stu-id="d9e49-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9e49-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9e49-123">Authorization</span></span>|<span data-ttu-id="d9e49-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d9e49-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9e49-125">接受</span><span class="sxs-lookup"><span data-stu-id="d9e49-125">Accept</span></span>|<span data-ttu-id="d9e49-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9e49-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9e49-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9e49-127">Request body</span></span>
<span data-ttu-id="d9e49-128">在请求正文中，提供 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9e49-128">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="d9e49-129">下表显示了创建 [androidLobApp](../resources/intune-apps-androidlobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d9e49-129">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="d9e49-130">属性</span><span class="sxs-lookup"><span data-stu-id="d9e49-130">Property</span></span>|<span data-ttu-id="d9e49-131">类型</span><span class="sxs-lookup"><span data-stu-id="d9e49-131">Type</span></span>|<span data-ttu-id="d9e49-132">说明</span><span class="sxs-lookup"><span data-stu-id="d9e49-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9e49-133">id</span><span class="sxs-lookup"><span data-stu-id="d9e49-133">id</span></span>|<span data-ttu-id="d9e49-134">String</span><span class="sxs-lookup"><span data-stu-id="d9e49-134">String</span></span>|<span data-ttu-id="d9e49-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d9e49-135">Key of the entity.</span></span> <span data-ttu-id="d9e49-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d9e49-137">displayName</span></span>|<span data-ttu-id="d9e49-138">String</span><span class="sxs-lookup"><span data-stu-id="d9e49-138">String</span></span>|<span data-ttu-id="d9e49-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="d9e49-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d9e49-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-141">说明</span><span class="sxs-lookup"><span data-stu-id="d9e49-141">description</span></span>|<span data-ttu-id="d9e49-142">String</span><span class="sxs-lookup"><span data-stu-id="d9e49-142">String</span></span>|<span data-ttu-id="d9e49-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="d9e49-143">The description of the app.</span></span> <span data-ttu-id="d9e49-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-145">publisher</span><span class="sxs-lookup"><span data-stu-id="d9e49-145">publisher</span></span>|<span data-ttu-id="d9e49-146">String</span><span class="sxs-lookup"><span data-stu-id="d9e49-146">String</span></span>|<span data-ttu-id="d9e49-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="d9e49-147">The publisher of the app.</span></span> <span data-ttu-id="d9e49-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d9e49-149">largeIcon</span></span>|[<span data-ttu-id="d9e49-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d9e49-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d9e49-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="d9e49-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d9e49-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9e49-153">createdDateTime</span></span>|<span data-ttu-id="d9e49-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9e49-154">DateTimeOffset</span></span>|<span data-ttu-id="d9e49-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d9e49-155">The date and time the app was created.</span></span> <span data-ttu-id="d9e49-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9e49-157">lastModifiedDateTime</span></span>|<span data-ttu-id="d9e49-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9e49-158">DateTimeOffset</span></span>|<span data-ttu-id="d9e49-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d9e49-159">The date and time the app was last modified.</span></span> <span data-ttu-id="d9e49-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d9e49-161">isFeatured</span></span>|<span data-ttu-id="d9e49-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9e49-162">Boolean</span></span>|<span data-ttu-id="d9e49-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d9e49-164">privacyInformationUrl</span></span>|<span data-ttu-id="d9e49-165">String</span><span class="sxs-lookup"><span data-stu-id="d9e49-165">String</span></span>|<span data-ttu-id="d9e49-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="d9e49-166">The privacy statement Url.</span></span> <span data-ttu-id="d9e49-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d9e49-168">informationUrl</span></span>|<span data-ttu-id="d9e49-169">String</span><span class="sxs-lookup"><span data-stu-id="d9e49-169">String</span></span>|<span data-ttu-id="d9e49-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="d9e49-170">The more information Url.</span></span> <span data-ttu-id="d9e49-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-172">owner</span><span class="sxs-lookup"><span data-stu-id="d9e49-172">owner</span></span>|<span data-ttu-id="d9e49-173">String</span><span class="sxs-lookup"><span data-stu-id="d9e49-173">String</span></span>|<span data-ttu-id="d9e49-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="d9e49-174">The owner of the app.</span></span> <span data-ttu-id="d9e49-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-176">developer</span><span class="sxs-lookup"><span data-stu-id="d9e49-176">developer</span></span>|<span data-ttu-id="d9e49-177">String</span><span class="sxs-lookup"><span data-stu-id="d9e49-177">String</span></span>|<span data-ttu-id="d9e49-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="d9e49-178">The developer of the app.</span></span> <span data-ttu-id="d9e49-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-180">notes</span><span class="sxs-lookup"><span data-stu-id="d9e49-180">notes</span></span>|<span data-ttu-id="d9e49-181">String</span><span class="sxs-lookup"><span data-stu-id="d9e49-181">String</span></span>|<span data-ttu-id="d9e49-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="d9e49-182">Notes for the app.</span></span> <span data-ttu-id="d9e49-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="d9e49-184">uploadState</span></span>|<span data-ttu-id="d9e49-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d9e49-185">Int32</span></span>|<span data-ttu-id="d9e49-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="d9e49-186">The upload state.</span></span> <span data-ttu-id="d9e49-187">可能的值是：0 - `Not Ready` 、1 - `Ready` 、2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="d9e49-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="d9e49-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="d9e49-189">publishingState</span></span>|[<span data-ttu-id="d9e49-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d9e49-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d9e49-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="d9e49-191">The publishing state for the app.</span></span> <span data-ttu-id="d9e49-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="d9e49-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d9e49-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="d9e49-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="d9e49-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="d9e49-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d9e49-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d9e49-195">isAssigned</span></span>|<span data-ttu-id="d9e49-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9e49-196">Boolean</span></span>|<span data-ttu-id="d9e49-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="d9e49-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d9e49-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d9e49-199">roleScopeTagIds</span></span>|<span data-ttu-id="d9e49-200">String collection</span><span class="sxs-lookup"><span data-stu-id="d9e49-200">String collection</span></span>|<span data-ttu-id="d9e49-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="d9e49-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d9e49-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="d9e49-203">dependentAppCount</span></span>|<span data-ttu-id="d9e49-204">Int32</span><span class="sxs-lookup"><span data-stu-id="d9e49-204">Int32</span></span>|<span data-ttu-id="d9e49-205">子应用具有的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="d9e49-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="d9e49-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="d9e49-207">supersedingAppCount</span></span>|<span data-ttu-id="d9e49-208">Int32</span><span class="sxs-lookup"><span data-stu-id="d9e49-208">Int32</span></span>|<span data-ttu-id="d9e49-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="d9e49-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="d9e49-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="d9e49-211">supersededAppCount</span></span>|<span data-ttu-id="d9e49-212">Int32</span><span class="sxs-lookup"><span data-stu-id="d9e49-212">Int32</span></span>|<span data-ttu-id="d9e49-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="d9e49-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="d9e49-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e49-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d9e49-215">committedContentVersion</span></span>|<span data-ttu-id="d9e49-216">String</span><span class="sxs-lookup"><span data-stu-id="d9e49-216">String</span></span>|<span data-ttu-id="d9e49-217">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="d9e49-217">The internal committed content version.</span></span> <span data-ttu-id="d9e49-218">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d9e49-219">fileName</span><span class="sxs-lookup"><span data-stu-id="d9e49-219">fileName</span></span>|<span data-ttu-id="d9e49-220">String</span><span class="sxs-lookup"><span data-stu-id="d9e49-220">String</span></span>|<span data-ttu-id="d9e49-221">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="d9e49-221">The name of the main Lob application file.</span></span> <span data-ttu-id="d9e49-222">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d9e49-223">size</span><span class="sxs-lookup"><span data-stu-id="d9e49-223">size</span></span>|<span data-ttu-id="d9e49-224">Int64</span><span class="sxs-lookup"><span data-stu-id="d9e49-224">Int64</span></span>|<span data-ttu-id="d9e49-225">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="d9e49-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="d9e49-226">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e49-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d9e49-227">packageId</span><span class="sxs-lookup"><span data-stu-id="d9e49-227">packageId</span></span>|<span data-ttu-id="d9e49-228">String</span><span class="sxs-lookup"><span data-stu-id="d9e49-228">String</span></span>|<span data-ttu-id="d9e49-229">包标识符。</span><span class="sxs-lookup"><span data-stu-id="d9e49-229">The package identifier.</span></span>|
|<span data-ttu-id="d9e49-230">identityName</span><span class="sxs-lookup"><span data-stu-id="d9e49-230">identityName</span></span>|<span data-ttu-id="d9e49-231">String</span><span class="sxs-lookup"><span data-stu-id="d9e49-231">String</span></span>|<span data-ttu-id="d9e49-232">标识名称。</span><span class="sxs-lookup"><span data-stu-id="d9e49-232">The Identity Name.</span></span>|
|<span data-ttu-id="d9e49-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d9e49-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d9e49-234">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d9e49-234">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="d9e49-235">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="d9e49-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="d9e49-236">versionName</span><span class="sxs-lookup"><span data-stu-id="d9e49-236">versionName</span></span>|<span data-ttu-id="d9e49-237">String</span><span class="sxs-lookup"><span data-stu-id="d9e49-237">String</span></span>|<span data-ttu-id="d9e49-238">Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="d9e49-238">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d9e49-239">versionCode</span><span class="sxs-lookup"><span data-stu-id="d9e49-239">versionCode</span></span>|<span data-ttu-id="d9e49-240">String</span><span class="sxs-lookup"><span data-stu-id="d9e49-240">String</span></span>|<span data-ttu-id="d9e49-241">Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="d9e49-241">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d9e49-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="d9e49-242">identityVersion</span></span>|<span data-ttu-id="d9e49-243">String</span><span class="sxs-lookup"><span data-stu-id="d9e49-243">String</span></span>|<span data-ttu-id="d9e49-244">标识版本。</span><span class="sxs-lookup"><span data-stu-id="d9e49-244">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="d9e49-245">响应</span><span class="sxs-lookup"><span data-stu-id="d9e49-245">Response</span></span>
<span data-ttu-id="d9e49-246">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidLobApp](../resources/intune-apps-androidlobapp.md)  对象。</span><span class="sxs-lookup"><span data-stu-id="d9e49-246">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9e49-247">示例</span><span class="sxs-lookup"><span data-stu-id="d9e49-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9e49-248">请求</span><span class="sxs-lookup"><span data-stu-id="d9e49-248">Request</span></span>
<span data-ttu-id="d9e49-249">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d9e49-249">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1510

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="d9e49-250">响应</span><span class="sxs-lookup"><span data-stu-id="d9e49-250">Response</span></span>
<span data-ttu-id="d9e49-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9e49-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1682

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```




