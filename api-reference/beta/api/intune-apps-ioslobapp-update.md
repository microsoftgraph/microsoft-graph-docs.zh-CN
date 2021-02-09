---
title: 更新 iosLobApp
description: 更新 iosLobApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ce883fd64d0abe18ed36fccd58f341c364eaac5e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157377"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="9bf5e-103">更新 iosLobApp</span><span class="sxs-lookup"><span data-stu-id="9bf5e-103">Update iosLobApp</span></span>

<span data-ttu-id="9bf5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bf5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bf5e-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bf5e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bf5e-107">更新 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-107">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bf5e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9bf5e-108">Prerequisites</span></span>
<span data-ttu-id="9bf5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bf5e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9bf5e-111">Permission type</span></span>|<span data-ttu-id="9bf5e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9bf5e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bf5e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9bf5e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9bf5e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bf5e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9bf5e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9bf5e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bf5e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-116">Not supported.</span></span>|
|<span data-ttu-id="9bf5e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9bf5e-117">Application</span></span>|<span data-ttu-id="9bf5e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bf5e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bf5e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9bf5e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="9bf5e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9bf5e-120">Request headers</span></span>
|<span data-ttu-id="9bf5e-121">标头</span><span class="sxs-lookup"><span data-stu-id="9bf5e-121">Header</span></span>|<span data-ttu-id="9bf5e-122">值</span><span class="sxs-lookup"><span data-stu-id="9bf5e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bf5e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bf5e-123">Authorization</span></span>|<span data-ttu-id="9bf5e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bf5e-125">接受</span><span class="sxs-lookup"><span data-stu-id="9bf5e-125">Accept</span></span>|<span data-ttu-id="9bf5e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9bf5e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bf5e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9bf5e-127">Request body</span></span>
<span data-ttu-id="9bf5e-128">在请求正文中，提供 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-128">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="9bf5e-129">下表显示了创建 [iosLobApp](../resources/intune-apps-ioslobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-129">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="9bf5e-130">属性</span><span class="sxs-lookup"><span data-stu-id="9bf5e-130">Property</span></span>|<span data-ttu-id="9bf5e-131">类型</span><span class="sxs-lookup"><span data-stu-id="9bf5e-131">Type</span></span>|<span data-ttu-id="9bf5e-132">说明</span><span class="sxs-lookup"><span data-stu-id="9bf5e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bf5e-133">id</span><span class="sxs-lookup"><span data-stu-id="9bf5e-133">id</span></span>|<span data-ttu-id="9bf5e-134">String</span><span class="sxs-lookup"><span data-stu-id="9bf5e-134">String</span></span>|<span data-ttu-id="9bf5e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-135">Key of the entity.</span></span> <span data-ttu-id="9bf5e-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9bf5e-137">displayName</span></span>|<span data-ttu-id="9bf5e-138">String</span><span class="sxs-lookup"><span data-stu-id="9bf5e-138">String</span></span>|<span data-ttu-id="9bf5e-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9bf5e-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-141">说明</span><span class="sxs-lookup"><span data-stu-id="9bf5e-141">description</span></span>|<span data-ttu-id="9bf5e-142">String</span><span class="sxs-lookup"><span data-stu-id="9bf5e-142">String</span></span>|<span data-ttu-id="9bf5e-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-143">The description of the app.</span></span> <span data-ttu-id="9bf5e-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="9bf5e-145">publisher</span></span>|<span data-ttu-id="9bf5e-146">String</span><span class="sxs-lookup"><span data-stu-id="9bf5e-146">String</span></span>|<span data-ttu-id="9bf5e-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-147">The publisher of the app.</span></span> <span data-ttu-id="9bf5e-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9bf5e-149">largeIcon</span></span>|[<span data-ttu-id="9bf5e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9bf5e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9bf5e-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9bf5e-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9bf5e-153">createdDateTime</span></span>|<span data-ttu-id="9bf5e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bf5e-154">DateTimeOffset</span></span>|<span data-ttu-id="9bf5e-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-155">The date and time the app was created.</span></span> <span data-ttu-id="9bf5e-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9bf5e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="9bf5e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bf5e-158">DateTimeOffset</span></span>|<span data-ttu-id="9bf5e-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="9bf5e-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9bf5e-161">isFeatured</span></span>|<span data-ttu-id="9bf5e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bf5e-162">Boolean</span></span>|<span data-ttu-id="9bf5e-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9bf5e-164">privacyInformationUrl</span></span>|<span data-ttu-id="9bf5e-165">String</span><span class="sxs-lookup"><span data-stu-id="9bf5e-165">String</span></span>|<span data-ttu-id="9bf5e-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-166">The privacy statement Url.</span></span> <span data-ttu-id="9bf5e-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9bf5e-168">informationUrl</span></span>|<span data-ttu-id="9bf5e-169">String</span><span class="sxs-lookup"><span data-stu-id="9bf5e-169">String</span></span>|<span data-ttu-id="9bf5e-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-170">The more information Url.</span></span> <span data-ttu-id="9bf5e-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-172">owner</span><span class="sxs-lookup"><span data-stu-id="9bf5e-172">owner</span></span>|<span data-ttu-id="9bf5e-173">String</span><span class="sxs-lookup"><span data-stu-id="9bf5e-173">String</span></span>|<span data-ttu-id="9bf5e-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-174">The owner of the app.</span></span> <span data-ttu-id="9bf5e-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-176">developer</span><span class="sxs-lookup"><span data-stu-id="9bf5e-176">developer</span></span>|<span data-ttu-id="9bf5e-177">String</span><span class="sxs-lookup"><span data-stu-id="9bf5e-177">String</span></span>|<span data-ttu-id="9bf5e-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-178">The developer of the app.</span></span> <span data-ttu-id="9bf5e-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-180">notes</span><span class="sxs-lookup"><span data-stu-id="9bf5e-180">notes</span></span>|<span data-ttu-id="9bf5e-181">String</span><span class="sxs-lookup"><span data-stu-id="9bf5e-181">String</span></span>|<span data-ttu-id="9bf5e-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-182">Notes for the app.</span></span> <span data-ttu-id="9bf5e-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="9bf5e-184">uploadState</span></span>|<span data-ttu-id="9bf5e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="9bf5e-185">Int32</span></span>|<span data-ttu-id="9bf5e-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-186">The upload state.</span></span> <span data-ttu-id="9bf5e-187">可能的值是：0 - `Not Ready` 、 1 - `Ready` 、 2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="9bf5e-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="9bf5e-189">publishingState</span></span>|[<span data-ttu-id="9bf5e-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9bf5e-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9bf5e-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-191">The publishing state for the app.</span></span> <span data-ttu-id="9bf5e-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9bf5e-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="9bf5e-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9bf5e-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9bf5e-195">isAssigned</span></span>|<span data-ttu-id="9bf5e-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bf5e-196">Boolean</span></span>|<span data-ttu-id="9bf5e-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9bf5e-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9bf5e-199">roleScopeTagIds</span></span>|<span data-ttu-id="9bf5e-200">字符串集合</span><span class="sxs-lookup"><span data-stu-id="9bf5e-200">String collection</span></span>|<span data-ttu-id="9bf5e-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9bf5e-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="9bf5e-203">dependentAppCount</span></span>|<span data-ttu-id="9bf5e-204">Int32</span><span class="sxs-lookup"><span data-stu-id="9bf5e-204">Int32</span></span>|<span data-ttu-id="9bf5e-205">子应用具有的依赖关系总数。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="9bf5e-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="9bf5e-207">supersedingAppCount</span></span>|<span data-ttu-id="9bf5e-208">Int32</span><span class="sxs-lookup"><span data-stu-id="9bf5e-208">Int32</span></span>|<span data-ttu-id="9bf5e-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="9bf5e-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="9bf5e-211">supersededAppCount</span></span>|<span data-ttu-id="9bf5e-212">Int32</span><span class="sxs-lookup"><span data-stu-id="9bf5e-212">Int32</span></span>|<span data-ttu-id="9bf5e-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="9bf5e-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bf5e-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9bf5e-215">committedContentVersion</span></span>|<span data-ttu-id="9bf5e-216">String</span><span class="sxs-lookup"><span data-stu-id="9bf5e-216">String</span></span>|<span data-ttu-id="9bf5e-217">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-217">The internal committed content version.</span></span> <span data-ttu-id="9bf5e-218">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9bf5e-219">fileName</span><span class="sxs-lookup"><span data-stu-id="9bf5e-219">fileName</span></span>|<span data-ttu-id="9bf5e-220">String</span><span class="sxs-lookup"><span data-stu-id="9bf5e-220">String</span></span>|<span data-ttu-id="9bf5e-221">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-221">The name of the main Lob application file.</span></span> <span data-ttu-id="9bf5e-222">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9bf5e-223">size</span><span class="sxs-lookup"><span data-stu-id="9bf5e-223">size</span></span>|<span data-ttu-id="9bf5e-224">Int64</span><span class="sxs-lookup"><span data-stu-id="9bf5e-224">Int64</span></span>|<span data-ttu-id="9bf5e-225">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="9bf5e-226">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bf5e-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9bf5e-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="9bf5e-227">bundleId</span></span>|<span data-ttu-id="9bf5e-228">String</span><span class="sxs-lookup"><span data-stu-id="9bf5e-228">String</span></span>|<span data-ttu-id="9bf5e-229">标识名称。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-229">The Identity Name.</span></span>|
|<span data-ttu-id="9bf5e-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="9bf5e-230">applicableDeviceType</span></span>|[<span data-ttu-id="9bf5e-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="9bf5e-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="9bf5e-232">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-232">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="9bf5e-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9bf5e-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9bf5e-234">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9bf5e-234">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="9bf5e-235">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="9bf5e-236">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9bf5e-236">expirationDateTime</span></span>|<span data-ttu-id="9bf5e-237">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bf5e-237">DateTimeOffset</span></span>|<span data-ttu-id="9bf5e-238">过期时间。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-238">The expiration time.</span></span>|
|<span data-ttu-id="9bf5e-239">versionNumber</span><span class="sxs-lookup"><span data-stu-id="9bf5e-239">versionNumber</span></span>|<span data-ttu-id="9bf5e-240">String</span><span class="sxs-lookup"><span data-stu-id="9bf5e-240">String</span></span>|<span data-ttu-id="9bf5e-241">iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-241">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9bf5e-242">buildNumber</span><span class="sxs-lookup"><span data-stu-id="9bf5e-242">buildNumber</span></span>|<span data-ttu-id="9bf5e-243">String</span><span class="sxs-lookup"><span data-stu-id="9bf5e-243">String</span></span>|<span data-ttu-id="9bf5e-244">iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-244">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9bf5e-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9bf5e-245">identityVersion</span></span>|<span data-ttu-id="9bf5e-246">String</span><span class="sxs-lookup"><span data-stu-id="9bf5e-246">String</span></span>|<span data-ttu-id="9bf5e-247">标识版本。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-247">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="9bf5e-248">响应</span><span class="sxs-lookup"><span data-stu-id="9bf5e-248">Response</span></span>
<span data-ttu-id="9bf5e-249">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-249">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bf5e-250">示例</span><span class="sxs-lookup"><span data-stu-id="9bf5e-250">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bf5e-251">请求</span><span class="sxs-lookup"><span data-stu-id="9bf5e-251">Request</span></span>
<span data-ttu-id="9bf5e-252">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-252">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1488

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="9bf5e-253">响应</span><span class="sxs-lookup"><span data-stu-id="9bf5e-253">Response</span></span>
<span data-ttu-id="9bf5e-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9bf5e-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1660

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```




