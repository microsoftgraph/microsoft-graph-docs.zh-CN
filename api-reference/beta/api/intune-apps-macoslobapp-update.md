---
title: 更新 macOSLobApp
description: 更新 macOSLobApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4ca98e294207217790c8c68288a8c3c57dfbc527
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864107"
---
# <a name="update-macoslobapp"></a><span data-ttu-id="52221-103">更新 macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="52221-103">Update macOSLobApp</span></span>

<span data-ttu-id="52221-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52221-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52221-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="52221-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52221-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="52221-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52221-107">更新 [macOSLobApp 对象](../resources/intune-apps-macoslobapp.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="52221-107">Update the properties of a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52221-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="52221-108">Prerequisites</span></span>
<span data-ttu-id="52221-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="52221-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52221-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="52221-111">Permission type</span></span>|<span data-ttu-id="52221-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="52221-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52221-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="52221-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52221-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52221-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="52221-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="52221-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52221-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="52221-116">Not supported.</span></span>|
|<span data-ttu-id="52221-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="52221-117">Application</span></span>|<span data-ttu-id="52221-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52221-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52221-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="52221-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="52221-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="52221-120">Request headers</span></span>
|<span data-ttu-id="52221-121">标头</span><span class="sxs-lookup"><span data-stu-id="52221-121">Header</span></span>|<span data-ttu-id="52221-122">值</span><span class="sxs-lookup"><span data-stu-id="52221-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52221-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="52221-123">Authorization</span></span>|<span data-ttu-id="52221-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="52221-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52221-125">接受</span><span class="sxs-lookup"><span data-stu-id="52221-125">Accept</span></span>|<span data-ttu-id="52221-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52221-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52221-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="52221-127">Request body</span></span>
<span data-ttu-id="52221-128">在请求正文中，提供 [macOSLobApp](../resources/intune-apps-macoslobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52221-128">In the request body, supply a JSON representation for the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

<span data-ttu-id="52221-129">下表显示创建 [macOSLobApp](../resources/intune-apps-macoslobapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="52221-129">The following table shows the properties that are required when you create the [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span></span>

|<span data-ttu-id="52221-130">属性</span><span class="sxs-lookup"><span data-stu-id="52221-130">Property</span></span>|<span data-ttu-id="52221-131">类型</span><span class="sxs-lookup"><span data-stu-id="52221-131">Type</span></span>|<span data-ttu-id="52221-132">说明</span><span class="sxs-lookup"><span data-stu-id="52221-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52221-133">id</span><span class="sxs-lookup"><span data-stu-id="52221-133">id</span></span>|<span data-ttu-id="52221-134">String</span><span class="sxs-lookup"><span data-stu-id="52221-134">String</span></span>|<span data-ttu-id="52221-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="52221-135">Key of the entity.</span></span> <span data-ttu-id="52221-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-137">displayName</span><span class="sxs-lookup"><span data-stu-id="52221-137">displayName</span></span>|<span data-ttu-id="52221-138">String</span><span class="sxs-lookup"><span data-stu-id="52221-138">String</span></span>|<span data-ttu-id="52221-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="52221-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="52221-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-141">说明</span><span class="sxs-lookup"><span data-stu-id="52221-141">description</span></span>|<span data-ttu-id="52221-142">String</span><span class="sxs-lookup"><span data-stu-id="52221-142">String</span></span>|<span data-ttu-id="52221-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="52221-143">The description of the app.</span></span> <span data-ttu-id="52221-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-145">publisher</span><span class="sxs-lookup"><span data-stu-id="52221-145">publisher</span></span>|<span data-ttu-id="52221-146">String</span><span class="sxs-lookup"><span data-stu-id="52221-146">String</span></span>|<span data-ttu-id="52221-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="52221-147">The publisher of the app.</span></span> <span data-ttu-id="52221-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="52221-149">largeIcon</span></span>|[<span data-ttu-id="52221-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="52221-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="52221-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="52221-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="52221-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="52221-153">createdDateTime</span></span>|<span data-ttu-id="52221-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52221-154">DateTimeOffset</span></span>|<span data-ttu-id="52221-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="52221-155">The date and time the app was created.</span></span> <span data-ttu-id="52221-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="52221-157">lastModifiedDateTime</span></span>|<span data-ttu-id="52221-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52221-158">DateTimeOffset</span></span>|<span data-ttu-id="52221-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="52221-159">The date and time the app was last modified.</span></span> <span data-ttu-id="52221-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="52221-161">isFeatured</span></span>|<span data-ttu-id="52221-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="52221-162">Boolean</span></span>|<span data-ttu-id="52221-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="52221-164">privacyInformationUrl</span></span>|<span data-ttu-id="52221-165">String</span><span class="sxs-lookup"><span data-stu-id="52221-165">String</span></span>|<span data-ttu-id="52221-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="52221-166">The privacy statement Url.</span></span> <span data-ttu-id="52221-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="52221-168">informationUrl</span></span>|<span data-ttu-id="52221-169">String</span><span class="sxs-lookup"><span data-stu-id="52221-169">String</span></span>|<span data-ttu-id="52221-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="52221-170">The more information Url.</span></span> <span data-ttu-id="52221-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-172">owner</span><span class="sxs-lookup"><span data-stu-id="52221-172">owner</span></span>|<span data-ttu-id="52221-173">String</span><span class="sxs-lookup"><span data-stu-id="52221-173">String</span></span>|<span data-ttu-id="52221-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="52221-174">The owner of the app.</span></span> <span data-ttu-id="52221-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-176">developer</span><span class="sxs-lookup"><span data-stu-id="52221-176">developer</span></span>|<span data-ttu-id="52221-177">String</span><span class="sxs-lookup"><span data-stu-id="52221-177">String</span></span>|<span data-ttu-id="52221-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="52221-178">The developer of the app.</span></span> <span data-ttu-id="52221-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-180">notes</span><span class="sxs-lookup"><span data-stu-id="52221-180">notes</span></span>|<span data-ttu-id="52221-181">String</span><span class="sxs-lookup"><span data-stu-id="52221-181">String</span></span>|<span data-ttu-id="52221-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="52221-182">Notes for the app.</span></span> <span data-ttu-id="52221-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="52221-184">uploadState</span></span>|<span data-ttu-id="52221-185">Int32</span><span class="sxs-lookup"><span data-stu-id="52221-185">Int32</span></span>|<span data-ttu-id="52221-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="52221-186">The upload state.</span></span> <span data-ttu-id="52221-187">可能的值是：0 - `Not Ready` 、1 - `Ready` 、2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="52221-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="52221-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="52221-189">publishingState</span></span>|[<span data-ttu-id="52221-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="52221-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="52221-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="52221-191">The publishing state for the app.</span></span> <span data-ttu-id="52221-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="52221-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="52221-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="52221-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="52221-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="52221-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="52221-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="52221-195">isAssigned</span></span>|<span data-ttu-id="52221-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="52221-196">Boolean</span></span>|<span data-ttu-id="52221-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="52221-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="52221-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="52221-199">roleScopeTagIds</span></span>|<span data-ttu-id="52221-200">String 集合</span><span class="sxs-lookup"><span data-stu-id="52221-200">String collection</span></span>|<span data-ttu-id="52221-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="52221-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="52221-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="52221-203">dependentAppCount</span></span>|<span data-ttu-id="52221-204">Int32</span><span class="sxs-lookup"><span data-stu-id="52221-204">Int32</span></span>|<span data-ttu-id="52221-205">子应用具有的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="52221-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="52221-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="52221-207">supersedingAppCount</span></span>|<span data-ttu-id="52221-208">Int32</span><span class="sxs-lookup"><span data-stu-id="52221-208">Int32</span></span>|<span data-ttu-id="52221-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="52221-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="52221-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="52221-211">supersededAppCount</span></span>|<span data-ttu-id="52221-212">Int32</span><span class="sxs-lookup"><span data-stu-id="52221-212">Int32</span></span>|<span data-ttu-id="52221-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="52221-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="52221-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52221-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="52221-215">committedContentVersion</span></span>|<span data-ttu-id="52221-216">String</span><span class="sxs-lookup"><span data-stu-id="52221-216">String</span></span>|<span data-ttu-id="52221-217">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="52221-217">The internal committed content version.</span></span> <span data-ttu-id="52221-218">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="52221-219">fileName</span><span class="sxs-lookup"><span data-stu-id="52221-219">fileName</span></span>|<span data-ttu-id="52221-220">String</span><span class="sxs-lookup"><span data-stu-id="52221-220">String</span></span>|<span data-ttu-id="52221-221">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="52221-221">The name of the main Lob application file.</span></span> <span data-ttu-id="52221-222">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="52221-223">size</span><span class="sxs-lookup"><span data-stu-id="52221-223">size</span></span>|<span data-ttu-id="52221-224">Int64</span><span class="sxs-lookup"><span data-stu-id="52221-224">Int64</span></span>|<span data-ttu-id="52221-225">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="52221-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="52221-226">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="52221-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="52221-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="52221-227">bundleId</span></span>|<span data-ttu-id="52221-228">String</span><span class="sxs-lookup"><span data-stu-id="52221-228">String</span></span>|<span data-ttu-id="52221-229">捆绑包 ID。</span><span class="sxs-lookup"><span data-stu-id="52221-229">The bundle id.</span></span>|
|<span data-ttu-id="52221-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="52221-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="52221-231">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="52221-231">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="52221-232">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="52221-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="52221-233">buildNumber</span><span class="sxs-lookup"><span data-stu-id="52221-233">buildNumber</span></span>|<span data-ttu-id="52221-234">String</span><span class="sxs-lookup"><span data-stu-id="52221-234">String</span></span>|<span data-ttu-id="52221-235">MacOS 业务线 (LoB) 号。</span><span class="sxs-lookup"><span data-stu-id="52221-235">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="52221-236">versionNumber</span><span class="sxs-lookup"><span data-stu-id="52221-236">versionNumber</span></span>|<span data-ttu-id="52221-237">String</span><span class="sxs-lookup"><span data-stu-id="52221-237">String</span></span>|<span data-ttu-id="52221-238">MacOS 业务线 (LoB) 版本号。</span><span class="sxs-lookup"><span data-stu-id="52221-238">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="52221-239">childApps</span><span class="sxs-lookup"><span data-stu-id="52221-239">childApps</span></span>|<span data-ttu-id="52221-240">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="52221-240">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="52221-241">此捆绑包中的应用列表</span><span class="sxs-lookup"><span data-stu-id="52221-241">The app list in this bundle package</span></span>|
|<span data-ttu-id="52221-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="52221-242">identityVersion</span></span>|<span data-ttu-id="52221-243">String</span><span class="sxs-lookup"><span data-stu-id="52221-243">String</span></span>|<span data-ttu-id="52221-244">标识版本。</span><span class="sxs-lookup"><span data-stu-id="52221-244">The identity version.</span></span>|
|<span data-ttu-id="52221-245">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="52221-245">md5HashChunkSize</span></span>|<span data-ttu-id="52221-246">Int32</span><span class="sxs-lookup"><span data-stu-id="52221-246">Int32</span></span>|<span data-ttu-id="52221-247">MD5 哈希的区块大小</span><span class="sxs-lookup"><span data-stu-id="52221-247">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="52221-248">md5Hash</span><span class="sxs-lookup"><span data-stu-id="52221-248">md5Hash</span></span>|<span data-ttu-id="52221-249">String 集合</span><span class="sxs-lookup"><span data-stu-id="52221-249">String collection</span></span>|<span data-ttu-id="52221-250">MD5 哈希代码</span><span class="sxs-lookup"><span data-stu-id="52221-250">The MD5 hash codes</span></span>|
|<span data-ttu-id="52221-251">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="52221-251">ignoreVersionDetection</span></span>|<span data-ttu-id="52221-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="52221-252">Boolean</span></span>|<span data-ttu-id="52221-253">控制应用的版本是否将用于检测安装在设备上的应用的布尔值。</span><span class="sxs-lookup"><span data-stu-id="52221-253">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="52221-254">对于使用自我更新功能 (macOS (LoB) 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="52221-254">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="52221-255">installAsManaged</span><span class="sxs-lookup"><span data-stu-id="52221-255">installAsManaged</span></span>|<span data-ttu-id="52221-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="52221-256">Boolean</span></span>|<span data-ttu-id="52221-257">用于控制应用是否将安装为托管应用的布尔值 (macOS 11.0 和其他 PKG) 。</span><span class="sxs-lookup"><span data-stu-id="52221-257">A boolean to control whether the app will be installed as managed (requires macOS 11.0 and other PKG restrictions).</span></span>|



## <a name="response"></a><span data-ttu-id="52221-258">响应</span><span class="sxs-lookup"><span data-stu-id="52221-258">Response</span></span>
<span data-ttu-id="52221-259">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [macOSLobApp](../resources/intune-apps-macoslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="52221-259">If successful, this method returns a `200 OK` response code and an updated [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52221-260">示例</span><span class="sxs-lookup"><span data-stu-id="52221-260">Example</span></span>

### <a name="request"></a><span data-ttu-id="52221-261">请求</span><span class="sxs-lookup"><span data-stu-id="52221-261">Request</span></span>
<span data-ttu-id="52221-262">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="52221-262">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1722

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
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
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true,
    "v10_14": true,
    "v10_15": true,
    "v11_0": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true,
  "installAsManaged": true
}
```

### <a name="response"></a><span data-ttu-id="52221-263">响应</span><span class="sxs-lookup"><span data-stu-id="52221-263">Response</span></span>
<span data-ttu-id="52221-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="52221-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1894

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
  "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true,
    "v10_14": true,
    "v10_15": true,
    "v11_0": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true,
  "installAsManaged": true
}
```




