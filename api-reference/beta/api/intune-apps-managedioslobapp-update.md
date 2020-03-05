---
title: 更新 managedIOSLobApp
description: 更新 managedIOSLobApp 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2f8da4cc926c4425d8b483526de1a397ef07eca1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445083"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="cbb85-103">更新 managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="cbb85-103">Update managedIOSLobApp</span></span>

<span data-ttu-id="cbb85-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="cbb85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cbb85-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cbb85-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbb85-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cbb85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbb85-107">更新 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cbb85-107">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbb85-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cbb85-108">Prerequisites</span></span>
<span data-ttu-id="cbb85-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cbb85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbb85-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cbb85-111">Permission type</span></span>|<span data-ttu-id="cbb85-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cbb85-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbb85-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cbb85-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cbb85-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbb85-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cbb85-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cbb85-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbb85-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbb85-116">Not supported.</span></span>|
|<span data-ttu-id="cbb85-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cbb85-117">Application</span></span>|<span data-ttu-id="cbb85-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbb85-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbb85-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cbb85-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="cbb85-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cbb85-120">Request headers</span></span>
|<span data-ttu-id="cbb85-121">标头</span><span class="sxs-lookup"><span data-stu-id="cbb85-121">Header</span></span>|<span data-ttu-id="cbb85-122">值</span><span class="sxs-lookup"><span data-stu-id="cbb85-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbb85-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbb85-123">Authorization</span></span>|<span data-ttu-id="cbb85-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cbb85-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbb85-125">接受</span><span class="sxs-lookup"><span data-stu-id="cbb85-125">Accept</span></span>|<span data-ttu-id="cbb85-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cbb85-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbb85-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cbb85-127">Request body</span></span>
<span data-ttu-id="cbb85-128">在请求正文中，提供 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cbb85-128">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="cbb85-129">下表显示创建 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cbb85-129">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="cbb85-130">属性</span><span class="sxs-lookup"><span data-stu-id="cbb85-130">Property</span></span>|<span data-ttu-id="cbb85-131">类型</span><span class="sxs-lookup"><span data-stu-id="cbb85-131">Type</span></span>|<span data-ttu-id="cbb85-132">说明</span><span class="sxs-lookup"><span data-stu-id="cbb85-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbb85-133">id</span><span class="sxs-lookup"><span data-stu-id="cbb85-133">id</span></span>|<span data-ttu-id="cbb85-134">字符串</span><span class="sxs-lookup"><span data-stu-id="cbb85-134">String</span></span>|<span data-ttu-id="cbb85-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cbb85-135">Key of the entity.</span></span> <span data-ttu-id="cbb85-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbb85-137">displayName</span><span class="sxs-lookup"><span data-stu-id="cbb85-137">displayName</span></span>|<span data-ttu-id="cbb85-138">String</span><span class="sxs-lookup"><span data-stu-id="cbb85-138">String</span></span>|<span data-ttu-id="cbb85-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="cbb85-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cbb85-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbb85-141">说明</span><span class="sxs-lookup"><span data-stu-id="cbb85-141">description</span></span>|<span data-ttu-id="cbb85-142">字符串</span><span class="sxs-lookup"><span data-stu-id="cbb85-142">String</span></span>|<span data-ttu-id="cbb85-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="cbb85-143">The description of the app.</span></span> <span data-ttu-id="cbb85-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbb85-145">publisher</span><span class="sxs-lookup"><span data-stu-id="cbb85-145">publisher</span></span>|<span data-ttu-id="cbb85-146">String</span><span class="sxs-lookup"><span data-stu-id="cbb85-146">String</span></span>|<span data-ttu-id="cbb85-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="cbb85-147">The publisher of the app.</span></span> <span data-ttu-id="cbb85-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbb85-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cbb85-149">largeIcon</span></span>|[<span data-ttu-id="cbb85-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cbb85-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cbb85-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="cbb85-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cbb85-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbb85-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cbb85-153">createdDateTime</span></span>|<span data-ttu-id="cbb85-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbb85-154">DateTimeOffset</span></span>|<span data-ttu-id="cbb85-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cbb85-155">The date and time the app was created.</span></span> <span data-ttu-id="cbb85-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbb85-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cbb85-157">lastModifiedDateTime</span></span>|<span data-ttu-id="cbb85-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbb85-158">DateTimeOffset</span></span>|<span data-ttu-id="cbb85-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cbb85-159">The date and time the app was last modified.</span></span> <span data-ttu-id="cbb85-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbb85-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cbb85-161">isFeatured</span></span>|<span data-ttu-id="cbb85-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbb85-162">Boolean</span></span>|<span data-ttu-id="cbb85-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbb85-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cbb85-164">privacyInformationUrl</span></span>|<span data-ttu-id="cbb85-165">String</span><span class="sxs-lookup"><span data-stu-id="cbb85-165">String</span></span>|<span data-ttu-id="cbb85-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="cbb85-166">The privacy statement Url.</span></span> <span data-ttu-id="cbb85-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbb85-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cbb85-168">informationUrl</span></span>|<span data-ttu-id="cbb85-169">String</span><span class="sxs-lookup"><span data-stu-id="cbb85-169">String</span></span>|<span data-ttu-id="cbb85-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="cbb85-170">The more information Url.</span></span> <span data-ttu-id="cbb85-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbb85-172">owner</span><span class="sxs-lookup"><span data-stu-id="cbb85-172">owner</span></span>|<span data-ttu-id="cbb85-173">String</span><span class="sxs-lookup"><span data-stu-id="cbb85-173">String</span></span>|<span data-ttu-id="cbb85-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="cbb85-174">The owner of the app.</span></span> <span data-ttu-id="cbb85-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbb85-176">developer</span><span class="sxs-lookup"><span data-stu-id="cbb85-176">developer</span></span>|<span data-ttu-id="cbb85-177">String</span><span class="sxs-lookup"><span data-stu-id="cbb85-177">String</span></span>|<span data-ttu-id="cbb85-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="cbb85-178">The developer of the app.</span></span> <span data-ttu-id="cbb85-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbb85-180">notes</span><span class="sxs-lookup"><span data-stu-id="cbb85-180">notes</span></span>|<span data-ttu-id="cbb85-181">String</span><span class="sxs-lookup"><span data-stu-id="cbb85-181">String</span></span>|<span data-ttu-id="cbb85-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="cbb85-182">Notes for the app.</span></span> <span data-ttu-id="cbb85-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbb85-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="cbb85-184">uploadState</span></span>|<span data-ttu-id="cbb85-185">Int32</span><span class="sxs-lookup"><span data-stu-id="cbb85-185">Int32</span></span>|<span data-ttu-id="cbb85-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="cbb85-186">The upload state.</span></span> <span data-ttu-id="cbb85-187">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbb85-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="cbb85-188">publishingState</span></span>|[<span data-ttu-id="cbb85-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cbb85-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cbb85-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="cbb85-190">The publishing state for the app.</span></span> <span data-ttu-id="cbb85-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="cbb85-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cbb85-192">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="cbb85-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="cbb85-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="cbb85-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cbb85-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="cbb85-194">isAssigned</span></span>|<span data-ttu-id="cbb85-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbb85-195">Boolean</span></span>|<span data-ttu-id="cbb85-196">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="cbb85-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="cbb85-197">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbb85-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cbb85-198">roleScopeTagIds</span></span>|<span data-ttu-id="cbb85-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="cbb85-199">String collection</span></span>|<span data-ttu-id="cbb85-200">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="cbb85-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="cbb85-201">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbb85-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="cbb85-202">dependentAppCount</span></span>|<span data-ttu-id="cbb85-203">Int32</span><span class="sxs-lookup"><span data-stu-id="cbb85-203">Int32</span></span>|<span data-ttu-id="cbb85-204">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="cbb85-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="cbb85-205">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbb85-206">appAvailability</span><span class="sxs-lookup"><span data-stu-id="cbb85-206">appAvailability</span></span>|[<span data-ttu-id="cbb85-207">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="cbb85-207">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="cbb85-208">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="cbb85-208">The Application's availability.</span></span> <span data-ttu-id="cbb85-209">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="cbb85-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="cbb85-210">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="cbb85-210">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="cbb85-211">version</span><span class="sxs-lookup"><span data-stu-id="cbb85-211">version</span></span>|<span data-ttu-id="cbb85-212">String</span><span class="sxs-lookup"><span data-stu-id="cbb85-212">String</span></span>|<span data-ttu-id="cbb85-213">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="cbb85-213">The Application's version.</span></span> <span data-ttu-id="cbb85-214">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-214">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="cbb85-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="cbb85-215">committedContentVersion</span></span>|<span data-ttu-id="cbb85-216">String</span><span class="sxs-lookup"><span data-stu-id="cbb85-216">String</span></span>|<span data-ttu-id="cbb85-217">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="cbb85-217">The internal committed content version.</span></span> <span data-ttu-id="cbb85-218">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-218">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="cbb85-219">fileName</span><span class="sxs-lookup"><span data-stu-id="cbb85-219">fileName</span></span>|<span data-ttu-id="cbb85-220">String</span><span class="sxs-lookup"><span data-stu-id="cbb85-220">String</span></span>|<span data-ttu-id="cbb85-221">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="cbb85-221">The name of the main Lob application file.</span></span> <span data-ttu-id="cbb85-222">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-222">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="cbb85-223">size</span><span class="sxs-lookup"><span data-stu-id="cbb85-223">size</span></span>|<span data-ttu-id="cbb85-224">Int64</span><span class="sxs-lookup"><span data-stu-id="cbb85-224">Int64</span></span>|<span data-ttu-id="cbb85-225">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="cbb85-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="cbb85-226">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbb85-226">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="cbb85-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="cbb85-227">bundleId</span></span>|<span data-ttu-id="cbb85-228">String</span><span class="sxs-lookup"><span data-stu-id="cbb85-228">String</span></span>|<span data-ttu-id="cbb85-229">标识名称。</span><span class="sxs-lookup"><span data-stu-id="cbb85-229">The Identity Name.</span></span>|
|<span data-ttu-id="cbb85-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="cbb85-230">applicableDeviceType</span></span>|[<span data-ttu-id="cbb85-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="cbb85-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="cbb85-232">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="cbb85-232">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="cbb85-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cbb85-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="cbb85-234">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cbb85-234">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="cbb85-235">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="cbb85-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="cbb85-236">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cbb85-236">expirationDateTime</span></span>|<span data-ttu-id="cbb85-237">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbb85-237">DateTimeOffset</span></span>|<span data-ttu-id="cbb85-238">过期时间。</span><span class="sxs-lookup"><span data-stu-id="cbb85-238">The expiration time.</span></span>|
|<span data-ttu-id="cbb85-239">versionNumber</span><span class="sxs-lookup"><span data-stu-id="cbb85-239">versionNumber</span></span>|<span data-ttu-id="cbb85-240">String</span><span class="sxs-lookup"><span data-stu-id="cbb85-240">String</span></span>|<span data-ttu-id="cbb85-241">托管 iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="cbb85-241">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="cbb85-242">buildNumber</span><span class="sxs-lookup"><span data-stu-id="cbb85-242">buildNumber</span></span>|<span data-ttu-id="cbb85-243">String</span><span class="sxs-lookup"><span data-stu-id="cbb85-243">String</span></span>|<span data-ttu-id="cbb85-244">托管 iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="cbb85-244">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="cbb85-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="cbb85-245">identityVersion</span></span>|<span data-ttu-id="cbb85-246">String</span><span class="sxs-lookup"><span data-stu-id="cbb85-246">String</span></span>|<span data-ttu-id="cbb85-247">标识版本。</span><span class="sxs-lookup"><span data-stu-id="cbb85-247">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="cbb85-248">响应</span><span class="sxs-lookup"><span data-stu-id="cbb85-248">Response</span></span>
<span data-ttu-id="cbb85-249">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cbb85-249">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbb85-250">示例</span><span class="sxs-lookup"><span data-stu-id="cbb85-250">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbb85-251">请求</span><span class="sxs-lookup"><span data-stu-id="cbb85-251">Request</span></span>
<span data-ttu-id="cbb85-252">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cbb85-252">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1489

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
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="cbb85-253">响应</span><span class="sxs-lookup"><span data-stu-id="cbb85-253">Response</span></span>
<span data-ttu-id="cbb85-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cbb85-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1661

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
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```





