---
title: 更新 windowsAppX
description: 更新 windowsAppX 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10ea9854ac8e9720f06393943e798224e91adf28
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47976597"
---
# <a name="update-windowsappx"></a><span data-ttu-id="996b3-103">更新 windowsAppX</span><span class="sxs-lookup"><span data-stu-id="996b3-103">Update windowsAppX</span></span>

<span data-ttu-id="996b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="996b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="996b3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="996b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="996b3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="996b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="996b3-107">更新 [windowsAppX](../resources/intune-apps-windowsappx.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="996b3-107">Update the properties of a [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="996b3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="996b3-108">Prerequisites</span></span>
<span data-ttu-id="996b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="996b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="996b3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="996b3-111">Permission type</span></span>|<span data-ttu-id="996b3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="996b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="996b3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="996b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="996b3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="996b3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="996b3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="996b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="996b3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="996b3-116">Not supported.</span></span>|
|<span data-ttu-id="996b3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="996b3-117">Application</span></span>|<span data-ttu-id="996b3-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="996b3-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="996b3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="996b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="996b3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="996b3-120">Request headers</span></span>
|<span data-ttu-id="996b3-121">标头</span><span class="sxs-lookup"><span data-stu-id="996b3-121">Header</span></span>|<span data-ttu-id="996b3-122">值</span><span class="sxs-lookup"><span data-stu-id="996b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="996b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="996b3-123">Authorization</span></span>|<span data-ttu-id="996b3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="996b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="996b3-125">接受</span><span class="sxs-lookup"><span data-stu-id="996b3-125">Accept</span></span>|<span data-ttu-id="996b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="996b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="996b3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="996b3-127">Request body</span></span>
<span data-ttu-id="996b3-128">在请求正文中，提供 [windowsAppX](../resources/intune-apps-windowsappx.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="996b3-128">In the request body, supply a JSON representation for the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

<span data-ttu-id="996b3-129">下表显示创建 [windowsAppX](../resources/intune-apps-windowsappx.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="996b3-129">The following table shows the properties that are required when you create the [windowsAppX](../resources/intune-apps-windowsappx.md).</span></span>

|<span data-ttu-id="996b3-130">属性</span><span class="sxs-lookup"><span data-stu-id="996b3-130">Property</span></span>|<span data-ttu-id="996b3-131">类型</span><span class="sxs-lookup"><span data-stu-id="996b3-131">Type</span></span>|<span data-ttu-id="996b3-132">说明</span><span class="sxs-lookup"><span data-stu-id="996b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="996b3-133">id</span><span class="sxs-lookup"><span data-stu-id="996b3-133">id</span></span>|<span data-ttu-id="996b3-134">String</span><span class="sxs-lookup"><span data-stu-id="996b3-134">String</span></span>|<span data-ttu-id="996b3-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="996b3-135">Key of the entity.</span></span> <span data-ttu-id="996b3-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="996b3-137">displayName</span></span>|<span data-ttu-id="996b3-138">String</span><span class="sxs-lookup"><span data-stu-id="996b3-138">String</span></span>|<span data-ttu-id="996b3-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="996b3-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="996b3-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-141">description</span><span class="sxs-lookup"><span data-stu-id="996b3-141">description</span></span>|<span data-ttu-id="996b3-142">String</span><span class="sxs-lookup"><span data-stu-id="996b3-142">String</span></span>|<span data-ttu-id="996b3-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="996b3-143">The description of the app.</span></span> <span data-ttu-id="996b3-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-145">publisher</span><span class="sxs-lookup"><span data-stu-id="996b3-145">publisher</span></span>|<span data-ttu-id="996b3-146">String</span><span class="sxs-lookup"><span data-stu-id="996b3-146">String</span></span>|<span data-ttu-id="996b3-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="996b3-147">The publisher of the app.</span></span> <span data-ttu-id="996b3-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="996b3-149">largeIcon</span></span>|[<span data-ttu-id="996b3-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="996b3-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="996b3-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="996b3-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="996b3-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="996b3-153">createdDateTime</span></span>|<span data-ttu-id="996b3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="996b3-154">DateTimeOffset</span></span>|<span data-ttu-id="996b3-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="996b3-155">The date and time the app was created.</span></span> <span data-ttu-id="996b3-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="996b3-157">lastModifiedDateTime</span></span>|<span data-ttu-id="996b3-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="996b3-158">DateTimeOffset</span></span>|<span data-ttu-id="996b3-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="996b3-159">The date and time the app was last modified.</span></span> <span data-ttu-id="996b3-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="996b3-161">isFeatured</span></span>|<span data-ttu-id="996b3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="996b3-162">Boolean</span></span>|<span data-ttu-id="996b3-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="996b3-164">privacyInformationUrl</span></span>|<span data-ttu-id="996b3-165">String</span><span class="sxs-lookup"><span data-stu-id="996b3-165">String</span></span>|<span data-ttu-id="996b3-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="996b3-166">The privacy statement Url.</span></span> <span data-ttu-id="996b3-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="996b3-168">informationUrl</span></span>|<span data-ttu-id="996b3-169">String</span><span class="sxs-lookup"><span data-stu-id="996b3-169">String</span></span>|<span data-ttu-id="996b3-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="996b3-170">The more information Url.</span></span> <span data-ttu-id="996b3-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-172">所有者</span><span class="sxs-lookup"><span data-stu-id="996b3-172">owner</span></span>|<span data-ttu-id="996b3-173">String</span><span class="sxs-lookup"><span data-stu-id="996b3-173">String</span></span>|<span data-ttu-id="996b3-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="996b3-174">The owner of the app.</span></span> <span data-ttu-id="996b3-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-176">developer</span><span class="sxs-lookup"><span data-stu-id="996b3-176">developer</span></span>|<span data-ttu-id="996b3-177">String</span><span class="sxs-lookup"><span data-stu-id="996b3-177">String</span></span>|<span data-ttu-id="996b3-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="996b3-178">The developer of the app.</span></span> <span data-ttu-id="996b3-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-180">notes</span><span class="sxs-lookup"><span data-stu-id="996b3-180">notes</span></span>|<span data-ttu-id="996b3-181">String</span><span class="sxs-lookup"><span data-stu-id="996b3-181">String</span></span>|<span data-ttu-id="996b3-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="996b3-182">Notes for the app.</span></span> <span data-ttu-id="996b3-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="996b3-184">uploadState</span></span>|<span data-ttu-id="996b3-185">Int32</span><span class="sxs-lookup"><span data-stu-id="996b3-185">Int32</span></span>|<span data-ttu-id="996b3-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="996b3-186">The upload state.</span></span> <span data-ttu-id="996b3-187">可能的值包括： 0- `Not Ready` 、1- `Ready` 、2- `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="996b3-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="996b3-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="996b3-189">publishingState</span></span>|[<span data-ttu-id="996b3-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="996b3-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="996b3-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="996b3-191">The publishing state for the app.</span></span> <span data-ttu-id="996b3-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="996b3-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="996b3-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="996b3-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="996b3-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="996b3-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="996b3-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="996b3-195">isAssigned</span></span>|<span data-ttu-id="996b3-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="996b3-196">Boolean</span></span>|<span data-ttu-id="996b3-197">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="996b3-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="996b3-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="996b3-199">roleScopeTagIds</span></span>|<span data-ttu-id="996b3-200">String collection</span><span class="sxs-lookup"><span data-stu-id="996b3-200">String collection</span></span>|<span data-ttu-id="996b3-201">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="996b3-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="996b3-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="996b3-203">dependentAppCount</span></span>|<span data-ttu-id="996b3-204">Int32</span><span class="sxs-lookup"><span data-stu-id="996b3-204">Int32</span></span>|<span data-ttu-id="996b3-205">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="996b3-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="996b3-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="996b3-207">supersedingAppCount</span></span>|<span data-ttu-id="996b3-208">Int32</span><span class="sxs-lookup"><span data-stu-id="996b3-208">Int32</span></span>|<span data-ttu-id="996b3-209">此应用程序直接或间接取代的应用程序总数量。</span><span class="sxs-lookup"><span data-stu-id="996b3-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="996b3-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="996b3-211">supersededAppCount</span></span>|<span data-ttu-id="996b3-212">Int32</span><span class="sxs-lookup"><span data-stu-id="996b3-212">Int32</span></span>|<span data-ttu-id="996b3-213">此应用程序直接或间接取代的应用程序总数量。</span><span class="sxs-lookup"><span data-stu-id="996b3-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="996b3-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="996b3-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="996b3-215">committedContentVersion</span></span>|<span data-ttu-id="996b3-216">String</span><span class="sxs-lookup"><span data-stu-id="996b3-216">String</span></span>|<span data-ttu-id="996b3-217">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="996b3-217">The internal committed content version.</span></span> <span data-ttu-id="996b3-218">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="996b3-219">fileName</span><span class="sxs-lookup"><span data-stu-id="996b3-219">fileName</span></span>|<span data-ttu-id="996b3-220">String</span><span class="sxs-lookup"><span data-stu-id="996b3-220">String</span></span>|<span data-ttu-id="996b3-221">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="996b3-221">The name of the main Lob application file.</span></span> <span data-ttu-id="996b3-222">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="996b3-223">size</span><span class="sxs-lookup"><span data-stu-id="996b3-223">size</span></span>|<span data-ttu-id="996b3-224">Int64</span><span class="sxs-lookup"><span data-stu-id="996b3-224">Int64</span></span>|<span data-ttu-id="996b3-225">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="996b3-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="996b3-226">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="996b3-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="996b3-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="996b3-227">applicableArchitectures</span></span>|[<span data-ttu-id="996b3-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="996b3-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="996b3-229">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="996b3-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="996b3-230">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="996b3-230">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="996b3-231">identityName</span><span class="sxs-lookup"><span data-stu-id="996b3-231">identityName</span></span>|<span data-ttu-id="996b3-232">String</span><span class="sxs-lookup"><span data-stu-id="996b3-232">String</span></span>|<span data-ttu-id="996b3-233">标识名称。</span><span class="sxs-lookup"><span data-stu-id="996b3-233">The Identity Name.</span></span>|
|<span data-ttu-id="996b3-234">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="996b3-234">identityPublisherHash</span></span>|<span data-ttu-id="996b3-235">String</span><span class="sxs-lookup"><span data-stu-id="996b3-235">String</span></span>|<span data-ttu-id="996b3-236">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="996b3-236">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="996b3-237">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="996b3-237">identityResourceIdentifier</span></span>|<span data-ttu-id="996b3-238">String</span><span class="sxs-lookup"><span data-stu-id="996b3-238">String</span></span>|<span data-ttu-id="996b3-239">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="996b3-239">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="996b3-240">isBundle</span><span class="sxs-lookup"><span data-stu-id="996b3-240">isBundle</span></span>|<span data-ttu-id="996b3-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="996b3-241">Boolean</span></span>|<span data-ttu-id="996b3-242">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="996b3-242">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="996b3-243">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="996b3-243">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="996b3-244">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="996b3-244">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="996b3-245">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="996b3-245">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="996b3-246">identityVersion</span><span class="sxs-lookup"><span data-stu-id="996b3-246">identityVersion</span></span>|<span data-ttu-id="996b3-247">String</span><span class="sxs-lookup"><span data-stu-id="996b3-247">String</span></span>|<span data-ttu-id="996b3-248">标识版本。</span><span class="sxs-lookup"><span data-stu-id="996b3-248">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="996b3-249">响应</span><span class="sxs-lookup"><span data-stu-id="996b3-249">Response</span></span>
<span data-ttu-id="996b3-250">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [windowsAppX](../resources/intune-apps-windowsappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="996b3-250">If successful, this method returns a `200 OK` response code and an updated [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="996b3-251">示例</span><span class="sxs-lookup"><span data-stu-id="996b3-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="996b3-252">请求</span><span class="sxs-lookup"><span data-stu-id="996b3-252">Request</span></span>
<span data-ttu-id="996b3-253">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="996b3-253">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1470

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="996b3-254">响应</span><span class="sxs-lookup"><span data-stu-id="996b3-254">Response</span></span>
<span data-ttu-id="996b3-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="996b3-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1642

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "identityVersion": "Identity Version value"
}
```






