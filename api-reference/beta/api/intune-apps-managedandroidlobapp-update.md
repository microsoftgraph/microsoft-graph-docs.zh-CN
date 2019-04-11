---
title: 更新 managedAndroidLobApp
description: 更新 managedAndroidLobApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a5d674a1f980e16348e67ce4165c218a3967ca8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807495"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="4390a-103">更新 managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="4390a-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="4390a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4390a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4390a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4390a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4390a-106">更新 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4390a-106">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4390a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4390a-107">Prerequisites</span></span>
<span data-ttu-id="4390a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4390a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4390a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4390a-110">Permission type</span></span>|<span data-ttu-id="4390a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4390a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4390a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4390a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4390a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4390a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4390a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4390a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4390a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4390a-115">Not supported.</span></span>|
|<span data-ttu-id="4390a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4390a-116">Application</span></span>|<span data-ttu-id="4390a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4390a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4390a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4390a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4390a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4390a-119">Request headers</span></span>
|<span data-ttu-id="4390a-120">标头</span><span class="sxs-lookup"><span data-stu-id="4390a-120">Header</span></span>|<span data-ttu-id="4390a-121">值</span><span class="sxs-lookup"><span data-stu-id="4390a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4390a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4390a-122">Authorization</span></span>|<span data-ttu-id="4390a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4390a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4390a-124">接受</span><span class="sxs-lookup"><span data-stu-id="4390a-124">Accept</span></span>|<span data-ttu-id="4390a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4390a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4390a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4390a-126">Request body</span></span>
<span data-ttu-id="4390a-127">在请求正文中，提供 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4390a-127">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="4390a-128">下表显示了创建 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4390a-128">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="4390a-129">属性</span><span class="sxs-lookup"><span data-stu-id="4390a-129">Property</span></span>|<span data-ttu-id="4390a-130">类型</span><span class="sxs-lookup"><span data-stu-id="4390a-130">Type</span></span>|<span data-ttu-id="4390a-131">说明</span><span class="sxs-lookup"><span data-stu-id="4390a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4390a-132">id</span><span class="sxs-lookup"><span data-stu-id="4390a-132">id</span></span>|<span data-ttu-id="4390a-133">String</span><span class="sxs-lookup"><span data-stu-id="4390a-133">String</span></span>|<span data-ttu-id="4390a-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4390a-134">Key of the entity.</span></span> <span data-ttu-id="4390a-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4390a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4390a-136">displayName</span></span>|<span data-ttu-id="4390a-137">String</span><span class="sxs-lookup"><span data-stu-id="4390a-137">String</span></span>|<span data-ttu-id="4390a-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="4390a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4390a-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4390a-140">description</span><span class="sxs-lookup"><span data-stu-id="4390a-140">description</span></span>|<span data-ttu-id="4390a-141">String</span><span class="sxs-lookup"><span data-stu-id="4390a-141">String</span></span>|<span data-ttu-id="4390a-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="4390a-142">The description of the app.</span></span> <span data-ttu-id="4390a-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4390a-144">publisher</span><span class="sxs-lookup"><span data-stu-id="4390a-144">publisher</span></span>|<span data-ttu-id="4390a-145">String</span><span class="sxs-lookup"><span data-stu-id="4390a-145">String</span></span>|<span data-ttu-id="4390a-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="4390a-146">The publisher of the app.</span></span> <span data-ttu-id="4390a-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4390a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4390a-148">largeIcon</span></span>|[<span data-ttu-id="4390a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4390a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4390a-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="4390a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4390a-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4390a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4390a-152">createdDateTime</span></span>|<span data-ttu-id="4390a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4390a-153">DateTimeOffset</span></span>|<span data-ttu-id="4390a-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4390a-154">The date and time the app was created.</span></span> <span data-ttu-id="4390a-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4390a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4390a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4390a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4390a-157">DateTimeOffset</span></span>|<span data-ttu-id="4390a-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4390a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="4390a-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4390a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4390a-160">isFeatured</span></span>|<span data-ttu-id="4390a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4390a-161">Boolean</span></span>|<span data-ttu-id="4390a-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4390a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4390a-163">privacyInformationUrl</span></span>|<span data-ttu-id="4390a-164">String</span><span class="sxs-lookup"><span data-stu-id="4390a-164">String</span></span>|<span data-ttu-id="4390a-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="4390a-165">The privacy statement Url.</span></span> <span data-ttu-id="4390a-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4390a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4390a-167">informationUrl</span></span>|<span data-ttu-id="4390a-168">String</span><span class="sxs-lookup"><span data-stu-id="4390a-168">String</span></span>|<span data-ttu-id="4390a-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="4390a-169">The more information Url.</span></span> <span data-ttu-id="4390a-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4390a-171">owner</span><span class="sxs-lookup"><span data-stu-id="4390a-171">owner</span></span>|<span data-ttu-id="4390a-172">字符串</span><span class="sxs-lookup"><span data-stu-id="4390a-172">String</span></span>|<span data-ttu-id="4390a-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="4390a-173">The owner of the app.</span></span> <span data-ttu-id="4390a-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4390a-175">developer</span><span class="sxs-lookup"><span data-stu-id="4390a-175">developer</span></span>|<span data-ttu-id="4390a-176">String</span><span class="sxs-lookup"><span data-stu-id="4390a-176">String</span></span>|<span data-ttu-id="4390a-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="4390a-177">The developer of the app.</span></span> <span data-ttu-id="4390a-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4390a-179">notes</span><span class="sxs-lookup"><span data-stu-id="4390a-179">notes</span></span>|<span data-ttu-id="4390a-180">String</span><span class="sxs-lookup"><span data-stu-id="4390a-180">String</span></span>|<span data-ttu-id="4390a-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="4390a-181">Notes for the app.</span></span> <span data-ttu-id="4390a-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4390a-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="4390a-183">uploadState</span></span>|<span data-ttu-id="4390a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="4390a-184">Int32</span></span>|<span data-ttu-id="4390a-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="4390a-185">The upload state.</span></span> <span data-ttu-id="4390a-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4390a-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="4390a-187">publishingState</span></span>|[<span data-ttu-id="4390a-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4390a-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4390a-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="4390a-189">The publishing state for the app.</span></span> <span data-ttu-id="4390a-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="4390a-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4390a-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="4390a-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4390a-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="4390a-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4390a-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4390a-193">isAssigned</span></span>|<span data-ttu-id="4390a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4390a-194">Boolean</span></span>|<span data-ttu-id="4390a-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="4390a-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4390a-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4390a-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4390a-197">roleScopeTagIds</span></span>|<span data-ttu-id="4390a-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="4390a-198">String collection</span></span>|<span data-ttu-id="4390a-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="4390a-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4390a-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4390a-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="4390a-201">dependentAppCount</span></span>|<span data-ttu-id="4390a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="4390a-202">Int32</span></span>|<span data-ttu-id="4390a-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="4390a-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4390a-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4390a-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="4390a-205">appAvailability</span></span>|[<span data-ttu-id="4390a-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="4390a-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="4390a-207">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="4390a-207">The Application's availability.</span></span> <span data-ttu-id="4390a-208">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="4390a-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="4390a-209">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="4390a-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="4390a-210">version</span><span class="sxs-lookup"><span data-stu-id="4390a-210">version</span></span>|<span data-ttu-id="4390a-211">String</span><span class="sxs-lookup"><span data-stu-id="4390a-211">String</span></span>|<span data-ttu-id="4390a-212">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="4390a-212">The Application's version.</span></span> <span data-ttu-id="4390a-213">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="4390a-214">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="4390a-214">committedContentVersion</span></span>|<span data-ttu-id="4390a-215">String</span><span class="sxs-lookup"><span data-stu-id="4390a-215">String</span></span>|<span data-ttu-id="4390a-216">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="4390a-216">The internal committed content version.</span></span> <span data-ttu-id="4390a-217">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4390a-218">fileName</span><span class="sxs-lookup"><span data-stu-id="4390a-218">fileName</span></span>|<span data-ttu-id="4390a-219">String</span><span class="sxs-lookup"><span data-stu-id="4390a-219">String</span></span>|<span data-ttu-id="4390a-220">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="4390a-220">The name of the main Lob application file.</span></span> <span data-ttu-id="4390a-221">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4390a-222">size</span><span class="sxs-lookup"><span data-stu-id="4390a-222">size</span></span>|<span data-ttu-id="4390a-223">Int64</span><span class="sxs-lookup"><span data-stu-id="4390a-223">Int64</span></span>|<span data-ttu-id="4390a-224">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="4390a-224">The total size, including all uploaded files.</span></span> <span data-ttu-id="4390a-225">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4390a-225">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4390a-226">packageId</span><span class="sxs-lookup"><span data-stu-id="4390a-226">packageId</span></span>|<span data-ttu-id="4390a-227">String</span><span class="sxs-lookup"><span data-stu-id="4390a-227">String</span></span>|<span data-ttu-id="4390a-228">包标识符。</span><span class="sxs-lookup"><span data-stu-id="4390a-228">The package identifier.</span></span>|
|<span data-ttu-id="4390a-229">identityName</span><span class="sxs-lookup"><span data-stu-id="4390a-229">identityName</span></span>|<span data-ttu-id="4390a-230">String</span><span class="sxs-lookup"><span data-stu-id="4390a-230">String</span></span>|<span data-ttu-id="4390a-231">标识名称。</span><span class="sxs-lookup"><span data-stu-id="4390a-231">The Identity Name.</span></span>|
|<span data-ttu-id="4390a-232">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4390a-232">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4390a-233">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4390a-233">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="4390a-234">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="4390a-234">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="4390a-235">versionName</span><span class="sxs-lookup"><span data-stu-id="4390a-235">versionName</span></span>|<span data-ttu-id="4390a-236">String</span><span class="sxs-lookup"><span data-stu-id="4390a-236">String</span></span>|<span data-ttu-id="4390a-237">托管 Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="4390a-237">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4390a-238">versionCode</span><span class="sxs-lookup"><span data-stu-id="4390a-238">versionCode</span></span>|<span data-ttu-id="4390a-239">String</span><span class="sxs-lookup"><span data-stu-id="4390a-239">String</span></span>|<span data-ttu-id="4390a-240">托管 Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="4390a-240">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4390a-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="4390a-241">identityVersion</span></span>|<span data-ttu-id="4390a-242">String</span><span class="sxs-lookup"><span data-stu-id="4390a-242">String</span></span>|<span data-ttu-id="4390a-243">标识版本。</span><span class="sxs-lookup"><span data-stu-id="4390a-243">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="4390a-244">响应</span><span class="sxs-lookup"><span data-stu-id="4390a-244">Response</span></span>
<span data-ttu-id="4390a-245">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4390a-245">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4390a-246">示例</span><span class="sxs-lookup"><span data-stu-id="4390a-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="4390a-247">请求</span><span class="sxs-lookup"><span data-stu-id="4390a-247">Request</span></span>
<span data-ttu-id="4390a-248">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4390a-248">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1491

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
  "dependentAppCount": 1,
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

### <a name="response"></a><span data-ttu-id="4390a-249">响应</span><span class="sxs-lookup"><span data-stu-id="4390a-249">Response</span></span>
<span data-ttu-id="4390a-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4390a-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1663

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
  "dependentAppCount": 1,
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





