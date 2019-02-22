---
title: 更新 managedAndroidLobApp
description: 更新 managedAndroidLobApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e43a6b1babb23c56818391e6fd89da58005dd8e0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157503"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="cfec6-103">更新 managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="cfec6-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="cfec6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cfec6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfec6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cfec6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfec6-106">更新 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cfec6-106">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cfec6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cfec6-107">Prerequisites</span></span>
<span data-ttu-id="cfec6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cfec6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cfec6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cfec6-110">Permission type</span></span>|<span data-ttu-id="cfec6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cfec6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfec6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cfec6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cfec6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfec6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cfec6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cfec6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfec6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfec6-115">Not supported.</span></span>|
|<span data-ttu-id="cfec6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cfec6-116">Application</span></span>|<span data-ttu-id="cfec6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfec6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfec6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cfec6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="cfec6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cfec6-119">Request headers</span></span>
|<span data-ttu-id="cfec6-120">标头</span><span class="sxs-lookup"><span data-stu-id="cfec6-120">Header</span></span>|<span data-ttu-id="cfec6-121">值</span><span class="sxs-lookup"><span data-stu-id="cfec6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfec6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfec6-122">Authorization</span></span>|<span data-ttu-id="cfec6-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cfec6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfec6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cfec6-124">Accept</span></span>|<span data-ttu-id="cfec6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cfec6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfec6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cfec6-126">Request body</span></span>
<span data-ttu-id="cfec6-127">在请求正文中，提供 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cfec6-127">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="cfec6-128">下表显示了创建 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cfec6-128">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="cfec6-129">属性</span><span class="sxs-lookup"><span data-stu-id="cfec6-129">Property</span></span>|<span data-ttu-id="cfec6-130">类型</span><span class="sxs-lookup"><span data-stu-id="cfec6-130">Type</span></span>|<span data-ttu-id="cfec6-131">说明</span><span class="sxs-lookup"><span data-stu-id="cfec6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfec6-132">id</span><span class="sxs-lookup"><span data-stu-id="cfec6-132">id</span></span>|<span data-ttu-id="cfec6-133">字串符号</span><span class="sxs-lookup"><span data-stu-id="cfec6-133">String</span></span>|<span data-ttu-id="cfec6-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cfec6-134">Key of the entity.</span></span> <span data-ttu-id="cfec6-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cfec6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cfec6-136">displayName</span></span>|<span data-ttu-id="cfec6-137">字符串</span><span class="sxs-lookup"><span data-stu-id="cfec6-137">String</span></span>|<span data-ttu-id="cfec6-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="cfec6-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cfec6-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cfec6-140">description</span><span class="sxs-lookup"><span data-stu-id="cfec6-140">description</span></span>|<span data-ttu-id="cfec6-141">字符串</span><span class="sxs-lookup"><span data-stu-id="cfec6-141">String</span></span>|<span data-ttu-id="cfec6-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="cfec6-142">The description of the app.</span></span> <span data-ttu-id="cfec6-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cfec6-144">publisher</span><span class="sxs-lookup"><span data-stu-id="cfec6-144">publisher</span></span>|<span data-ttu-id="cfec6-145">字符串</span><span class="sxs-lookup"><span data-stu-id="cfec6-145">String</span></span>|<span data-ttu-id="cfec6-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="cfec6-146">The publisher of the app.</span></span> <span data-ttu-id="cfec6-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cfec6-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cfec6-148">largeIcon</span></span>|[<span data-ttu-id="cfec6-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cfec6-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cfec6-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="cfec6-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cfec6-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cfec6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cfec6-152">createdDateTime</span></span>|<span data-ttu-id="cfec6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfec6-153">DateTimeOffset</span></span>|<span data-ttu-id="cfec6-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cfec6-154">The date and time the app was created.</span></span> <span data-ttu-id="cfec6-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cfec6-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cfec6-156">lastModifiedDateTime</span></span>|<span data-ttu-id="cfec6-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfec6-157">DateTimeOffset</span></span>|<span data-ttu-id="cfec6-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cfec6-158">The date and time the app was last modified.</span></span> <span data-ttu-id="cfec6-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cfec6-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cfec6-160">isFeatured</span></span>|<span data-ttu-id="cfec6-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfec6-161">Boolean</span></span>|<span data-ttu-id="cfec6-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cfec6-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cfec6-163">privacyInformationUrl</span></span>|<span data-ttu-id="cfec6-164">字符串</span><span class="sxs-lookup"><span data-stu-id="cfec6-164">String</span></span>|<span data-ttu-id="cfec6-165">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="cfec6-165">The privacy statement Url.</span></span> <span data-ttu-id="cfec6-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cfec6-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cfec6-167">informationUrl</span></span>|<span data-ttu-id="cfec6-168">字符串</span><span class="sxs-lookup"><span data-stu-id="cfec6-168">String</span></span>|<span data-ttu-id="cfec6-169">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="cfec6-169">The more information Url.</span></span> <span data-ttu-id="cfec6-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cfec6-171">owner</span><span class="sxs-lookup"><span data-stu-id="cfec6-171">owner</span></span>|<span data-ttu-id="cfec6-172">String</span><span class="sxs-lookup"><span data-stu-id="cfec6-172">String</span></span>|<span data-ttu-id="cfec6-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="cfec6-173">The owner of the app.</span></span> <span data-ttu-id="cfec6-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cfec6-175">developer</span><span class="sxs-lookup"><span data-stu-id="cfec6-175">developer</span></span>|<span data-ttu-id="cfec6-176">String</span><span class="sxs-lookup"><span data-stu-id="cfec6-176">String</span></span>|<span data-ttu-id="cfec6-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="cfec6-177">The developer of the app.</span></span> <span data-ttu-id="cfec6-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cfec6-179">notes</span><span class="sxs-lookup"><span data-stu-id="cfec6-179">notes</span></span>|<span data-ttu-id="cfec6-180">String</span><span class="sxs-lookup"><span data-stu-id="cfec6-180">String</span></span>|<span data-ttu-id="cfec6-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="cfec6-181">Notes for the app.</span></span> <span data-ttu-id="cfec6-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cfec6-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="cfec6-183">uploadState</span></span>|<span data-ttu-id="cfec6-184">Int32</span><span class="sxs-lookup"><span data-stu-id="cfec6-184">Int32</span></span>|<span data-ttu-id="cfec6-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="cfec6-185">The upload state.</span></span> <span data-ttu-id="cfec6-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cfec6-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="cfec6-187">publishingState</span></span>|[<span data-ttu-id="cfec6-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cfec6-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cfec6-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="cfec6-189">The publishing state for the app.</span></span> <span data-ttu-id="cfec6-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="cfec6-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cfec6-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="cfec6-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="cfec6-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="cfec6-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cfec6-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="cfec6-193">isAssigned</span></span>|<span data-ttu-id="cfec6-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfec6-194">Boolean</span></span>|<span data-ttu-id="cfec6-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="cfec6-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="cfec6-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cfec6-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cfec6-197">roleScopeTagIds</span></span>|<span data-ttu-id="cfec6-198">String collection</span><span class="sxs-lookup"><span data-stu-id="cfec6-198">String collection</span></span>|<span data-ttu-id="cfec6-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="cfec6-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="cfec6-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cfec6-201">appAvailability</span><span class="sxs-lookup"><span data-stu-id="cfec6-201">appAvailability</span></span>|[<span data-ttu-id="cfec6-202">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="cfec6-202">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="cfec6-203">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="cfec6-203">The Application's availability.</span></span> <span data-ttu-id="cfec6-204">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="cfec6-204">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="cfec6-205">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="cfec6-205">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="cfec6-206">version</span><span class="sxs-lookup"><span data-stu-id="cfec6-206">version</span></span>|<span data-ttu-id="cfec6-207">字符串</span><span class="sxs-lookup"><span data-stu-id="cfec6-207">String</span></span>|<span data-ttu-id="cfec6-208">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="cfec6-208">The Application's version.</span></span> <span data-ttu-id="cfec6-209">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="cfec6-210">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="cfec6-210">committedContentVersion</span></span>|<span data-ttu-id="cfec6-211">字符串</span><span class="sxs-lookup"><span data-stu-id="cfec6-211">String</span></span>|<span data-ttu-id="cfec6-212">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="cfec6-212">The internal committed content version.</span></span> <span data-ttu-id="cfec6-213">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-213">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="cfec6-214">fileName</span><span class="sxs-lookup"><span data-stu-id="cfec6-214">fileName</span></span>|<span data-ttu-id="cfec6-215">字符串</span><span class="sxs-lookup"><span data-stu-id="cfec6-215">String</span></span>|<span data-ttu-id="cfec6-216">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="cfec6-216">The name of the main Lob application file.</span></span> <span data-ttu-id="cfec6-217">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="cfec6-218">size</span><span class="sxs-lookup"><span data-stu-id="cfec6-218">size</span></span>|<span data-ttu-id="cfec6-219">Int64</span><span class="sxs-lookup"><span data-stu-id="cfec6-219">Int64</span></span>|<span data-ttu-id="cfec6-220">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="cfec6-220">The total size, including all uploaded files.</span></span> <span data-ttu-id="cfec6-221">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfec6-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="cfec6-222">packageId</span><span class="sxs-lookup"><span data-stu-id="cfec6-222">packageId</span></span>|<span data-ttu-id="cfec6-223">字符串</span><span class="sxs-lookup"><span data-stu-id="cfec6-223">String</span></span>|<span data-ttu-id="cfec6-224">包标识符。</span><span class="sxs-lookup"><span data-stu-id="cfec6-224">The package identifier.</span></span>|
|<span data-ttu-id="cfec6-225">identityName</span><span class="sxs-lookup"><span data-stu-id="cfec6-225">identityName</span></span>|<span data-ttu-id="cfec6-226">String</span><span class="sxs-lookup"><span data-stu-id="cfec6-226">String</span></span>|<span data-ttu-id="cfec6-227">标识名称。</span><span class="sxs-lookup"><span data-stu-id="cfec6-227">The Identity Name.</span></span>|
|<span data-ttu-id="cfec6-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cfec6-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="cfec6-229">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cfec6-229">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="cfec6-230">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="cfec6-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="cfec6-231">versionName</span><span class="sxs-lookup"><span data-stu-id="cfec6-231">versionName</span></span>|<span data-ttu-id="cfec6-232">字符串</span><span class="sxs-lookup"><span data-stu-id="cfec6-232">String</span></span>|<span data-ttu-id="cfec6-233">托管 Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="cfec6-233">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="cfec6-234">versionCode</span><span class="sxs-lookup"><span data-stu-id="cfec6-234">versionCode</span></span>|<span data-ttu-id="cfec6-235">String</span><span class="sxs-lookup"><span data-stu-id="cfec6-235">String</span></span>|<span data-ttu-id="cfec6-236">托管 Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="cfec6-236">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="cfec6-237">identityVersion</span><span class="sxs-lookup"><span data-stu-id="cfec6-237">identityVersion</span></span>|<span data-ttu-id="cfec6-238">String</span><span class="sxs-lookup"><span data-stu-id="cfec6-238">String</span></span>|<span data-ttu-id="cfec6-239">标识版本。</span><span class="sxs-lookup"><span data-stu-id="cfec6-239">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="cfec6-240">响应</span><span class="sxs-lookup"><span data-stu-id="cfec6-240">Response</span></span>
<span data-ttu-id="cfec6-241">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cfec6-241">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfec6-242">示例</span><span class="sxs-lookup"><span data-stu-id="cfec6-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfec6-243">请求</span><span class="sxs-lookup"><span data-stu-id="cfec6-243">Request</span></span>
<span data-ttu-id="cfec6-244">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cfec6-244">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1464

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="cfec6-245">响应</span><span class="sxs-lookup"><span data-stu-id="cfec6-245">Response</span></span>
<span data-ttu-id="cfec6-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cfec6-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1636

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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




