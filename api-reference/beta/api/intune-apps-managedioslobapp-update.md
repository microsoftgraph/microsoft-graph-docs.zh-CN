---
title: 更新 managedIOSLobApp
description: 更新 managedIOSLobApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab5d49e4116dbf6660079e6a2b278b9a2a5890ff
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168423"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="51922-103">更新 managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="51922-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="51922-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="51922-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51922-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51922-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51922-106">更新 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="51922-106">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51922-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="51922-107">Prerequisites</span></span>
<span data-ttu-id="51922-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="51922-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="51922-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="51922-110">Permission type</span></span>|<span data-ttu-id="51922-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="51922-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51922-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51922-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51922-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51922-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="51922-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51922-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51922-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="51922-115">Not supported.</span></span>|
|<span data-ttu-id="51922-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="51922-116">Application</span></span>|<span data-ttu-id="51922-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="51922-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51922-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51922-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="51922-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="51922-119">Request headers</span></span>
|<span data-ttu-id="51922-120">标头</span><span class="sxs-lookup"><span data-stu-id="51922-120">Header</span></span>|<span data-ttu-id="51922-121">值</span><span class="sxs-lookup"><span data-stu-id="51922-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51922-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="51922-122">Authorization</span></span>|<span data-ttu-id="51922-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="51922-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51922-124">Accept</span><span class="sxs-lookup"><span data-stu-id="51922-124">Accept</span></span>|<span data-ttu-id="51922-125">application/json</span><span class="sxs-lookup"><span data-stu-id="51922-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51922-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="51922-126">Request body</span></span>
<span data-ttu-id="51922-127">在请求正文中，提供 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51922-127">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="51922-128">下表显示创建 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="51922-128">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="51922-129">属性</span><span class="sxs-lookup"><span data-stu-id="51922-129">Property</span></span>|<span data-ttu-id="51922-130">类型</span><span class="sxs-lookup"><span data-stu-id="51922-130">Type</span></span>|<span data-ttu-id="51922-131">说明</span><span class="sxs-lookup"><span data-stu-id="51922-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51922-132">id</span><span class="sxs-lookup"><span data-stu-id="51922-132">id</span></span>|<span data-ttu-id="51922-133">字串符号</span><span class="sxs-lookup"><span data-stu-id="51922-133">String</span></span>|<span data-ttu-id="51922-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="51922-134">Key of the entity.</span></span> <span data-ttu-id="51922-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51922-136">displayName</span><span class="sxs-lookup"><span data-stu-id="51922-136">displayName</span></span>|<span data-ttu-id="51922-137">字符串</span><span class="sxs-lookup"><span data-stu-id="51922-137">String</span></span>|<span data-ttu-id="51922-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="51922-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="51922-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51922-140">description</span><span class="sxs-lookup"><span data-stu-id="51922-140">description</span></span>|<span data-ttu-id="51922-141">字符串</span><span class="sxs-lookup"><span data-stu-id="51922-141">String</span></span>|<span data-ttu-id="51922-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="51922-142">The description of the app.</span></span> <span data-ttu-id="51922-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51922-144">publisher</span><span class="sxs-lookup"><span data-stu-id="51922-144">publisher</span></span>|<span data-ttu-id="51922-145">字符串</span><span class="sxs-lookup"><span data-stu-id="51922-145">String</span></span>|<span data-ttu-id="51922-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="51922-146">The publisher of the app.</span></span> <span data-ttu-id="51922-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51922-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="51922-148">largeIcon</span></span>|[<span data-ttu-id="51922-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="51922-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="51922-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="51922-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="51922-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51922-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51922-152">createdDateTime</span></span>|<span data-ttu-id="51922-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51922-153">DateTimeOffset</span></span>|<span data-ttu-id="51922-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="51922-154">The date and time the app was created.</span></span> <span data-ttu-id="51922-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51922-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51922-156">lastModifiedDateTime</span></span>|<span data-ttu-id="51922-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51922-157">DateTimeOffset</span></span>|<span data-ttu-id="51922-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="51922-158">The date and time the app was last modified.</span></span> <span data-ttu-id="51922-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51922-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="51922-160">isFeatured</span></span>|<span data-ttu-id="51922-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="51922-161">Boolean</span></span>|<span data-ttu-id="51922-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51922-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="51922-163">privacyInformationUrl</span></span>|<span data-ttu-id="51922-164">字符串</span><span class="sxs-lookup"><span data-stu-id="51922-164">String</span></span>|<span data-ttu-id="51922-165">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="51922-165">The privacy statement Url.</span></span> <span data-ttu-id="51922-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51922-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="51922-167">informationUrl</span></span>|<span data-ttu-id="51922-168">字符串</span><span class="sxs-lookup"><span data-stu-id="51922-168">String</span></span>|<span data-ttu-id="51922-169">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="51922-169">The more information Url.</span></span> <span data-ttu-id="51922-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51922-171">owner</span><span class="sxs-lookup"><span data-stu-id="51922-171">owner</span></span>|<span data-ttu-id="51922-172">String</span><span class="sxs-lookup"><span data-stu-id="51922-172">String</span></span>|<span data-ttu-id="51922-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="51922-173">The owner of the app.</span></span> <span data-ttu-id="51922-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51922-175">developer</span><span class="sxs-lookup"><span data-stu-id="51922-175">developer</span></span>|<span data-ttu-id="51922-176">String</span><span class="sxs-lookup"><span data-stu-id="51922-176">String</span></span>|<span data-ttu-id="51922-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="51922-177">The developer of the app.</span></span> <span data-ttu-id="51922-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51922-179">notes</span><span class="sxs-lookup"><span data-stu-id="51922-179">notes</span></span>|<span data-ttu-id="51922-180">String</span><span class="sxs-lookup"><span data-stu-id="51922-180">String</span></span>|<span data-ttu-id="51922-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="51922-181">Notes for the app.</span></span> <span data-ttu-id="51922-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51922-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="51922-183">uploadState</span></span>|<span data-ttu-id="51922-184">Int32</span><span class="sxs-lookup"><span data-stu-id="51922-184">Int32</span></span>|<span data-ttu-id="51922-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="51922-185">The upload state.</span></span> <span data-ttu-id="51922-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51922-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="51922-187">publishingState</span></span>|[<span data-ttu-id="51922-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="51922-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="51922-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="51922-189">The publishing state for the app.</span></span> <span data-ttu-id="51922-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="51922-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="51922-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="51922-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="51922-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="51922-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="51922-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="51922-193">isAssigned</span></span>|<span data-ttu-id="51922-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="51922-194">Boolean</span></span>|<span data-ttu-id="51922-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="51922-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="51922-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51922-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="51922-197">roleScopeTagIds</span></span>|<span data-ttu-id="51922-198">String collection</span><span class="sxs-lookup"><span data-stu-id="51922-198">String collection</span></span>|<span data-ttu-id="51922-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="51922-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="51922-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51922-201">appAvailability</span><span class="sxs-lookup"><span data-stu-id="51922-201">appAvailability</span></span>|[<span data-ttu-id="51922-202">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="51922-202">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="51922-203">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="51922-203">The Application's availability.</span></span> <span data-ttu-id="51922-204">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="51922-204">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="51922-205">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="51922-205">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="51922-206">version</span><span class="sxs-lookup"><span data-stu-id="51922-206">version</span></span>|<span data-ttu-id="51922-207">字符串</span><span class="sxs-lookup"><span data-stu-id="51922-207">String</span></span>|<span data-ttu-id="51922-208">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="51922-208">The Application's version.</span></span> <span data-ttu-id="51922-209">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="51922-210">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="51922-210">committedContentVersion</span></span>|<span data-ttu-id="51922-211">字符串</span><span class="sxs-lookup"><span data-stu-id="51922-211">String</span></span>|<span data-ttu-id="51922-212">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="51922-212">The internal committed content version.</span></span> <span data-ttu-id="51922-213">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-213">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="51922-214">fileName</span><span class="sxs-lookup"><span data-stu-id="51922-214">fileName</span></span>|<span data-ttu-id="51922-215">字符串</span><span class="sxs-lookup"><span data-stu-id="51922-215">String</span></span>|<span data-ttu-id="51922-216">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="51922-216">The name of the main Lob application file.</span></span> <span data-ttu-id="51922-217">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="51922-218">size</span><span class="sxs-lookup"><span data-stu-id="51922-218">size</span></span>|<span data-ttu-id="51922-219">Int64</span><span class="sxs-lookup"><span data-stu-id="51922-219">Int64</span></span>|<span data-ttu-id="51922-220">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="51922-220">The total size, including all uploaded files.</span></span> <span data-ttu-id="51922-221">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="51922-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="51922-222">bundleId</span><span class="sxs-lookup"><span data-stu-id="51922-222">bundleId</span></span>|<span data-ttu-id="51922-223">字符串</span><span class="sxs-lookup"><span data-stu-id="51922-223">String</span></span>|<span data-ttu-id="51922-224">标识名称。</span><span class="sxs-lookup"><span data-stu-id="51922-224">The Identity Name.</span></span>|
|<span data-ttu-id="51922-225">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="51922-225">applicableDeviceType</span></span>|[<span data-ttu-id="51922-226">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="51922-226">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="51922-227">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="51922-227">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="51922-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="51922-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="51922-229">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="51922-229">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="51922-230">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="51922-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="51922-231">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="51922-231">expirationDateTime</span></span>|<span data-ttu-id="51922-232">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51922-232">DateTimeOffset</span></span>|<span data-ttu-id="51922-233">过期时间。</span><span class="sxs-lookup"><span data-stu-id="51922-233">The expiration time.</span></span>|
|<span data-ttu-id="51922-234">versionNumber</span><span class="sxs-lookup"><span data-stu-id="51922-234">versionNumber</span></span>|<span data-ttu-id="51922-235">String</span><span class="sxs-lookup"><span data-stu-id="51922-235">String</span></span>|<span data-ttu-id="51922-236">托管 iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="51922-236">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="51922-237">buildNumber</span><span class="sxs-lookup"><span data-stu-id="51922-237">buildNumber</span></span>|<span data-ttu-id="51922-238">字符串</span><span class="sxs-lookup"><span data-stu-id="51922-238">String</span></span>|<span data-ttu-id="51922-239">托管 iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="51922-239">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="51922-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="51922-240">identityVersion</span></span>|<span data-ttu-id="51922-241">String</span><span class="sxs-lookup"><span data-stu-id="51922-241">String</span></span>|<span data-ttu-id="51922-242">标识版本。</span><span class="sxs-lookup"><span data-stu-id="51922-242">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="51922-243">响应</span><span class="sxs-lookup"><span data-stu-id="51922-243">Response</span></span>
<span data-ttu-id="51922-244">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51922-244">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51922-245">示例</span><span class="sxs-lookup"><span data-stu-id="51922-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="51922-246">请求</span><span class="sxs-lookup"><span data-stu-id="51922-246">Request</span></span>
<span data-ttu-id="51922-247">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="51922-247">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1442

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
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="51922-248">响应</span><span class="sxs-lookup"><span data-stu-id="51922-248">Response</span></span>
<span data-ttu-id="51922-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="51922-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1614

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
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```




