---
title: 更新 webApp
description: 更新 webApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a65ab5ba1b08ea99841636bc4f72f8c7594511a8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435068"
---
# <a name="update-webapp"></a><span data-ttu-id="38e92-103">更新 webApp</span><span class="sxs-lookup"><span data-stu-id="38e92-103">Update webApp</span></span>

<span data-ttu-id="38e92-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38e92-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38e92-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="38e92-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38e92-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="38e92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38e92-107">更新 [webApp](../resources/intune-apps-webapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="38e92-107">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38e92-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="38e92-108">Prerequisites</span></span>
<span data-ttu-id="38e92-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38e92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38e92-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="38e92-111">Permission type</span></span>|<span data-ttu-id="38e92-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="38e92-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38e92-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38e92-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38e92-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38e92-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="38e92-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38e92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38e92-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="38e92-116">Not supported.</span></span>|
|<span data-ttu-id="38e92-117">Application</span><span class="sxs-lookup"><span data-stu-id="38e92-117">Application</span></span>|<span data-ttu-id="38e92-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38e92-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38e92-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38e92-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="38e92-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="38e92-120">Request headers</span></span>
|<span data-ttu-id="38e92-121">标头</span><span class="sxs-lookup"><span data-stu-id="38e92-121">Header</span></span>|<span data-ttu-id="38e92-122">值</span><span class="sxs-lookup"><span data-stu-id="38e92-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38e92-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="38e92-123">Authorization</span></span>|<span data-ttu-id="38e92-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="38e92-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38e92-125">接受</span><span class="sxs-lookup"><span data-stu-id="38e92-125">Accept</span></span>|<span data-ttu-id="38e92-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38e92-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38e92-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="38e92-127">Request body</span></span>
<span data-ttu-id="38e92-128">在请求正文中，提供 [webApp](../resources/intune-apps-webapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38e92-128">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="38e92-129">下表显示创建 [webApp](../resources/intune-apps-webapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="38e92-129">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="38e92-130">属性</span><span class="sxs-lookup"><span data-stu-id="38e92-130">Property</span></span>|<span data-ttu-id="38e92-131">类型</span><span class="sxs-lookup"><span data-stu-id="38e92-131">Type</span></span>|<span data-ttu-id="38e92-132">说明</span><span class="sxs-lookup"><span data-stu-id="38e92-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38e92-133">id</span><span class="sxs-lookup"><span data-stu-id="38e92-133">id</span></span>|<span data-ttu-id="38e92-134">String</span><span class="sxs-lookup"><span data-stu-id="38e92-134">String</span></span>|<span data-ttu-id="38e92-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="38e92-135">Key of the entity.</span></span> <span data-ttu-id="38e92-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-137">displayName</span><span class="sxs-lookup"><span data-stu-id="38e92-137">displayName</span></span>|<span data-ttu-id="38e92-138">String</span><span class="sxs-lookup"><span data-stu-id="38e92-138">String</span></span>|<span data-ttu-id="38e92-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="38e92-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="38e92-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-141">说明</span><span class="sxs-lookup"><span data-stu-id="38e92-141">description</span></span>|<span data-ttu-id="38e92-142">String</span><span class="sxs-lookup"><span data-stu-id="38e92-142">String</span></span>|<span data-ttu-id="38e92-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="38e92-143">The description of the app.</span></span> <span data-ttu-id="38e92-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-145">publisher</span><span class="sxs-lookup"><span data-stu-id="38e92-145">publisher</span></span>|<span data-ttu-id="38e92-146">String</span><span class="sxs-lookup"><span data-stu-id="38e92-146">String</span></span>|<span data-ttu-id="38e92-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="38e92-147">The publisher of the app.</span></span> <span data-ttu-id="38e92-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="38e92-149">largeIcon</span></span>|[<span data-ttu-id="38e92-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="38e92-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="38e92-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="38e92-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="38e92-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38e92-153">createdDateTime</span></span>|<span data-ttu-id="38e92-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38e92-154">DateTimeOffset</span></span>|<span data-ttu-id="38e92-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="38e92-155">The date and time the app was created.</span></span> <span data-ttu-id="38e92-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38e92-157">lastModifiedDateTime</span></span>|<span data-ttu-id="38e92-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38e92-158">DateTimeOffset</span></span>|<span data-ttu-id="38e92-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="38e92-159">The date and time the app was last modified.</span></span> <span data-ttu-id="38e92-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="38e92-161">isFeatured</span></span>|<span data-ttu-id="38e92-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="38e92-162">Boolean</span></span>|<span data-ttu-id="38e92-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="38e92-164">privacyInformationUrl</span></span>|<span data-ttu-id="38e92-165">String</span><span class="sxs-lookup"><span data-stu-id="38e92-165">String</span></span>|<span data-ttu-id="38e92-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="38e92-166">The privacy statement Url.</span></span> <span data-ttu-id="38e92-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="38e92-168">informationUrl</span></span>|<span data-ttu-id="38e92-169">String</span><span class="sxs-lookup"><span data-stu-id="38e92-169">String</span></span>|<span data-ttu-id="38e92-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="38e92-170">The more information Url.</span></span> <span data-ttu-id="38e92-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-172">所有者</span><span class="sxs-lookup"><span data-stu-id="38e92-172">owner</span></span>|<span data-ttu-id="38e92-173">String</span><span class="sxs-lookup"><span data-stu-id="38e92-173">String</span></span>|<span data-ttu-id="38e92-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="38e92-174">The owner of the app.</span></span> <span data-ttu-id="38e92-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-176">developer</span><span class="sxs-lookup"><span data-stu-id="38e92-176">developer</span></span>|<span data-ttu-id="38e92-177">String</span><span class="sxs-lookup"><span data-stu-id="38e92-177">String</span></span>|<span data-ttu-id="38e92-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="38e92-178">The developer of the app.</span></span> <span data-ttu-id="38e92-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-180">notes</span><span class="sxs-lookup"><span data-stu-id="38e92-180">notes</span></span>|<span data-ttu-id="38e92-181">String</span><span class="sxs-lookup"><span data-stu-id="38e92-181">String</span></span>|<span data-ttu-id="38e92-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="38e92-182">Notes for the app.</span></span> <span data-ttu-id="38e92-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="38e92-184">uploadState</span></span>|<span data-ttu-id="38e92-185">Int32</span><span class="sxs-lookup"><span data-stu-id="38e92-185">Int32</span></span>|<span data-ttu-id="38e92-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="38e92-186">The upload state.</span></span> <span data-ttu-id="38e92-187">可能的值是： 0 - `Not Ready` ， 1 - `Ready` ， 2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="38e92-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="38e92-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="38e92-189">publishingState</span></span>|[<span data-ttu-id="38e92-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="38e92-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="38e92-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="38e92-191">The publishing state for the app.</span></span> <span data-ttu-id="38e92-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="38e92-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="38e92-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="38e92-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="38e92-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="38e92-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="38e92-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="38e92-195">isAssigned</span></span>|<span data-ttu-id="38e92-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="38e92-196">Boolean</span></span>|<span data-ttu-id="38e92-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="38e92-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="38e92-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="38e92-199">roleScopeTagIds</span></span>|<span data-ttu-id="38e92-200">字符串集合</span><span class="sxs-lookup"><span data-stu-id="38e92-200">String collection</span></span>|<span data-ttu-id="38e92-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="38e92-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="38e92-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="38e92-203">dependentAppCount</span></span>|<span data-ttu-id="38e92-204">Int32</span><span class="sxs-lookup"><span data-stu-id="38e92-204">Int32</span></span>|<span data-ttu-id="38e92-205">子应用具有的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="38e92-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="38e92-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="38e92-207">supersedingAppCount</span></span>|<span data-ttu-id="38e92-208">Int32</span><span class="sxs-lookup"><span data-stu-id="38e92-208">Int32</span></span>|<span data-ttu-id="38e92-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="38e92-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="38e92-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="38e92-211">supersededAppCount</span></span>|<span data-ttu-id="38e92-212">Int32</span><span class="sxs-lookup"><span data-stu-id="38e92-212">Int32</span></span>|<span data-ttu-id="38e92-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="38e92-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="38e92-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="38e92-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="38e92-215">appUrl</span><span class="sxs-lookup"><span data-stu-id="38e92-215">appUrl</span></span>|<span data-ttu-id="38e92-216">String</span><span class="sxs-lookup"><span data-stu-id="38e92-216">String</span></span>|<span data-ttu-id="38e92-217">Web 应用 URL。</span><span class="sxs-lookup"><span data-stu-id="38e92-217">The web app URL.</span></span> <span data-ttu-id="38e92-218">此属性不能为 PATCHed。</span><span class="sxs-lookup"><span data-stu-id="38e92-218">This property cannot be PATCHed.</span></span>|
|<span data-ttu-id="38e92-219">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="38e92-219">useManagedBrowser</span></span>|<span data-ttu-id="38e92-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="38e92-220">Boolean</span></span>|<span data-ttu-id="38e92-221">是否使用托管浏览器。</span><span class="sxs-lookup"><span data-stu-id="38e92-221">Whether or not to use managed browser.</span></span> <span data-ttu-id="38e92-222">此属性仅适用于 Android 和 iOS。</span><span class="sxs-lookup"><span data-stu-id="38e92-222">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="38e92-223">响应</span><span class="sxs-lookup"><span data-stu-id="38e92-223">Response</span></span>
<span data-ttu-id="38e92-224">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [webApp](../resources/intune-apps-webapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="38e92-224">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38e92-225">示例</span><span class="sxs-lookup"><span data-stu-id="38e92-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="38e92-226">请求</span><span class="sxs-lookup"><span data-stu-id="38e92-226">Request</span></span>
<span data-ttu-id="38e92-227">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="38e92-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 836

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="38e92-228">响应</span><span class="sxs-lookup"><span data-stu-id="38e92-228">Response</span></span>
<span data-ttu-id="38e92-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="38e92-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1008

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```




