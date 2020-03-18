---
title: 更新 androidLobApp
description: 更新 androidLobApp 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 68f96ed11b196a26a8fcec2e162fbc1eda60c013
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762299"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="e32ec-103">更新 androidLobApp</span><span class="sxs-lookup"><span data-stu-id="e32ec-103">Update androidLobApp</span></span>

> <span data-ttu-id="e32ec-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e32ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e32ec-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e32ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e32ec-106">更新 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e32ec-106">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e32ec-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e32ec-107">Prerequisites</span></span>
<span data-ttu-id="e32ec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e32ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e32ec-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e32ec-110">Permission type</span></span>|<span data-ttu-id="e32ec-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e32ec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e32ec-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e32ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e32ec-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e32ec-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e32ec-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e32ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e32ec-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e32ec-115">Not supported.</span></span>|
|<span data-ttu-id="e32ec-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e32ec-116">Application</span></span>|<span data-ttu-id="e32ec-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e32ec-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e32ec-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e32ec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e32ec-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e32ec-119">Request headers</span></span>
|<span data-ttu-id="e32ec-120">标头</span><span class="sxs-lookup"><span data-stu-id="e32ec-120">Header</span></span>|<span data-ttu-id="e32ec-121">值</span><span class="sxs-lookup"><span data-stu-id="e32ec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e32ec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e32ec-122">Authorization</span></span>|<span data-ttu-id="e32ec-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e32ec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e32ec-124">接受</span><span class="sxs-lookup"><span data-stu-id="e32ec-124">Accept</span></span>|<span data-ttu-id="e32ec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e32ec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e32ec-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e32ec-126">Request body</span></span>
<span data-ttu-id="e32ec-127">在请求正文中，提供 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e32ec-127">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="e32ec-128">下表显示了创建 [androidLobApp](../resources/intune-apps-androidlobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e32ec-128">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="e32ec-129">属性</span><span class="sxs-lookup"><span data-stu-id="e32ec-129">Property</span></span>|<span data-ttu-id="e32ec-130">类型</span><span class="sxs-lookup"><span data-stu-id="e32ec-130">Type</span></span>|<span data-ttu-id="e32ec-131">说明</span><span class="sxs-lookup"><span data-stu-id="e32ec-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e32ec-132">id</span><span class="sxs-lookup"><span data-stu-id="e32ec-132">id</span></span>|<span data-ttu-id="e32ec-133">字符串</span><span class="sxs-lookup"><span data-stu-id="e32ec-133">String</span></span>|<span data-ttu-id="e32ec-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e32ec-134">Key of the entity.</span></span> <span data-ttu-id="e32ec-135">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e32ec-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e32ec-136">displayName</span></span>|<span data-ttu-id="e32ec-137">String</span><span class="sxs-lookup"><span data-stu-id="e32ec-137">String</span></span>|<span data-ttu-id="e32ec-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="e32ec-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e32ec-139">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e32ec-140">说明</span><span class="sxs-lookup"><span data-stu-id="e32ec-140">description</span></span>|<span data-ttu-id="e32ec-141">字符串</span><span class="sxs-lookup"><span data-stu-id="e32ec-141">String</span></span>|<span data-ttu-id="e32ec-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="e32ec-142">The description of the app.</span></span> <span data-ttu-id="e32ec-143">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e32ec-144">publisher</span><span class="sxs-lookup"><span data-stu-id="e32ec-144">publisher</span></span>|<span data-ttu-id="e32ec-145">String</span><span class="sxs-lookup"><span data-stu-id="e32ec-145">String</span></span>|<span data-ttu-id="e32ec-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="e32ec-146">The publisher of the app.</span></span> <span data-ttu-id="e32ec-147">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e32ec-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e32ec-148">largeIcon</span></span>|[<span data-ttu-id="e32ec-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e32ec-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e32ec-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="e32ec-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e32ec-151">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e32ec-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e32ec-152">createdDateTime</span></span>|<span data-ttu-id="e32ec-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e32ec-153">DateTimeOffset</span></span>|<span data-ttu-id="e32ec-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e32ec-154">The date and time the app was created.</span></span> <span data-ttu-id="e32ec-155">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e32ec-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e32ec-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e32ec-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e32ec-157">DateTimeOffset</span></span>|<span data-ttu-id="e32ec-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e32ec-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e32ec-159">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e32ec-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e32ec-160">isFeatured</span></span>|<span data-ttu-id="e32ec-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e32ec-161">Boolean</span></span>|<span data-ttu-id="e32ec-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e32ec-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e32ec-163">privacyInformationUrl</span></span>|<span data-ttu-id="e32ec-164">String</span><span class="sxs-lookup"><span data-stu-id="e32ec-164">String</span></span>|<span data-ttu-id="e32ec-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="e32ec-165">The privacy statement Url.</span></span> <span data-ttu-id="e32ec-166">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e32ec-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e32ec-167">informationUrl</span></span>|<span data-ttu-id="e32ec-168">String</span><span class="sxs-lookup"><span data-stu-id="e32ec-168">String</span></span>|<span data-ttu-id="e32ec-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="e32ec-169">The more information Url.</span></span> <span data-ttu-id="e32ec-170">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e32ec-171">owner</span><span class="sxs-lookup"><span data-stu-id="e32ec-171">owner</span></span>|<span data-ttu-id="e32ec-172">String</span><span class="sxs-lookup"><span data-stu-id="e32ec-172">String</span></span>|<span data-ttu-id="e32ec-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="e32ec-173">The owner of the app.</span></span> <span data-ttu-id="e32ec-174">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e32ec-175">developer</span><span class="sxs-lookup"><span data-stu-id="e32ec-175">developer</span></span>|<span data-ttu-id="e32ec-176">String</span><span class="sxs-lookup"><span data-stu-id="e32ec-176">String</span></span>|<span data-ttu-id="e32ec-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="e32ec-177">The developer of the app.</span></span> <span data-ttu-id="e32ec-178">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e32ec-179">notes</span><span class="sxs-lookup"><span data-stu-id="e32ec-179">notes</span></span>|<span data-ttu-id="e32ec-180">String</span><span class="sxs-lookup"><span data-stu-id="e32ec-180">String</span></span>|<span data-ttu-id="e32ec-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="e32ec-181">Notes for the app.</span></span> <span data-ttu-id="e32ec-182">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e32ec-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="e32ec-183">uploadState</span></span>|<span data-ttu-id="e32ec-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e32ec-184">Int32</span></span>|<span data-ttu-id="e32ec-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="e32ec-185">The upload state.</span></span> <span data-ttu-id="e32ec-186">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e32ec-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="e32ec-187">publishingState</span></span>|[<span data-ttu-id="e32ec-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e32ec-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e32ec-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="e32ec-189">The publishing state for the app.</span></span> <span data-ttu-id="e32ec-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="e32ec-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e32ec-191">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="e32ec-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="e32ec-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="e32ec-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e32ec-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e32ec-193">isAssigned</span></span>|<span data-ttu-id="e32ec-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e32ec-194">Boolean</span></span>|<span data-ttu-id="e32ec-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="e32ec-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e32ec-196">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e32ec-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e32ec-197">roleScopeTagIds</span></span>|<span data-ttu-id="e32ec-198">String collection</span><span class="sxs-lookup"><span data-stu-id="e32ec-198">String collection</span></span>|<span data-ttu-id="e32ec-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="e32ec-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e32ec-200">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e32ec-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e32ec-201">dependentAppCount</span></span>|<span data-ttu-id="e32ec-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e32ec-202">Int32</span></span>|<span data-ttu-id="e32ec-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="e32ec-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e32ec-204">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e32ec-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e32ec-205">committedContentVersion</span></span>|<span data-ttu-id="e32ec-206">String</span><span class="sxs-lookup"><span data-stu-id="e32ec-206">String</span></span>|<span data-ttu-id="e32ec-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="e32ec-207">The internal committed content version.</span></span> <span data-ttu-id="e32ec-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e32ec-209">fileName</span><span class="sxs-lookup"><span data-stu-id="e32ec-209">fileName</span></span>|<span data-ttu-id="e32ec-210">String</span><span class="sxs-lookup"><span data-stu-id="e32ec-210">String</span></span>|<span data-ttu-id="e32ec-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="e32ec-211">The name of the main Lob application file.</span></span> <span data-ttu-id="e32ec-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e32ec-213">size</span><span class="sxs-lookup"><span data-stu-id="e32ec-213">size</span></span>|<span data-ttu-id="e32ec-214">Int64</span><span class="sxs-lookup"><span data-stu-id="e32ec-214">Int64</span></span>|<span data-ttu-id="e32ec-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="e32ec-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="e32ec-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e32ec-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e32ec-217">packageId</span><span class="sxs-lookup"><span data-stu-id="e32ec-217">packageId</span></span>|<span data-ttu-id="e32ec-218">String</span><span class="sxs-lookup"><span data-stu-id="e32ec-218">String</span></span>|<span data-ttu-id="e32ec-219">包标识符。</span><span class="sxs-lookup"><span data-stu-id="e32ec-219">The package identifier.</span></span>|
|<span data-ttu-id="e32ec-220">identityName</span><span class="sxs-lookup"><span data-stu-id="e32ec-220">identityName</span></span>|<span data-ttu-id="e32ec-221">String</span><span class="sxs-lookup"><span data-stu-id="e32ec-221">String</span></span>|<span data-ttu-id="e32ec-222">标识名称。</span><span class="sxs-lookup"><span data-stu-id="e32ec-222">The Identity Name.</span></span>|
|<span data-ttu-id="e32ec-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e32ec-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e32ec-224">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e32ec-224">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="e32ec-225">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="e32ec-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e32ec-226">versionName</span><span class="sxs-lookup"><span data-stu-id="e32ec-226">versionName</span></span>|<span data-ttu-id="e32ec-227">String</span><span class="sxs-lookup"><span data-stu-id="e32ec-227">String</span></span>|<span data-ttu-id="e32ec-228">Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="e32ec-228">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e32ec-229">versionCode</span><span class="sxs-lookup"><span data-stu-id="e32ec-229">versionCode</span></span>|<span data-ttu-id="e32ec-230">String</span><span class="sxs-lookup"><span data-stu-id="e32ec-230">String</span></span>|<span data-ttu-id="e32ec-231">Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="e32ec-231">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e32ec-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e32ec-232">identityVersion</span></span>|<span data-ttu-id="e32ec-233">String</span><span class="sxs-lookup"><span data-stu-id="e32ec-233">String</span></span>|<span data-ttu-id="e32ec-234">标识版本。</span><span class="sxs-lookup"><span data-stu-id="e32ec-234">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="e32ec-235">响应</span><span class="sxs-lookup"><span data-stu-id="e32ec-235">Response</span></span>
<span data-ttu-id="e32ec-236">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidLobApp](../resources/intune-apps-androidlobapp.md)  对象。</span><span class="sxs-lookup"><span data-stu-id="e32ec-236">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e32ec-237">示例</span><span class="sxs-lookup"><span data-stu-id="e32ec-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="e32ec-238">请求</span><span class="sxs-lookup"><span data-stu-id="e32ec-238">Request</span></span>
<span data-ttu-id="e32ec-239">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e32ec-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1413

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
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="e32ec-240">响应</span><span class="sxs-lookup"><span data-stu-id="e32ec-240">Response</span></span>
<span data-ttu-id="e32ec-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e32ec-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1585

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
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```




