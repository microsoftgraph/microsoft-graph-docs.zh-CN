---
title: 更新 windowsAppX
description: 更新 windowsAppX 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f763e6a9e89ed701177ccb11dca79825ee4592bf
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157090"
---
# <a name="update-windowsappx"></a><span data-ttu-id="af90f-103">更新 windowsAppX</span><span class="sxs-lookup"><span data-stu-id="af90f-103">Update windowsAppX</span></span>

<span data-ttu-id="af90f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af90f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af90f-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="af90f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af90f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="af90f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af90f-107">更新 [windowsAppX 对象](../resources/intune-apps-windowsappx.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="af90f-107">Update the properties of a [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af90f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="af90f-108">Prerequisites</span></span>
<span data-ttu-id="af90f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="af90f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af90f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="af90f-111">Permission type</span></span>|<span data-ttu-id="af90f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="af90f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af90f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="af90f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af90f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af90f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="af90f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="af90f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af90f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="af90f-116">Not supported.</span></span>|
|<span data-ttu-id="af90f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="af90f-117">Application</span></span>|<span data-ttu-id="af90f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af90f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af90f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="af90f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="af90f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="af90f-120">Request headers</span></span>
|<span data-ttu-id="af90f-121">标头</span><span class="sxs-lookup"><span data-stu-id="af90f-121">Header</span></span>|<span data-ttu-id="af90f-122">值</span><span class="sxs-lookup"><span data-stu-id="af90f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af90f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="af90f-123">Authorization</span></span>|<span data-ttu-id="af90f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="af90f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af90f-125">接受</span><span class="sxs-lookup"><span data-stu-id="af90f-125">Accept</span></span>|<span data-ttu-id="af90f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af90f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af90f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="af90f-127">Request body</span></span>
<span data-ttu-id="af90f-128">在请求正文中，提供 [windowsAppX](../resources/intune-apps-windowsappx.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af90f-128">In the request body, supply a JSON representation for the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

<span data-ttu-id="af90f-129">下表显示创建 [windowsAppX](../resources/intune-apps-windowsappx.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="af90f-129">The following table shows the properties that are required when you create the [windowsAppX](../resources/intune-apps-windowsappx.md).</span></span>

|<span data-ttu-id="af90f-130">属性</span><span class="sxs-lookup"><span data-stu-id="af90f-130">Property</span></span>|<span data-ttu-id="af90f-131">类型</span><span class="sxs-lookup"><span data-stu-id="af90f-131">Type</span></span>|<span data-ttu-id="af90f-132">说明</span><span class="sxs-lookup"><span data-stu-id="af90f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af90f-133">id</span><span class="sxs-lookup"><span data-stu-id="af90f-133">id</span></span>|<span data-ttu-id="af90f-134">String</span><span class="sxs-lookup"><span data-stu-id="af90f-134">String</span></span>|<span data-ttu-id="af90f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="af90f-135">Key of the entity.</span></span> <span data-ttu-id="af90f-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="af90f-137">displayName</span></span>|<span data-ttu-id="af90f-138">String</span><span class="sxs-lookup"><span data-stu-id="af90f-138">String</span></span>|<span data-ttu-id="af90f-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="af90f-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="af90f-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-141">说明</span><span class="sxs-lookup"><span data-stu-id="af90f-141">description</span></span>|<span data-ttu-id="af90f-142">String</span><span class="sxs-lookup"><span data-stu-id="af90f-142">String</span></span>|<span data-ttu-id="af90f-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="af90f-143">The description of the app.</span></span> <span data-ttu-id="af90f-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-145">publisher</span><span class="sxs-lookup"><span data-stu-id="af90f-145">publisher</span></span>|<span data-ttu-id="af90f-146">String</span><span class="sxs-lookup"><span data-stu-id="af90f-146">String</span></span>|<span data-ttu-id="af90f-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="af90f-147">The publisher of the app.</span></span> <span data-ttu-id="af90f-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="af90f-149">largeIcon</span></span>|[<span data-ttu-id="af90f-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="af90f-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="af90f-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="af90f-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="af90f-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af90f-153">createdDateTime</span></span>|<span data-ttu-id="af90f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af90f-154">DateTimeOffset</span></span>|<span data-ttu-id="af90f-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="af90f-155">The date and time the app was created.</span></span> <span data-ttu-id="af90f-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af90f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="af90f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af90f-158">DateTimeOffset</span></span>|<span data-ttu-id="af90f-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="af90f-159">The date and time the app was last modified.</span></span> <span data-ttu-id="af90f-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="af90f-161">isFeatured</span></span>|<span data-ttu-id="af90f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="af90f-162">Boolean</span></span>|<span data-ttu-id="af90f-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="af90f-164">privacyInformationUrl</span></span>|<span data-ttu-id="af90f-165">String</span><span class="sxs-lookup"><span data-stu-id="af90f-165">String</span></span>|<span data-ttu-id="af90f-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="af90f-166">The privacy statement Url.</span></span> <span data-ttu-id="af90f-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="af90f-168">informationUrl</span></span>|<span data-ttu-id="af90f-169">String</span><span class="sxs-lookup"><span data-stu-id="af90f-169">String</span></span>|<span data-ttu-id="af90f-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="af90f-170">The more information Url.</span></span> <span data-ttu-id="af90f-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-172">owner</span><span class="sxs-lookup"><span data-stu-id="af90f-172">owner</span></span>|<span data-ttu-id="af90f-173">String</span><span class="sxs-lookup"><span data-stu-id="af90f-173">String</span></span>|<span data-ttu-id="af90f-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="af90f-174">The owner of the app.</span></span> <span data-ttu-id="af90f-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-176">developer</span><span class="sxs-lookup"><span data-stu-id="af90f-176">developer</span></span>|<span data-ttu-id="af90f-177">String</span><span class="sxs-lookup"><span data-stu-id="af90f-177">String</span></span>|<span data-ttu-id="af90f-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="af90f-178">The developer of the app.</span></span> <span data-ttu-id="af90f-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-180">notes</span><span class="sxs-lookup"><span data-stu-id="af90f-180">notes</span></span>|<span data-ttu-id="af90f-181">String</span><span class="sxs-lookup"><span data-stu-id="af90f-181">String</span></span>|<span data-ttu-id="af90f-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="af90f-182">Notes for the app.</span></span> <span data-ttu-id="af90f-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="af90f-184">uploadState</span></span>|<span data-ttu-id="af90f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="af90f-185">Int32</span></span>|<span data-ttu-id="af90f-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="af90f-186">The upload state.</span></span> <span data-ttu-id="af90f-187">可能的值是：0 - `Not Ready` 、 1 - `Ready` 、 2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="af90f-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="af90f-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="af90f-189">publishingState</span></span>|[<span data-ttu-id="af90f-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="af90f-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="af90f-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="af90f-191">The publishing state for the app.</span></span> <span data-ttu-id="af90f-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="af90f-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="af90f-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="af90f-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="af90f-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="af90f-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="af90f-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="af90f-195">isAssigned</span></span>|<span data-ttu-id="af90f-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="af90f-196">Boolean</span></span>|<span data-ttu-id="af90f-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="af90f-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="af90f-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="af90f-199">roleScopeTagIds</span></span>|<span data-ttu-id="af90f-200">字符串集合</span><span class="sxs-lookup"><span data-stu-id="af90f-200">String collection</span></span>|<span data-ttu-id="af90f-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="af90f-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="af90f-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="af90f-203">dependentAppCount</span></span>|<span data-ttu-id="af90f-204">Int32</span><span class="sxs-lookup"><span data-stu-id="af90f-204">Int32</span></span>|<span data-ttu-id="af90f-205">子应用具有的依赖关系总数。</span><span class="sxs-lookup"><span data-stu-id="af90f-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="af90f-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="af90f-207">supersedingAppCount</span></span>|<span data-ttu-id="af90f-208">Int32</span><span class="sxs-lookup"><span data-stu-id="af90f-208">Int32</span></span>|<span data-ttu-id="af90f-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="af90f-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="af90f-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="af90f-211">supersededAppCount</span></span>|<span data-ttu-id="af90f-212">Int32</span><span class="sxs-lookup"><span data-stu-id="af90f-212">Int32</span></span>|<span data-ttu-id="af90f-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="af90f-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="af90f-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af90f-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="af90f-215">committedContentVersion</span></span>|<span data-ttu-id="af90f-216">String</span><span class="sxs-lookup"><span data-stu-id="af90f-216">String</span></span>|<span data-ttu-id="af90f-217">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="af90f-217">The internal committed content version.</span></span> <span data-ttu-id="af90f-218">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="af90f-219">fileName</span><span class="sxs-lookup"><span data-stu-id="af90f-219">fileName</span></span>|<span data-ttu-id="af90f-220">String</span><span class="sxs-lookup"><span data-stu-id="af90f-220">String</span></span>|<span data-ttu-id="af90f-221">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="af90f-221">The name of the main Lob application file.</span></span> <span data-ttu-id="af90f-222">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="af90f-223">size</span><span class="sxs-lookup"><span data-stu-id="af90f-223">size</span></span>|<span data-ttu-id="af90f-224">Int64</span><span class="sxs-lookup"><span data-stu-id="af90f-224">Int64</span></span>|<span data-ttu-id="af90f-225">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="af90f-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="af90f-226">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="af90f-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="af90f-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="af90f-227">applicableArchitectures</span></span>|[<span data-ttu-id="af90f-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="af90f-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="af90f-229">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="af90f-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="af90f-230">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="af90f-230">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="af90f-231">identityName</span><span class="sxs-lookup"><span data-stu-id="af90f-231">identityName</span></span>|<span data-ttu-id="af90f-232">String</span><span class="sxs-lookup"><span data-stu-id="af90f-232">String</span></span>|<span data-ttu-id="af90f-233">标识名称。</span><span class="sxs-lookup"><span data-stu-id="af90f-233">The Identity Name.</span></span>|
|<span data-ttu-id="af90f-234">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="af90f-234">identityPublisherHash</span></span>|<span data-ttu-id="af90f-235">String</span><span class="sxs-lookup"><span data-stu-id="af90f-235">String</span></span>|<span data-ttu-id="af90f-236">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="af90f-236">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="af90f-237">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="af90f-237">identityResourceIdentifier</span></span>|<span data-ttu-id="af90f-238">String</span><span class="sxs-lookup"><span data-stu-id="af90f-238">String</span></span>|<span data-ttu-id="af90f-239">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="af90f-239">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="af90f-240">isBundle</span><span class="sxs-lookup"><span data-stu-id="af90f-240">isBundle</span></span>|<span data-ttu-id="af90f-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="af90f-241">Boolean</span></span>|<span data-ttu-id="af90f-242">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="af90f-242">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="af90f-243">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="af90f-243">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="af90f-244">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="af90f-244">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="af90f-245">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="af90f-245">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="af90f-246">identityVersion</span><span class="sxs-lookup"><span data-stu-id="af90f-246">identityVersion</span></span>|<span data-ttu-id="af90f-247">String</span><span class="sxs-lookup"><span data-stu-id="af90f-247">String</span></span>|<span data-ttu-id="af90f-248">标识版本。</span><span class="sxs-lookup"><span data-stu-id="af90f-248">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="af90f-249">响应</span><span class="sxs-lookup"><span data-stu-id="af90f-249">Response</span></span>
<span data-ttu-id="af90f-250">如果成功，此方法在响应 `200 OK` 正文中返回响应代码和更新的 [windowsAppX](../resources/intune-apps-windowsappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="af90f-250">If successful, this method returns a `200 OK` response code and an updated [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af90f-251">示例</span><span class="sxs-lookup"><span data-stu-id="af90f-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="af90f-252">请求</span><span class="sxs-lookup"><span data-stu-id="af90f-252">Request</span></span>
<span data-ttu-id="af90f-253">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="af90f-253">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1516

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="af90f-254">响应</span><span class="sxs-lookup"><span data-stu-id="af90f-254">Response</span></span>
<span data-ttu-id="af90f-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="af90f-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1688

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```




