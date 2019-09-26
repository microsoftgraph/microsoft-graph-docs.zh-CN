---
title: 创建 managedAndroidLobApp
description: 创建新的 managedAndroidLobApp 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73a339e35cd721ecfe2643a4894208a5e0d688fe
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37177540"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="4008d-103">创建 managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="4008d-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="4008d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4008d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4008d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4008d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4008d-106">创建新的 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4008d-106">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4008d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4008d-107">Prerequisites</span></span>
<span data-ttu-id="4008d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4008d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4008d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4008d-110">Permission type</span></span>|<span data-ttu-id="4008d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4008d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4008d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4008d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4008d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4008d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4008d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4008d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4008d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4008d-115">Not supported.</span></span>|
|<span data-ttu-id="4008d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4008d-116">Application</span></span>|<span data-ttu-id="4008d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4008d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4008d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4008d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4008d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4008d-119">Request headers</span></span>
|<span data-ttu-id="4008d-120">标头</span><span class="sxs-lookup"><span data-stu-id="4008d-120">Header</span></span>|<span data-ttu-id="4008d-121">值</span><span class="sxs-lookup"><span data-stu-id="4008d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4008d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4008d-122">Authorization</span></span>|<span data-ttu-id="4008d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4008d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4008d-124">接受</span><span class="sxs-lookup"><span data-stu-id="4008d-124">Accept</span></span>|<span data-ttu-id="4008d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4008d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4008d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4008d-126">Request body</span></span>
<span data-ttu-id="4008d-127">在请求正文中，提供 managedAndroidLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4008d-127">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="4008d-128">下表显示了创建 managedAndroidLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4008d-128">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="4008d-129">属性</span><span class="sxs-lookup"><span data-stu-id="4008d-129">Property</span></span>|<span data-ttu-id="4008d-130">类型</span><span class="sxs-lookup"><span data-stu-id="4008d-130">Type</span></span>|<span data-ttu-id="4008d-131">说明</span><span class="sxs-lookup"><span data-stu-id="4008d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4008d-132">id</span><span class="sxs-lookup"><span data-stu-id="4008d-132">id</span></span>|<span data-ttu-id="4008d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4008d-133">String</span></span>|<span data-ttu-id="4008d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4008d-134">Key of the entity.</span></span> <span data-ttu-id="4008d-135">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4008d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4008d-136">displayName</span></span>|<span data-ttu-id="4008d-137">String</span><span class="sxs-lookup"><span data-stu-id="4008d-137">String</span></span>|<span data-ttu-id="4008d-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="4008d-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4008d-139">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4008d-140">说明</span><span class="sxs-lookup"><span data-stu-id="4008d-140">description</span></span>|<span data-ttu-id="4008d-141">字符串</span><span class="sxs-lookup"><span data-stu-id="4008d-141">String</span></span>|<span data-ttu-id="4008d-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="4008d-142">The description of the app.</span></span> <span data-ttu-id="4008d-143">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4008d-144">publisher</span><span class="sxs-lookup"><span data-stu-id="4008d-144">publisher</span></span>|<span data-ttu-id="4008d-145">String</span><span class="sxs-lookup"><span data-stu-id="4008d-145">String</span></span>|<span data-ttu-id="4008d-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="4008d-146">The publisher of the app.</span></span> <span data-ttu-id="4008d-147">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4008d-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4008d-148">largeIcon</span></span>|[<span data-ttu-id="4008d-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4008d-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4008d-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="4008d-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4008d-151">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4008d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4008d-152">createdDateTime</span></span>|<span data-ttu-id="4008d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4008d-153">DateTimeOffset</span></span>|<span data-ttu-id="4008d-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4008d-154">The date and time the app was created.</span></span> <span data-ttu-id="4008d-155">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4008d-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4008d-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4008d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4008d-157">DateTimeOffset</span></span>|<span data-ttu-id="4008d-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4008d-158">The date and time the app was last modified.</span></span> <span data-ttu-id="4008d-159">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4008d-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4008d-160">isFeatured</span></span>|<span data-ttu-id="4008d-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4008d-161">Boolean</span></span>|<span data-ttu-id="4008d-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4008d-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4008d-163">privacyInformationUrl</span></span>|<span data-ttu-id="4008d-164">String</span><span class="sxs-lookup"><span data-stu-id="4008d-164">String</span></span>|<span data-ttu-id="4008d-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="4008d-165">The privacy statement Url.</span></span> <span data-ttu-id="4008d-166">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4008d-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4008d-167">informationUrl</span></span>|<span data-ttu-id="4008d-168">String</span><span class="sxs-lookup"><span data-stu-id="4008d-168">String</span></span>|<span data-ttu-id="4008d-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="4008d-169">The more information Url.</span></span> <span data-ttu-id="4008d-170">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4008d-171">owner</span><span class="sxs-lookup"><span data-stu-id="4008d-171">owner</span></span>|<span data-ttu-id="4008d-172">String</span><span class="sxs-lookup"><span data-stu-id="4008d-172">String</span></span>|<span data-ttu-id="4008d-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="4008d-173">The owner of the app.</span></span> <span data-ttu-id="4008d-174">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4008d-175">developer</span><span class="sxs-lookup"><span data-stu-id="4008d-175">developer</span></span>|<span data-ttu-id="4008d-176">String</span><span class="sxs-lookup"><span data-stu-id="4008d-176">String</span></span>|<span data-ttu-id="4008d-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="4008d-177">The developer of the app.</span></span> <span data-ttu-id="4008d-178">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4008d-179">notes</span><span class="sxs-lookup"><span data-stu-id="4008d-179">notes</span></span>|<span data-ttu-id="4008d-180">String</span><span class="sxs-lookup"><span data-stu-id="4008d-180">String</span></span>|<span data-ttu-id="4008d-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="4008d-181">Notes for the app.</span></span> <span data-ttu-id="4008d-182">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4008d-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="4008d-183">uploadState</span></span>|<span data-ttu-id="4008d-184">Int32</span><span class="sxs-lookup"><span data-stu-id="4008d-184">Int32</span></span>|<span data-ttu-id="4008d-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="4008d-185">The upload state.</span></span> <span data-ttu-id="4008d-186">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4008d-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="4008d-187">publishingState</span></span>|[<span data-ttu-id="4008d-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4008d-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4008d-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="4008d-189">The publishing state for the app.</span></span> <span data-ttu-id="4008d-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="4008d-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4008d-191">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="4008d-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="4008d-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="4008d-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4008d-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4008d-193">isAssigned</span></span>|<span data-ttu-id="4008d-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4008d-194">Boolean</span></span>|<span data-ttu-id="4008d-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="4008d-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4008d-196">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4008d-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4008d-197">roleScopeTagIds</span></span>|<span data-ttu-id="4008d-198">String collection</span><span class="sxs-lookup"><span data-stu-id="4008d-198">String collection</span></span>|<span data-ttu-id="4008d-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="4008d-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4008d-200">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4008d-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="4008d-201">dependentAppCount</span></span>|<span data-ttu-id="4008d-202">Int32</span><span class="sxs-lookup"><span data-stu-id="4008d-202">Int32</span></span>|<span data-ttu-id="4008d-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="4008d-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4008d-204">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4008d-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="4008d-205">appAvailability</span></span>|[<span data-ttu-id="4008d-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="4008d-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="4008d-207">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="4008d-207">The Application's availability.</span></span> <span data-ttu-id="4008d-208">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="4008d-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="4008d-209">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="4008d-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="4008d-210">version</span><span class="sxs-lookup"><span data-stu-id="4008d-210">version</span></span>|<span data-ttu-id="4008d-211">String</span><span class="sxs-lookup"><span data-stu-id="4008d-211">String</span></span>|<span data-ttu-id="4008d-212">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="4008d-212">The Application's version.</span></span> <span data-ttu-id="4008d-213">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="4008d-214">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="4008d-214">committedContentVersion</span></span>|<span data-ttu-id="4008d-215">String</span><span class="sxs-lookup"><span data-stu-id="4008d-215">String</span></span>|<span data-ttu-id="4008d-216">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="4008d-216">The internal committed content version.</span></span> <span data-ttu-id="4008d-217">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4008d-218">fileName</span><span class="sxs-lookup"><span data-stu-id="4008d-218">fileName</span></span>|<span data-ttu-id="4008d-219">String</span><span class="sxs-lookup"><span data-stu-id="4008d-219">String</span></span>|<span data-ttu-id="4008d-220">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="4008d-220">The name of the main Lob application file.</span></span> <span data-ttu-id="4008d-221">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4008d-222">size</span><span class="sxs-lookup"><span data-stu-id="4008d-222">size</span></span>|<span data-ttu-id="4008d-223">Int64</span><span class="sxs-lookup"><span data-stu-id="4008d-223">Int64</span></span>|<span data-ttu-id="4008d-224">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="4008d-224">The total size, including all uploaded files.</span></span> <span data-ttu-id="4008d-225">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4008d-225">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4008d-226">packageId</span><span class="sxs-lookup"><span data-stu-id="4008d-226">packageId</span></span>|<span data-ttu-id="4008d-227">String</span><span class="sxs-lookup"><span data-stu-id="4008d-227">String</span></span>|<span data-ttu-id="4008d-228">包标识符。</span><span class="sxs-lookup"><span data-stu-id="4008d-228">The package identifier.</span></span>|
|<span data-ttu-id="4008d-229">identityName</span><span class="sxs-lookup"><span data-stu-id="4008d-229">identityName</span></span>|<span data-ttu-id="4008d-230">String</span><span class="sxs-lookup"><span data-stu-id="4008d-230">String</span></span>|<span data-ttu-id="4008d-231">标识名称。</span><span class="sxs-lookup"><span data-stu-id="4008d-231">The Identity Name.</span></span>|
|<span data-ttu-id="4008d-232">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4008d-232">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4008d-233">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4008d-233">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="4008d-234">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="4008d-234">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="4008d-235">versionName</span><span class="sxs-lookup"><span data-stu-id="4008d-235">versionName</span></span>|<span data-ttu-id="4008d-236">String</span><span class="sxs-lookup"><span data-stu-id="4008d-236">String</span></span>|<span data-ttu-id="4008d-237">托管 Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="4008d-237">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4008d-238">versionCode</span><span class="sxs-lookup"><span data-stu-id="4008d-238">versionCode</span></span>|<span data-ttu-id="4008d-239">String</span><span class="sxs-lookup"><span data-stu-id="4008d-239">String</span></span>|<span data-ttu-id="4008d-240">托管 Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="4008d-240">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4008d-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="4008d-241">identityVersion</span></span>|<span data-ttu-id="4008d-242">String</span><span class="sxs-lookup"><span data-stu-id="4008d-242">String</span></span>|<span data-ttu-id="4008d-243">标识版本。</span><span class="sxs-lookup"><span data-stu-id="4008d-243">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="4008d-244">响应</span><span class="sxs-lookup"><span data-stu-id="4008d-244">Response</span></span>
<span data-ttu-id="4008d-245">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4008d-245">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4008d-246">示例</span><span class="sxs-lookup"><span data-stu-id="4008d-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="4008d-247">请求</span><span class="sxs-lookup"><span data-stu-id="4008d-247">Request</span></span>
<span data-ttu-id="4008d-248">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4008d-248">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="4008d-249">响应</span><span class="sxs-lookup"><span data-stu-id="4008d-249">Response</span></span>
<span data-ttu-id="4008d-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4008d-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




