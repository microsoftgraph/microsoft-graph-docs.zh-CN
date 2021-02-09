---
title: 更新 win32LobApp
description: 更新 win32LobApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 242341eca66747ed401f177880677bbc5cb017af
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157139"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="b2aa2-103">更新 win32LobApp</span><span class="sxs-lookup"><span data-stu-id="b2aa2-103">Update win32LobApp</span></span>

<span data-ttu-id="b2aa2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2aa2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2aa2-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2aa2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2aa2-107">更新 [win32LobApp 对象](../resources/intune-apps-win32lobapp.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-107">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2aa2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b2aa2-108">Prerequisites</span></span>
<span data-ttu-id="b2aa2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2aa2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2aa2-111">Permission type</span></span>|<span data-ttu-id="b2aa2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b2aa2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2aa2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2aa2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2aa2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2aa2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b2aa2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2aa2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2aa2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-116">Not supported.</span></span>|
|<span data-ttu-id="b2aa2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2aa2-117">Application</span></span>|<span data-ttu-id="b2aa2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2aa2-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2aa2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2aa2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="b2aa2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2aa2-120">Request headers</span></span>
|<span data-ttu-id="b2aa2-121">标头</span><span class="sxs-lookup"><span data-stu-id="b2aa2-121">Header</span></span>|<span data-ttu-id="b2aa2-122">值</span><span class="sxs-lookup"><span data-stu-id="b2aa2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2aa2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2aa2-123">Authorization</span></span>|<span data-ttu-id="b2aa2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2aa2-125">接受</span><span class="sxs-lookup"><span data-stu-id="b2aa2-125">Accept</span></span>|<span data-ttu-id="b2aa2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2aa2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2aa2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2aa2-127">Request body</span></span>
<span data-ttu-id="b2aa2-128">在请求正文中，提供 [win32LobApp](../resources/intune-apps-win32lobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-128">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="b2aa2-129">下表显示创建 [win32LobApp](../resources/intune-apps-win32lobapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-129">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="b2aa2-130">属性</span><span class="sxs-lookup"><span data-stu-id="b2aa2-130">Property</span></span>|<span data-ttu-id="b2aa2-131">类型</span><span class="sxs-lookup"><span data-stu-id="b2aa2-131">Type</span></span>|<span data-ttu-id="b2aa2-132">说明</span><span class="sxs-lookup"><span data-stu-id="b2aa2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2aa2-133">id</span><span class="sxs-lookup"><span data-stu-id="b2aa2-133">id</span></span>|<span data-ttu-id="b2aa2-134">String</span><span class="sxs-lookup"><span data-stu-id="b2aa2-134">String</span></span>|<span data-ttu-id="b2aa2-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-135">Key of the entity.</span></span> <span data-ttu-id="b2aa2-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b2aa2-137">displayName</span></span>|<span data-ttu-id="b2aa2-138">String</span><span class="sxs-lookup"><span data-stu-id="b2aa2-138">String</span></span>|<span data-ttu-id="b2aa2-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b2aa2-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-141">说明</span><span class="sxs-lookup"><span data-stu-id="b2aa2-141">description</span></span>|<span data-ttu-id="b2aa2-142">String</span><span class="sxs-lookup"><span data-stu-id="b2aa2-142">String</span></span>|<span data-ttu-id="b2aa2-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-143">The description of the app.</span></span> <span data-ttu-id="b2aa2-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-145">publisher</span><span class="sxs-lookup"><span data-stu-id="b2aa2-145">publisher</span></span>|<span data-ttu-id="b2aa2-146">String</span><span class="sxs-lookup"><span data-stu-id="b2aa2-146">String</span></span>|<span data-ttu-id="b2aa2-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-147">The publisher of the app.</span></span> <span data-ttu-id="b2aa2-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b2aa2-149">largeIcon</span></span>|[<span data-ttu-id="b2aa2-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b2aa2-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b2aa2-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b2aa2-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2aa2-153">createdDateTime</span></span>|<span data-ttu-id="b2aa2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2aa2-154">DateTimeOffset</span></span>|<span data-ttu-id="b2aa2-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-155">The date and time the app was created.</span></span> <span data-ttu-id="b2aa2-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2aa2-157">lastModifiedDateTime</span></span>|<span data-ttu-id="b2aa2-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2aa2-158">DateTimeOffset</span></span>|<span data-ttu-id="b2aa2-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-159">The date and time the app was last modified.</span></span> <span data-ttu-id="b2aa2-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b2aa2-161">isFeatured</span></span>|<span data-ttu-id="b2aa2-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2aa2-162">Boolean</span></span>|<span data-ttu-id="b2aa2-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b2aa2-164">privacyInformationUrl</span></span>|<span data-ttu-id="b2aa2-165">String</span><span class="sxs-lookup"><span data-stu-id="b2aa2-165">String</span></span>|<span data-ttu-id="b2aa2-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-166">The privacy statement Url.</span></span> <span data-ttu-id="b2aa2-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b2aa2-168">informationUrl</span></span>|<span data-ttu-id="b2aa2-169">String</span><span class="sxs-lookup"><span data-stu-id="b2aa2-169">String</span></span>|<span data-ttu-id="b2aa2-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-170">The more information Url.</span></span> <span data-ttu-id="b2aa2-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-172">owner</span><span class="sxs-lookup"><span data-stu-id="b2aa2-172">owner</span></span>|<span data-ttu-id="b2aa2-173">String</span><span class="sxs-lookup"><span data-stu-id="b2aa2-173">String</span></span>|<span data-ttu-id="b2aa2-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-174">The owner of the app.</span></span> <span data-ttu-id="b2aa2-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-176">developer</span><span class="sxs-lookup"><span data-stu-id="b2aa2-176">developer</span></span>|<span data-ttu-id="b2aa2-177">String</span><span class="sxs-lookup"><span data-stu-id="b2aa2-177">String</span></span>|<span data-ttu-id="b2aa2-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-178">The developer of the app.</span></span> <span data-ttu-id="b2aa2-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-180">notes</span><span class="sxs-lookup"><span data-stu-id="b2aa2-180">notes</span></span>|<span data-ttu-id="b2aa2-181">String</span><span class="sxs-lookup"><span data-stu-id="b2aa2-181">String</span></span>|<span data-ttu-id="b2aa2-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-182">Notes for the app.</span></span> <span data-ttu-id="b2aa2-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="b2aa2-184">uploadState</span></span>|<span data-ttu-id="b2aa2-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b2aa2-185">Int32</span></span>|<span data-ttu-id="b2aa2-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-186">The upload state.</span></span> <span data-ttu-id="b2aa2-187">可能的值是：0 - `Not Ready` 、 1 - `Ready` 、 2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="b2aa2-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="b2aa2-189">publishingState</span></span>|[<span data-ttu-id="b2aa2-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b2aa2-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b2aa2-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-191">The publishing state for the app.</span></span> <span data-ttu-id="b2aa2-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b2aa2-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="b2aa2-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b2aa2-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b2aa2-195">isAssigned</span></span>|<span data-ttu-id="b2aa2-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2aa2-196">Boolean</span></span>|<span data-ttu-id="b2aa2-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b2aa2-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b2aa2-199">roleScopeTagIds</span></span>|<span data-ttu-id="b2aa2-200">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b2aa2-200">String collection</span></span>|<span data-ttu-id="b2aa2-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b2aa2-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="b2aa2-203">dependentAppCount</span></span>|<span data-ttu-id="b2aa2-204">Int32</span><span class="sxs-lookup"><span data-stu-id="b2aa2-204">Int32</span></span>|<span data-ttu-id="b2aa2-205">子应用具有的依赖关系总数。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b2aa2-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="b2aa2-207">supersedingAppCount</span></span>|<span data-ttu-id="b2aa2-208">Int32</span><span class="sxs-lookup"><span data-stu-id="b2aa2-208">Int32</span></span>|<span data-ttu-id="b2aa2-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="b2aa2-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="b2aa2-211">supersededAppCount</span></span>|<span data-ttu-id="b2aa2-212">Int32</span><span class="sxs-lookup"><span data-stu-id="b2aa2-212">Int32</span></span>|<span data-ttu-id="b2aa2-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="b2aa2-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b2aa2-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b2aa2-215">committedContentVersion</span></span>|<span data-ttu-id="b2aa2-216">String</span><span class="sxs-lookup"><span data-stu-id="b2aa2-216">String</span></span>|<span data-ttu-id="b2aa2-217">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-217">The internal committed content version.</span></span> <span data-ttu-id="b2aa2-218">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b2aa2-219">fileName</span><span class="sxs-lookup"><span data-stu-id="b2aa2-219">fileName</span></span>|<span data-ttu-id="b2aa2-220">String</span><span class="sxs-lookup"><span data-stu-id="b2aa2-220">String</span></span>|<span data-ttu-id="b2aa2-221">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-221">The name of the main Lob application file.</span></span> <span data-ttu-id="b2aa2-222">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b2aa2-223">size</span><span class="sxs-lookup"><span data-stu-id="b2aa2-223">size</span></span>|<span data-ttu-id="b2aa2-224">Int64</span><span class="sxs-lookup"><span data-stu-id="b2aa2-224">Int64</span></span>|<span data-ttu-id="b2aa2-225">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="b2aa2-226">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2aa2-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b2aa2-227">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="b2aa2-227">installCommandLine</span></span>|<span data-ttu-id="b2aa2-228">String</span><span class="sxs-lookup"><span data-stu-id="b2aa2-228">String</span></span>|<span data-ttu-id="b2aa2-229">安装此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="b2aa2-229">The command line to install this app</span></span>|
|<span data-ttu-id="b2aa2-230">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="b2aa2-230">uninstallCommandLine</span></span>|<span data-ttu-id="b2aa2-231">String</span><span class="sxs-lookup"><span data-stu-id="b2aa2-231">String</span></span>|<span data-ttu-id="b2aa2-232">卸载此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="b2aa2-232">The command line to uninstall this app</span></span>|
|<span data-ttu-id="b2aa2-233">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="b2aa2-233">applicableArchitectures</span></span>|[<span data-ttu-id="b2aa2-234">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="b2aa2-234">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="b2aa2-235">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-235">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="b2aa2-236">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-236">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="b2aa2-237">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b2aa2-237">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b2aa2-238">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b2aa2-238">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="b2aa2-239">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-239">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="b2aa2-240">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="b2aa2-240">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="b2aa2-241">Int32</span><span class="sxs-lookup"><span data-stu-id="b2aa2-241">Int32</span></span>|<span data-ttu-id="b2aa2-242">安装此应用所需的最小可用磁盘空间的值。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-242">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="b2aa2-243">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="b2aa2-243">minimumMemoryInMB</span></span>|<span data-ttu-id="b2aa2-244">Int32</span><span class="sxs-lookup"><span data-stu-id="b2aa2-244">Int32</span></span>|<span data-ttu-id="b2aa2-245">安装此应用所需的最小物理内存的值。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-245">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="b2aa2-246">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="b2aa2-246">minimumNumberOfProcessors</span></span>|<span data-ttu-id="b2aa2-247">Int32</span><span class="sxs-lookup"><span data-stu-id="b2aa2-247">Int32</span></span>|<span data-ttu-id="b2aa2-248">安装此应用所需的最少处理器数的值。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-248">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="b2aa2-249">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="b2aa2-249">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="b2aa2-250">Int32</span><span class="sxs-lookup"><span data-stu-id="b2aa2-250">Int32</span></span>|<span data-ttu-id="b2aa2-251">安装此应用所需的最小 CPU 速度的值。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-251">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="b2aa2-252">detectionRules</span><span class="sxs-lookup"><span data-stu-id="b2aa2-252">detectionRules</span></span>|<span data-ttu-id="b2aa2-253">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b2aa2-253">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="b2aa2-254">检测 Win32 业务线和 LoB (的检测) 规则。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-254">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b2aa2-255">requirementRules</span><span class="sxs-lookup"><span data-stu-id="b2aa2-255">requirementRules</span></span>|<span data-ttu-id="b2aa2-256">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b2aa2-256">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="b2aa2-257">在 LoB 应用中检测 Win32 业务线 () 规则。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-257">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b2aa2-258">规则</span><span class="sxs-lookup"><span data-stu-id="b2aa2-258">rules</span></span>|<span data-ttu-id="b2aa2-259">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b2aa2-259">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="b2aa2-260">此应用程序的检测和要求规则。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-260">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="b2aa2-261">installExperience</span><span class="sxs-lookup"><span data-stu-id="b2aa2-261">installExperience</span></span>|[<span data-ttu-id="b2aa2-262">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="b2aa2-262">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="b2aa2-263">此应用程序的安装体验。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-263">The install experience for this app.</span></span>|
|<span data-ttu-id="b2aa2-264">returnCodes</span><span class="sxs-lookup"><span data-stu-id="b2aa2-264">returnCodes</span></span>|<span data-ttu-id="b2aa2-265">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b2aa2-265">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="b2aa2-266">安装后行为的返回代码。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-266">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="b2aa2-267">msiInformation</span><span class="sxs-lookup"><span data-stu-id="b2aa2-267">msiInformation</span></span>|[<span data-ttu-id="b2aa2-268">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="b2aa2-268">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="b2aa2-269">如果此 Win32 应用是 MSI 应用，则 MSI 详细信息。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-269">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="b2aa2-270">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="b2aa2-270">setupFilePath</span></span>|<span data-ttu-id="b2aa2-271">String</span><span class="sxs-lookup"><span data-stu-id="b2aa2-271">String</span></span>|<span data-ttu-id="b2aa2-272">加密 Win32LobApp 程序包中安装文件的相对路径。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-272">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="b2aa2-273">minimumSupportedWindowsRelease</span><span class="sxs-lookup"><span data-stu-id="b2aa2-273">minimumSupportedWindowsRelease</span></span>|<span data-ttu-id="b2aa2-274">String</span><span class="sxs-lookup"><span data-stu-id="b2aa2-274">String</span></span>|<span data-ttu-id="b2aa2-275">受支持的最低窗口版本的值。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-275">The value for the minimum supported windows release.</span></span>|
|<span data-ttu-id="b2aa2-276">displayVersion</span><span class="sxs-lookup"><span data-stu-id="b2aa2-276">displayVersion</span></span>|<span data-ttu-id="b2aa2-277">String</span><span class="sxs-lookup"><span data-stu-id="b2aa2-277">String</span></span>|<span data-ttu-id="b2aa2-278">此应用的 UX 中显示的版本。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-278">The version displayed in the UX for this app.</span></span>|



## <a name="response"></a><span data-ttu-id="b2aa2-279">响应</span><span class="sxs-lookup"><span data-stu-id="b2aa2-279">Response</span></span>
<span data-ttu-id="b2aa2-280">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [win32LobApp](../resources/intune-apps-win32lobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-280">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2aa2-281">示例</span><span class="sxs-lookup"><span data-stu-id="b2aa2-281">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2aa2-282">请求</span><span class="sxs-lookup"><span data-stu-id="b2aa2-282">Request</span></span>
<span data-ttu-id="b2aa2-283">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-283">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 3405

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value",
  "displayVersion": "Display Version value"
}
```

### <a name="response"></a><span data-ttu-id="b2aa2-284">响应</span><span class="sxs-lookup"><span data-stu-id="b2aa2-284">Response</span></span>
<span data-ttu-id="b2aa2-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b2aa2-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3577

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value",
  "displayVersion": "Display Version value"
}
```




