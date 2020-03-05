---
title: 创建 managedAndroidLobApp
description: 创建新的 managedAndroidLobApp 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a3d84f87b9602eb6df917729d1d45c69058419e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451096"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="ac0f8-103">创建 managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="ac0f8-103">Create managedAndroidLobApp</span></span>

<span data-ttu-id="ac0f8-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ac0f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac0f8-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac0f8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac0f8-107">创建新的 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-107">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac0f8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ac0f8-108">Prerequisites</span></span>
<span data-ttu-id="ac0f8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac0f8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac0f8-111">Permission type</span></span>|<span data-ttu-id="ac0f8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ac0f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac0f8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac0f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ac0f8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac0f8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ac0f8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac0f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac0f8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-116">Not supported.</span></span>|
|<span data-ttu-id="ac0f8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac0f8-117">Application</span></span>|<span data-ttu-id="ac0f8-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac0f8-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac0f8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac0f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ac0f8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac0f8-120">Request headers</span></span>
|<span data-ttu-id="ac0f8-121">标头</span><span class="sxs-lookup"><span data-stu-id="ac0f8-121">Header</span></span>|<span data-ttu-id="ac0f8-122">值</span><span class="sxs-lookup"><span data-stu-id="ac0f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac0f8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac0f8-123">Authorization</span></span>|<span data-ttu-id="ac0f8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac0f8-125">接受</span><span class="sxs-lookup"><span data-stu-id="ac0f8-125">Accept</span></span>|<span data-ttu-id="ac0f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac0f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac0f8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac0f8-127">Request body</span></span>
<span data-ttu-id="ac0f8-128">在请求正文中，提供 managedAndroidLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-128">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="ac0f8-129">下表显示了创建 managedAndroidLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-129">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="ac0f8-130">属性</span><span class="sxs-lookup"><span data-stu-id="ac0f8-130">Property</span></span>|<span data-ttu-id="ac0f8-131">类型</span><span class="sxs-lookup"><span data-stu-id="ac0f8-131">Type</span></span>|<span data-ttu-id="ac0f8-132">说明</span><span class="sxs-lookup"><span data-stu-id="ac0f8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac0f8-133">id</span><span class="sxs-lookup"><span data-stu-id="ac0f8-133">id</span></span>|<span data-ttu-id="ac0f8-134">字符串</span><span class="sxs-lookup"><span data-stu-id="ac0f8-134">String</span></span>|<span data-ttu-id="ac0f8-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-135">Key of the entity.</span></span> <span data-ttu-id="ac0f8-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0f8-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ac0f8-137">displayName</span></span>|<span data-ttu-id="ac0f8-138">String</span><span class="sxs-lookup"><span data-stu-id="ac0f8-138">String</span></span>|<span data-ttu-id="ac0f8-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ac0f8-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0f8-141">说明</span><span class="sxs-lookup"><span data-stu-id="ac0f8-141">description</span></span>|<span data-ttu-id="ac0f8-142">字符串</span><span class="sxs-lookup"><span data-stu-id="ac0f8-142">String</span></span>|<span data-ttu-id="ac0f8-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-143">The description of the app.</span></span> <span data-ttu-id="ac0f8-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0f8-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ac0f8-145">publisher</span></span>|<span data-ttu-id="ac0f8-146">String</span><span class="sxs-lookup"><span data-stu-id="ac0f8-146">String</span></span>|<span data-ttu-id="ac0f8-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-147">The publisher of the app.</span></span> <span data-ttu-id="ac0f8-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0f8-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ac0f8-149">largeIcon</span></span>|[<span data-ttu-id="ac0f8-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ac0f8-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ac0f8-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ac0f8-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0f8-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac0f8-153">createdDateTime</span></span>|<span data-ttu-id="ac0f8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac0f8-154">DateTimeOffset</span></span>|<span data-ttu-id="ac0f8-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-155">The date and time the app was created.</span></span> <span data-ttu-id="ac0f8-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0f8-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac0f8-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ac0f8-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac0f8-158">DateTimeOffset</span></span>|<span data-ttu-id="ac0f8-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ac0f8-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0f8-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ac0f8-161">isFeatured</span></span>|<span data-ttu-id="ac0f8-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac0f8-162">Boolean</span></span>|<span data-ttu-id="ac0f8-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0f8-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ac0f8-164">privacyInformationUrl</span></span>|<span data-ttu-id="ac0f8-165">String</span><span class="sxs-lookup"><span data-stu-id="ac0f8-165">String</span></span>|<span data-ttu-id="ac0f8-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-166">The privacy statement Url.</span></span> <span data-ttu-id="ac0f8-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0f8-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ac0f8-168">informationUrl</span></span>|<span data-ttu-id="ac0f8-169">String</span><span class="sxs-lookup"><span data-stu-id="ac0f8-169">String</span></span>|<span data-ttu-id="ac0f8-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-170">The more information Url.</span></span> <span data-ttu-id="ac0f8-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0f8-172">owner</span><span class="sxs-lookup"><span data-stu-id="ac0f8-172">owner</span></span>|<span data-ttu-id="ac0f8-173">String</span><span class="sxs-lookup"><span data-stu-id="ac0f8-173">String</span></span>|<span data-ttu-id="ac0f8-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-174">The owner of the app.</span></span> <span data-ttu-id="ac0f8-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0f8-176">developer</span><span class="sxs-lookup"><span data-stu-id="ac0f8-176">developer</span></span>|<span data-ttu-id="ac0f8-177">String</span><span class="sxs-lookup"><span data-stu-id="ac0f8-177">String</span></span>|<span data-ttu-id="ac0f8-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-178">The developer of the app.</span></span> <span data-ttu-id="ac0f8-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0f8-180">notes</span><span class="sxs-lookup"><span data-stu-id="ac0f8-180">notes</span></span>|<span data-ttu-id="ac0f8-181">String</span><span class="sxs-lookup"><span data-stu-id="ac0f8-181">String</span></span>|<span data-ttu-id="ac0f8-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-182">Notes for the app.</span></span> <span data-ttu-id="ac0f8-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0f8-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ac0f8-184">uploadState</span></span>|<span data-ttu-id="ac0f8-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ac0f8-185">Int32</span></span>|<span data-ttu-id="ac0f8-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-186">The upload state.</span></span> <span data-ttu-id="ac0f8-187">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0f8-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="ac0f8-188">publishingState</span></span>|[<span data-ttu-id="ac0f8-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ac0f8-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ac0f8-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-190">The publishing state for the app.</span></span> <span data-ttu-id="ac0f8-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ac0f8-192">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ac0f8-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ac0f8-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ac0f8-194">isAssigned</span></span>|<span data-ttu-id="ac0f8-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac0f8-195">Boolean</span></span>|<span data-ttu-id="ac0f8-196">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ac0f8-197">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0f8-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ac0f8-198">roleScopeTagIds</span></span>|<span data-ttu-id="ac0f8-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="ac0f8-199">String collection</span></span>|<span data-ttu-id="ac0f8-200">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ac0f8-201">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0f8-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="ac0f8-202">dependentAppCount</span></span>|<span data-ttu-id="ac0f8-203">Int32</span><span class="sxs-lookup"><span data-stu-id="ac0f8-203">Int32</span></span>|<span data-ttu-id="ac0f8-204">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ac0f8-205">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0f8-206">appAvailability</span><span class="sxs-lookup"><span data-stu-id="ac0f8-206">appAvailability</span></span>|[<span data-ttu-id="ac0f8-207">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="ac0f8-207">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="ac0f8-208">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-208">The Application's availability.</span></span> <span data-ttu-id="ac0f8-209">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="ac0f8-210">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-210">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="ac0f8-211">version</span><span class="sxs-lookup"><span data-stu-id="ac0f8-211">version</span></span>|<span data-ttu-id="ac0f8-212">String</span><span class="sxs-lookup"><span data-stu-id="ac0f8-212">String</span></span>|<span data-ttu-id="ac0f8-213">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-213">The Application's version.</span></span> <span data-ttu-id="ac0f8-214">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-214">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="ac0f8-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ac0f8-215">committedContentVersion</span></span>|<span data-ttu-id="ac0f8-216">String</span><span class="sxs-lookup"><span data-stu-id="ac0f8-216">String</span></span>|<span data-ttu-id="ac0f8-217">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-217">The internal committed content version.</span></span> <span data-ttu-id="ac0f8-218">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-218">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ac0f8-219">fileName</span><span class="sxs-lookup"><span data-stu-id="ac0f8-219">fileName</span></span>|<span data-ttu-id="ac0f8-220">String</span><span class="sxs-lookup"><span data-stu-id="ac0f8-220">String</span></span>|<span data-ttu-id="ac0f8-221">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-221">The name of the main Lob application file.</span></span> <span data-ttu-id="ac0f8-222">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-222">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ac0f8-223">size</span><span class="sxs-lookup"><span data-stu-id="ac0f8-223">size</span></span>|<span data-ttu-id="ac0f8-224">Int64</span><span class="sxs-lookup"><span data-stu-id="ac0f8-224">Int64</span></span>|<span data-ttu-id="ac0f8-225">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="ac0f8-226">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f8-226">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ac0f8-227">packageId</span><span class="sxs-lookup"><span data-stu-id="ac0f8-227">packageId</span></span>|<span data-ttu-id="ac0f8-228">String</span><span class="sxs-lookup"><span data-stu-id="ac0f8-228">String</span></span>|<span data-ttu-id="ac0f8-229">包标识符。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-229">The package identifier.</span></span>|
|<span data-ttu-id="ac0f8-230">identityName</span><span class="sxs-lookup"><span data-stu-id="ac0f8-230">identityName</span></span>|<span data-ttu-id="ac0f8-231">String</span><span class="sxs-lookup"><span data-stu-id="ac0f8-231">String</span></span>|<span data-ttu-id="ac0f8-232">标识名称。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-232">The Identity Name.</span></span>|
|<span data-ttu-id="ac0f8-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ac0f8-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ac0f8-234">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ac0f8-234">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="ac0f8-235">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ac0f8-236">versionName</span><span class="sxs-lookup"><span data-stu-id="ac0f8-236">versionName</span></span>|<span data-ttu-id="ac0f8-237">String</span><span class="sxs-lookup"><span data-stu-id="ac0f8-237">String</span></span>|<span data-ttu-id="ac0f8-238">托管 Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-238">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ac0f8-239">versionCode</span><span class="sxs-lookup"><span data-stu-id="ac0f8-239">versionCode</span></span>|<span data-ttu-id="ac0f8-240">String</span><span class="sxs-lookup"><span data-stu-id="ac0f8-240">String</span></span>|<span data-ttu-id="ac0f8-241">托管 Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-241">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ac0f8-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ac0f8-242">identityVersion</span></span>|<span data-ttu-id="ac0f8-243">String</span><span class="sxs-lookup"><span data-stu-id="ac0f8-243">String</span></span>|<span data-ttu-id="ac0f8-244">标识版本。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-244">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ac0f8-245">响应</span><span class="sxs-lookup"><span data-stu-id="ac0f8-245">Response</span></span>
<span data-ttu-id="ac0f8-246">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-246">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac0f8-247">示例</span><span class="sxs-lookup"><span data-stu-id="ac0f8-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac0f8-248">请求</span><span class="sxs-lookup"><span data-stu-id="ac0f8-248">Request</span></span>
<span data-ttu-id="ac0f8-249">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-249">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ac0f8-250">响应</span><span class="sxs-lookup"><span data-stu-id="ac0f8-250">Response</span></span>
<span data-ttu-id="ac0f8-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ac0f8-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





