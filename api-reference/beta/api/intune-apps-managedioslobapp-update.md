---
title: 更新 managedIOSLobApp
description: 更新 managedIOSLobApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4de8289ce0ee128acc8c2c12622bbc098412b3ef
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157237"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="436da-103">更新 managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="436da-103">Update managedIOSLobApp</span></span>

<span data-ttu-id="436da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="436da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="436da-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="436da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="436da-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="436da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="436da-107">更新 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="436da-107">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="436da-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="436da-108">Prerequisites</span></span>
<span data-ttu-id="436da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="436da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="436da-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="436da-111">Permission type</span></span>|<span data-ttu-id="436da-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="436da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="436da-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="436da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="436da-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="436da-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="436da-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="436da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="436da-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="436da-116">Not supported.</span></span>|
|<span data-ttu-id="436da-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="436da-117">Application</span></span>|<span data-ttu-id="436da-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="436da-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="436da-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="436da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="436da-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="436da-120">Request headers</span></span>
|<span data-ttu-id="436da-121">标头</span><span class="sxs-lookup"><span data-stu-id="436da-121">Header</span></span>|<span data-ttu-id="436da-122">值</span><span class="sxs-lookup"><span data-stu-id="436da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="436da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="436da-123">Authorization</span></span>|<span data-ttu-id="436da-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="436da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="436da-125">接受</span><span class="sxs-lookup"><span data-stu-id="436da-125">Accept</span></span>|<span data-ttu-id="436da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="436da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="436da-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="436da-127">Request body</span></span>
<span data-ttu-id="436da-128">在请求正文中，提供 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="436da-128">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="436da-129">下表显示创建 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="436da-129">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="436da-130">属性</span><span class="sxs-lookup"><span data-stu-id="436da-130">Property</span></span>|<span data-ttu-id="436da-131">类型</span><span class="sxs-lookup"><span data-stu-id="436da-131">Type</span></span>|<span data-ttu-id="436da-132">说明</span><span class="sxs-lookup"><span data-stu-id="436da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="436da-133">id</span><span class="sxs-lookup"><span data-stu-id="436da-133">id</span></span>|<span data-ttu-id="436da-134">String</span><span class="sxs-lookup"><span data-stu-id="436da-134">String</span></span>|<span data-ttu-id="436da-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="436da-135">Key of the entity.</span></span> <span data-ttu-id="436da-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-137">displayName</span><span class="sxs-lookup"><span data-stu-id="436da-137">displayName</span></span>|<span data-ttu-id="436da-138">String</span><span class="sxs-lookup"><span data-stu-id="436da-138">String</span></span>|<span data-ttu-id="436da-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="436da-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="436da-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-141">说明</span><span class="sxs-lookup"><span data-stu-id="436da-141">description</span></span>|<span data-ttu-id="436da-142">String</span><span class="sxs-lookup"><span data-stu-id="436da-142">String</span></span>|<span data-ttu-id="436da-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="436da-143">The description of the app.</span></span> <span data-ttu-id="436da-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-145">publisher</span><span class="sxs-lookup"><span data-stu-id="436da-145">publisher</span></span>|<span data-ttu-id="436da-146">String</span><span class="sxs-lookup"><span data-stu-id="436da-146">String</span></span>|<span data-ttu-id="436da-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="436da-147">The publisher of the app.</span></span> <span data-ttu-id="436da-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="436da-149">largeIcon</span></span>|[<span data-ttu-id="436da-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="436da-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="436da-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="436da-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="436da-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="436da-153">createdDateTime</span></span>|<span data-ttu-id="436da-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="436da-154">DateTimeOffset</span></span>|<span data-ttu-id="436da-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="436da-155">The date and time the app was created.</span></span> <span data-ttu-id="436da-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="436da-157">lastModifiedDateTime</span></span>|<span data-ttu-id="436da-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="436da-158">DateTimeOffset</span></span>|<span data-ttu-id="436da-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="436da-159">The date and time the app was last modified.</span></span> <span data-ttu-id="436da-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="436da-161">isFeatured</span></span>|<span data-ttu-id="436da-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="436da-162">Boolean</span></span>|<span data-ttu-id="436da-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="436da-164">privacyInformationUrl</span></span>|<span data-ttu-id="436da-165">String</span><span class="sxs-lookup"><span data-stu-id="436da-165">String</span></span>|<span data-ttu-id="436da-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="436da-166">The privacy statement Url.</span></span> <span data-ttu-id="436da-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="436da-168">informationUrl</span></span>|<span data-ttu-id="436da-169">String</span><span class="sxs-lookup"><span data-stu-id="436da-169">String</span></span>|<span data-ttu-id="436da-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="436da-170">The more information Url.</span></span> <span data-ttu-id="436da-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-172">owner</span><span class="sxs-lookup"><span data-stu-id="436da-172">owner</span></span>|<span data-ttu-id="436da-173">String</span><span class="sxs-lookup"><span data-stu-id="436da-173">String</span></span>|<span data-ttu-id="436da-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="436da-174">The owner of the app.</span></span> <span data-ttu-id="436da-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-176">developer</span><span class="sxs-lookup"><span data-stu-id="436da-176">developer</span></span>|<span data-ttu-id="436da-177">String</span><span class="sxs-lookup"><span data-stu-id="436da-177">String</span></span>|<span data-ttu-id="436da-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="436da-178">The developer of the app.</span></span> <span data-ttu-id="436da-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-180">notes</span><span class="sxs-lookup"><span data-stu-id="436da-180">notes</span></span>|<span data-ttu-id="436da-181">String</span><span class="sxs-lookup"><span data-stu-id="436da-181">String</span></span>|<span data-ttu-id="436da-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="436da-182">Notes for the app.</span></span> <span data-ttu-id="436da-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="436da-184">uploadState</span></span>|<span data-ttu-id="436da-185">Int32</span><span class="sxs-lookup"><span data-stu-id="436da-185">Int32</span></span>|<span data-ttu-id="436da-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="436da-186">The upload state.</span></span> <span data-ttu-id="436da-187">可能的值是：0 - `Not Ready` 、 1 - `Ready` 、 2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="436da-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="436da-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="436da-189">publishingState</span></span>|[<span data-ttu-id="436da-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="436da-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="436da-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="436da-191">The publishing state for the app.</span></span> <span data-ttu-id="436da-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="436da-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="436da-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="436da-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="436da-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="436da-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="436da-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="436da-195">isAssigned</span></span>|<span data-ttu-id="436da-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="436da-196">Boolean</span></span>|<span data-ttu-id="436da-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="436da-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="436da-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="436da-199">roleScopeTagIds</span></span>|<span data-ttu-id="436da-200">字符串集合</span><span class="sxs-lookup"><span data-stu-id="436da-200">String collection</span></span>|<span data-ttu-id="436da-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="436da-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="436da-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="436da-203">dependentAppCount</span></span>|<span data-ttu-id="436da-204">Int32</span><span class="sxs-lookup"><span data-stu-id="436da-204">Int32</span></span>|<span data-ttu-id="436da-205">子应用具有的依赖关系总数。</span><span class="sxs-lookup"><span data-stu-id="436da-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="436da-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="436da-207">supersedingAppCount</span></span>|<span data-ttu-id="436da-208">Int32</span><span class="sxs-lookup"><span data-stu-id="436da-208">Int32</span></span>|<span data-ttu-id="436da-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="436da-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="436da-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="436da-211">supersededAppCount</span></span>|<span data-ttu-id="436da-212">Int32</span><span class="sxs-lookup"><span data-stu-id="436da-212">Int32</span></span>|<span data-ttu-id="436da-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="436da-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="436da-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="436da-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="436da-215">appAvailability</span></span>|[<span data-ttu-id="436da-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="436da-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="436da-217">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="436da-217">The Application's availability.</span></span> <span data-ttu-id="436da-218">继承自 [managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="436da-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="436da-219">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="436da-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="436da-220">version</span><span class="sxs-lookup"><span data-stu-id="436da-220">version</span></span>|<span data-ttu-id="436da-221">String</span><span class="sxs-lookup"><span data-stu-id="436da-221">String</span></span>|<span data-ttu-id="436da-222">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="436da-222">The Application's version.</span></span> <span data-ttu-id="436da-223">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="436da-224">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="436da-224">committedContentVersion</span></span>|<span data-ttu-id="436da-225">String</span><span class="sxs-lookup"><span data-stu-id="436da-225">String</span></span>|<span data-ttu-id="436da-226">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="436da-226">The internal committed content version.</span></span> <span data-ttu-id="436da-227">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-227">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="436da-228">fileName</span><span class="sxs-lookup"><span data-stu-id="436da-228">fileName</span></span>|<span data-ttu-id="436da-229">String</span><span class="sxs-lookup"><span data-stu-id="436da-229">String</span></span>|<span data-ttu-id="436da-230">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="436da-230">The name of the main Lob application file.</span></span> <span data-ttu-id="436da-231">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-231">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="436da-232">size</span><span class="sxs-lookup"><span data-stu-id="436da-232">size</span></span>|<span data-ttu-id="436da-233">Int64</span><span class="sxs-lookup"><span data-stu-id="436da-233">Int64</span></span>|<span data-ttu-id="436da-234">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="436da-234">The total size, including all uploaded files.</span></span> <span data-ttu-id="436da-235">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="436da-235">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="436da-236">bundleId</span><span class="sxs-lookup"><span data-stu-id="436da-236">bundleId</span></span>|<span data-ttu-id="436da-237">String</span><span class="sxs-lookup"><span data-stu-id="436da-237">String</span></span>|<span data-ttu-id="436da-238">标识名称。</span><span class="sxs-lookup"><span data-stu-id="436da-238">The Identity Name.</span></span>|
|<span data-ttu-id="436da-239">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="436da-239">applicableDeviceType</span></span>|[<span data-ttu-id="436da-240">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="436da-240">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="436da-241">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="436da-241">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="436da-242">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="436da-242">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="436da-243">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="436da-243">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="436da-244">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="436da-244">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="436da-245">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="436da-245">expirationDateTime</span></span>|<span data-ttu-id="436da-246">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="436da-246">DateTimeOffset</span></span>|<span data-ttu-id="436da-247">过期时间。</span><span class="sxs-lookup"><span data-stu-id="436da-247">The expiration time.</span></span>|
|<span data-ttu-id="436da-248">versionNumber</span><span class="sxs-lookup"><span data-stu-id="436da-248">versionNumber</span></span>|<span data-ttu-id="436da-249">String</span><span class="sxs-lookup"><span data-stu-id="436da-249">String</span></span>|<span data-ttu-id="436da-250">托管 iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="436da-250">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="436da-251">buildNumber</span><span class="sxs-lookup"><span data-stu-id="436da-251">buildNumber</span></span>|<span data-ttu-id="436da-252">String</span><span class="sxs-lookup"><span data-stu-id="436da-252">String</span></span>|<span data-ttu-id="436da-253">托管 iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="436da-253">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="436da-254">identityVersion</span><span class="sxs-lookup"><span data-stu-id="436da-254">identityVersion</span></span>|<span data-ttu-id="436da-255">String</span><span class="sxs-lookup"><span data-stu-id="436da-255">String</span></span>|<span data-ttu-id="436da-256">标识版本。</span><span class="sxs-lookup"><span data-stu-id="436da-256">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="436da-257">响应</span><span class="sxs-lookup"><span data-stu-id="436da-257">Response</span></span>
<span data-ttu-id="436da-258">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="436da-258">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="436da-259">示例</span><span class="sxs-lookup"><span data-stu-id="436da-259">Example</span></span>

### <a name="request"></a><span data-ttu-id="436da-260">请求</span><span class="sxs-lookup"><span data-stu-id="436da-260">Request</span></span>
<span data-ttu-id="436da-261">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="436da-261">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1566

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="436da-262">响应</span><span class="sxs-lookup"><span data-stu-id="436da-262">Response</span></span>
<span data-ttu-id="436da-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="436da-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1738

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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




