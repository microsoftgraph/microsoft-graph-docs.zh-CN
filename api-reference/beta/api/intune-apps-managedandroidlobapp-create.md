---
title: 创建 managedAndroidLobApp
description: 创建新的 managedAndroidLobApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9eb57a81da2aaae1f7c9dae16cd1673eb045fe11
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157349"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="a1155-103">创建 managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="a1155-103">Create managedAndroidLobApp</span></span>

<span data-ttu-id="a1155-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1155-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1155-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a1155-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1155-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1155-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1155-107">创建新的 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1155-107">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1155-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1155-108">Prerequisites</span></span>
<span data-ttu-id="a1155-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1155-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1155-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1155-111">Permission type</span></span>|<span data-ttu-id="a1155-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a1155-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1155-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1155-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1155-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1155-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a1155-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1155-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1155-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1155-116">Not supported.</span></span>|
|<span data-ttu-id="a1155-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1155-117">Application</span></span>|<span data-ttu-id="a1155-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1155-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1155-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1155-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a1155-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1155-120">Request headers</span></span>
|<span data-ttu-id="a1155-121">标头</span><span class="sxs-lookup"><span data-stu-id="a1155-121">Header</span></span>|<span data-ttu-id="a1155-122">值</span><span class="sxs-lookup"><span data-stu-id="a1155-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1155-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1155-123">Authorization</span></span>|<span data-ttu-id="a1155-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1155-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1155-125">接受</span><span class="sxs-lookup"><span data-stu-id="a1155-125">Accept</span></span>|<span data-ttu-id="a1155-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1155-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1155-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1155-127">Request body</span></span>
<span data-ttu-id="a1155-128">在请求正文中，提供 managedAndroidLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1155-128">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="a1155-129">下表显示了创建 managedAndroidLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a1155-129">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="a1155-130">属性</span><span class="sxs-lookup"><span data-stu-id="a1155-130">Property</span></span>|<span data-ttu-id="a1155-131">类型</span><span class="sxs-lookup"><span data-stu-id="a1155-131">Type</span></span>|<span data-ttu-id="a1155-132">说明</span><span class="sxs-lookup"><span data-stu-id="a1155-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1155-133">id</span><span class="sxs-lookup"><span data-stu-id="a1155-133">id</span></span>|<span data-ttu-id="a1155-134">String</span><span class="sxs-lookup"><span data-stu-id="a1155-134">String</span></span>|<span data-ttu-id="a1155-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a1155-135">Key of the entity.</span></span> <span data-ttu-id="a1155-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a1155-137">displayName</span></span>|<span data-ttu-id="a1155-138">String</span><span class="sxs-lookup"><span data-stu-id="a1155-138">String</span></span>|<span data-ttu-id="a1155-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="a1155-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a1155-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-141">说明</span><span class="sxs-lookup"><span data-stu-id="a1155-141">description</span></span>|<span data-ttu-id="a1155-142">String</span><span class="sxs-lookup"><span data-stu-id="a1155-142">String</span></span>|<span data-ttu-id="a1155-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="a1155-143">The description of the app.</span></span> <span data-ttu-id="a1155-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-145">publisher</span><span class="sxs-lookup"><span data-stu-id="a1155-145">publisher</span></span>|<span data-ttu-id="a1155-146">String</span><span class="sxs-lookup"><span data-stu-id="a1155-146">String</span></span>|<span data-ttu-id="a1155-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="a1155-147">The publisher of the app.</span></span> <span data-ttu-id="a1155-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a1155-149">largeIcon</span></span>|[<span data-ttu-id="a1155-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a1155-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a1155-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="a1155-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a1155-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1155-153">createdDateTime</span></span>|<span data-ttu-id="a1155-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1155-154">DateTimeOffset</span></span>|<span data-ttu-id="a1155-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a1155-155">The date and time the app was created.</span></span> <span data-ttu-id="a1155-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1155-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a1155-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1155-158">DateTimeOffset</span></span>|<span data-ttu-id="a1155-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a1155-159">The date and time the app was last modified.</span></span> <span data-ttu-id="a1155-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a1155-161">isFeatured</span></span>|<span data-ttu-id="a1155-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1155-162">Boolean</span></span>|<span data-ttu-id="a1155-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a1155-164">privacyInformationUrl</span></span>|<span data-ttu-id="a1155-165">String</span><span class="sxs-lookup"><span data-stu-id="a1155-165">String</span></span>|<span data-ttu-id="a1155-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="a1155-166">The privacy statement Url.</span></span> <span data-ttu-id="a1155-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a1155-168">informationUrl</span></span>|<span data-ttu-id="a1155-169">String</span><span class="sxs-lookup"><span data-stu-id="a1155-169">String</span></span>|<span data-ttu-id="a1155-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="a1155-170">The more information Url.</span></span> <span data-ttu-id="a1155-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-172">owner</span><span class="sxs-lookup"><span data-stu-id="a1155-172">owner</span></span>|<span data-ttu-id="a1155-173">String</span><span class="sxs-lookup"><span data-stu-id="a1155-173">String</span></span>|<span data-ttu-id="a1155-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="a1155-174">The owner of the app.</span></span> <span data-ttu-id="a1155-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-176">developer</span><span class="sxs-lookup"><span data-stu-id="a1155-176">developer</span></span>|<span data-ttu-id="a1155-177">String</span><span class="sxs-lookup"><span data-stu-id="a1155-177">String</span></span>|<span data-ttu-id="a1155-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="a1155-178">The developer of the app.</span></span> <span data-ttu-id="a1155-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-180">notes</span><span class="sxs-lookup"><span data-stu-id="a1155-180">notes</span></span>|<span data-ttu-id="a1155-181">String</span><span class="sxs-lookup"><span data-stu-id="a1155-181">String</span></span>|<span data-ttu-id="a1155-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="a1155-182">Notes for the app.</span></span> <span data-ttu-id="a1155-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="a1155-184">uploadState</span></span>|<span data-ttu-id="a1155-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a1155-185">Int32</span></span>|<span data-ttu-id="a1155-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="a1155-186">The upload state.</span></span> <span data-ttu-id="a1155-187">可能的值是：0 - `Not Ready` 、 1 - `Ready` 、 2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="a1155-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="a1155-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="a1155-189">publishingState</span></span>|[<span data-ttu-id="a1155-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a1155-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a1155-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="a1155-191">The publishing state for the app.</span></span> <span data-ttu-id="a1155-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="a1155-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a1155-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="a1155-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="a1155-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="a1155-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a1155-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a1155-195">isAssigned</span></span>|<span data-ttu-id="a1155-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1155-196">Boolean</span></span>|<span data-ttu-id="a1155-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="a1155-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a1155-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a1155-199">roleScopeTagIds</span></span>|<span data-ttu-id="a1155-200">字符串集合</span><span class="sxs-lookup"><span data-stu-id="a1155-200">String collection</span></span>|<span data-ttu-id="a1155-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="a1155-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a1155-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="a1155-203">dependentAppCount</span></span>|<span data-ttu-id="a1155-204">Int32</span><span class="sxs-lookup"><span data-stu-id="a1155-204">Int32</span></span>|<span data-ttu-id="a1155-205">子应用具有的依赖关系总数。</span><span class="sxs-lookup"><span data-stu-id="a1155-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="a1155-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="a1155-207">supersedingAppCount</span></span>|<span data-ttu-id="a1155-208">Int32</span><span class="sxs-lookup"><span data-stu-id="a1155-208">Int32</span></span>|<span data-ttu-id="a1155-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="a1155-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="a1155-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="a1155-211">supersededAppCount</span></span>|<span data-ttu-id="a1155-212">Int32</span><span class="sxs-lookup"><span data-stu-id="a1155-212">Int32</span></span>|<span data-ttu-id="a1155-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="a1155-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="a1155-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1155-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="a1155-215">appAvailability</span></span>|[<span data-ttu-id="a1155-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="a1155-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="a1155-217">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="a1155-217">The Application's availability.</span></span> <span data-ttu-id="a1155-218">继承自 [managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="a1155-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="a1155-219">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="a1155-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="a1155-220">version</span><span class="sxs-lookup"><span data-stu-id="a1155-220">version</span></span>|<span data-ttu-id="a1155-221">String</span><span class="sxs-lookup"><span data-stu-id="a1155-221">String</span></span>|<span data-ttu-id="a1155-222">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="a1155-222">The Application's version.</span></span> <span data-ttu-id="a1155-223">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="a1155-224">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="a1155-224">committedContentVersion</span></span>|<span data-ttu-id="a1155-225">String</span><span class="sxs-lookup"><span data-stu-id="a1155-225">String</span></span>|<span data-ttu-id="a1155-226">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="a1155-226">The internal committed content version.</span></span> <span data-ttu-id="a1155-227">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-227">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a1155-228">fileName</span><span class="sxs-lookup"><span data-stu-id="a1155-228">fileName</span></span>|<span data-ttu-id="a1155-229">String</span><span class="sxs-lookup"><span data-stu-id="a1155-229">String</span></span>|<span data-ttu-id="a1155-230">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="a1155-230">The name of the main Lob application file.</span></span> <span data-ttu-id="a1155-231">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-231">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a1155-232">size</span><span class="sxs-lookup"><span data-stu-id="a1155-232">size</span></span>|<span data-ttu-id="a1155-233">Int64</span><span class="sxs-lookup"><span data-stu-id="a1155-233">Int64</span></span>|<span data-ttu-id="a1155-234">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="a1155-234">The total size, including all uploaded files.</span></span> <span data-ttu-id="a1155-235">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1155-235">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a1155-236">packageId</span><span class="sxs-lookup"><span data-stu-id="a1155-236">packageId</span></span>|<span data-ttu-id="a1155-237">String</span><span class="sxs-lookup"><span data-stu-id="a1155-237">String</span></span>|<span data-ttu-id="a1155-238">包标识符。</span><span class="sxs-lookup"><span data-stu-id="a1155-238">The package identifier.</span></span>|
|<span data-ttu-id="a1155-239">identityName</span><span class="sxs-lookup"><span data-stu-id="a1155-239">identityName</span></span>|<span data-ttu-id="a1155-240">String</span><span class="sxs-lookup"><span data-stu-id="a1155-240">String</span></span>|<span data-ttu-id="a1155-241">标识名称。</span><span class="sxs-lookup"><span data-stu-id="a1155-241">The Identity Name.</span></span>|
|<span data-ttu-id="a1155-242">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a1155-242">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a1155-243">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a1155-243">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="a1155-244">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="a1155-244">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="a1155-245">versionName</span><span class="sxs-lookup"><span data-stu-id="a1155-245">versionName</span></span>|<span data-ttu-id="a1155-246">String</span><span class="sxs-lookup"><span data-stu-id="a1155-246">String</span></span>|<span data-ttu-id="a1155-247">托管 Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="a1155-247">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="a1155-248">versionCode</span><span class="sxs-lookup"><span data-stu-id="a1155-248">versionCode</span></span>|<span data-ttu-id="a1155-249">String</span><span class="sxs-lookup"><span data-stu-id="a1155-249">String</span></span>|<span data-ttu-id="a1155-250">托管 Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="a1155-250">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="a1155-251">identityVersion</span><span class="sxs-lookup"><span data-stu-id="a1155-251">identityVersion</span></span>|<span data-ttu-id="a1155-252">String</span><span class="sxs-lookup"><span data-stu-id="a1155-252">String</span></span>|<span data-ttu-id="a1155-253">标识版本。</span><span class="sxs-lookup"><span data-stu-id="a1155-253">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="a1155-254">响应</span><span class="sxs-lookup"><span data-stu-id="a1155-254">Response</span></span>
<span data-ttu-id="a1155-255">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1155-255">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1155-256">示例</span><span class="sxs-lookup"><span data-stu-id="a1155-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1155-257">请求</span><span class="sxs-lookup"><span data-stu-id="a1155-257">Request</span></span>
<span data-ttu-id="a1155-258">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1155-258">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1588

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="a1155-259">响应</span><span class="sxs-lookup"><span data-stu-id="a1155-259">Response</span></span>
<span data-ttu-id="a1155-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1155-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1760

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```




