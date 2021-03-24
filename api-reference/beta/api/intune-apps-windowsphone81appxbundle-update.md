---
title: 更新 windowsPhone81AppXBundle
description: 更新 windowsPhone81AppXBundle 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 52605849fdb65d08f3cc6a971f480ff05b922c9e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127030"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="56bf1-103">更新 windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="56bf1-103">Update windowsPhone81AppXBundle</span></span>

<span data-ttu-id="56bf1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56bf1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56bf1-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="56bf1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56bf1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56bf1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56bf1-107">更新 [windowsPhone81AppXBundle 对象](../resources/intune-apps-windowsphone81appxbundle.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="56bf1-107">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56bf1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="56bf1-108">Prerequisites</span></span>
<span data-ttu-id="56bf1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56bf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56bf1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="56bf1-111">Permission type</span></span>|<span data-ttu-id="56bf1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56bf1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56bf1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56bf1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56bf1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56bf1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="56bf1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56bf1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56bf1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="56bf1-116">Not supported.</span></span>|
|<span data-ttu-id="56bf1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="56bf1-117">Application</span></span>|<span data-ttu-id="56bf1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56bf1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56bf1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56bf1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="56bf1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="56bf1-120">Request headers</span></span>
|<span data-ttu-id="56bf1-121">标头</span><span class="sxs-lookup"><span data-stu-id="56bf1-121">Header</span></span>|<span data-ttu-id="56bf1-122">值</span><span class="sxs-lookup"><span data-stu-id="56bf1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56bf1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="56bf1-123">Authorization</span></span>|<span data-ttu-id="56bf1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="56bf1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56bf1-125">接受</span><span class="sxs-lookup"><span data-stu-id="56bf1-125">Accept</span></span>|<span data-ttu-id="56bf1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56bf1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56bf1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="56bf1-127">Request body</span></span>
<span data-ttu-id="56bf1-128">在请求正文中，提供 [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56bf1-128">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="56bf1-129">下表显示创建 [windowsPhone81AppXBundle 时所需的属性](../resources/intune-apps-windowsphone81appxbundle.md)。</span><span class="sxs-lookup"><span data-stu-id="56bf1-129">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="56bf1-130">属性</span><span class="sxs-lookup"><span data-stu-id="56bf1-130">Property</span></span>|<span data-ttu-id="56bf1-131">类型</span><span class="sxs-lookup"><span data-stu-id="56bf1-131">Type</span></span>|<span data-ttu-id="56bf1-132">说明</span><span class="sxs-lookup"><span data-stu-id="56bf1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56bf1-133">id</span><span class="sxs-lookup"><span data-stu-id="56bf1-133">id</span></span>|<span data-ttu-id="56bf1-134">String</span><span class="sxs-lookup"><span data-stu-id="56bf1-134">String</span></span>|<span data-ttu-id="56bf1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="56bf1-135">Key of the entity.</span></span> <span data-ttu-id="56bf1-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-137">displayName</span><span class="sxs-lookup"><span data-stu-id="56bf1-137">displayName</span></span>|<span data-ttu-id="56bf1-138">String</span><span class="sxs-lookup"><span data-stu-id="56bf1-138">String</span></span>|<span data-ttu-id="56bf1-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="56bf1-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="56bf1-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-141">说明</span><span class="sxs-lookup"><span data-stu-id="56bf1-141">description</span></span>|<span data-ttu-id="56bf1-142">String</span><span class="sxs-lookup"><span data-stu-id="56bf1-142">String</span></span>|<span data-ttu-id="56bf1-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="56bf1-143">The description of the app.</span></span> <span data-ttu-id="56bf1-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-145">publisher</span><span class="sxs-lookup"><span data-stu-id="56bf1-145">publisher</span></span>|<span data-ttu-id="56bf1-146">String</span><span class="sxs-lookup"><span data-stu-id="56bf1-146">String</span></span>|<span data-ttu-id="56bf1-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="56bf1-147">The publisher of the app.</span></span> <span data-ttu-id="56bf1-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="56bf1-149">largeIcon</span></span>|[<span data-ttu-id="56bf1-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="56bf1-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="56bf1-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="56bf1-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="56bf1-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56bf1-153">createdDateTime</span></span>|<span data-ttu-id="56bf1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56bf1-154">DateTimeOffset</span></span>|<span data-ttu-id="56bf1-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="56bf1-155">The date and time the app was created.</span></span> <span data-ttu-id="56bf1-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56bf1-157">lastModifiedDateTime</span></span>|<span data-ttu-id="56bf1-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56bf1-158">DateTimeOffset</span></span>|<span data-ttu-id="56bf1-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="56bf1-159">The date and time the app was last modified.</span></span> <span data-ttu-id="56bf1-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="56bf1-161">isFeatured</span></span>|<span data-ttu-id="56bf1-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="56bf1-162">Boolean</span></span>|<span data-ttu-id="56bf1-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="56bf1-164">privacyInformationUrl</span></span>|<span data-ttu-id="56bf1-165">String</span><span class="sxs-lookup"><span data-stu-id="56bf1-165">String</span></span>|<span data-ttu-id="56bf1-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="56bf1-166">The privacy statement Url.</span></span> <span data-ttu-id="56bf1-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="56bf1-168">informationUrl</span></span>|<span data-ttu-id="56bf1-169">String</span><span class="sxs-lookup"><span data-stu-id="56bf1-169">String</span></span>|<span data-ttu-id="56bf1-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="56bf1-170">The more information Url.</span></span> <span data-ttu-id="56bf1-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-172">owner</span><span class="sxs-lookup"><span data-stu-id="56bf1-172">owner</span></span>|<span data-ttu-id="56bf1-173">String</span><span class="sxs-lookup"><span data-stu-id="56bf1-173">String</span></span>|<span data-ttu-id="56bf1-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="56bf1-174">The owner of the app.</span></span> <span data-ttu-id="56bf1-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-176">developer</span><span class="sxs-lookup"><span data-stu-id="56bf1-176">developer</span></span>|<span data-ttu-id="56bf1-177">String</span><span class="sxs-lookup"><span data-stu-id="56bf1-177">String</span></span>|<span data-ttu-id="56bf1-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="56bf1-178">The developer of the app.</span></span> <span data-ttu-id="56bf1-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-180">notes</span><span class="sxs-lookup"><span data-stu-id="56bf1-180">notes</span></span>|<span data-ttu-id="56bf1-181">String</span><span class="sxs-lookup"><span data-stu-id="56bf1-181">String</span></span>|<span data-ttu-id="56bf1-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="56bf1-182">Notes for the app.</span></span> <span data-ttu-id="56bf1-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="56bf1-184">uploadState</span></span>|<span data-ttu-id="56bf1-185">Int32</span><span class="sxs-lookup"><span data-stu-id="56bf1-185">Int32</span></span>|<span data-ttu-id="56bf1-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="56bf1-186">The upload state.</span></span> <span data-ttu-id="56bf1-187">可能的值是：0 - `Not Ready` 、1 - `Ready` 、2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="56bf1-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="56bf1-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="56bf1-189">publishingState</span></span>|[<span data-ttu-id="56bf1-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="56bf1-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="56bf1-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="56bf1-191">The publishing state for the app.</span></span> <span data-ttu-id="56bf1-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="56bf1-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="56bf1-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="56bf1-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="56bf1-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="56bf1-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="56bf1-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="56bf1-195">isAssigned</span></span>|<span data-ttu-id="56bf1-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="56bf1-196">Boolean</span></span>|<span data-ttu-id="56bf1-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="56bf1-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="56bf1-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="56bf1-199">roleScopeTagIds</span></span>|<span data-ttu-id="56bf1-200">String collection</span><span class="sxs-lookup"><span data-stu-id="56bf1-200">String collection</span></span>|<span data-ttu-id="56bf1-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="56bf1-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="56bf1-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="56bf1-203">dependentAppCount</span></span>|<span data-ttu-id="56bf1-204">Int32</span><span class="sxs-lookup"><span data-stu-id="56bf1-204">Int32</span></span>|<span data-ttu-id="56bf1-205">子应用具有的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="56bf1-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="56bf1-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="56bf1-207">supersedingAppCount</span></span>|<span data-ttu-id="56bf1-208">Int32</span><span class="sxs-lookup"><span data-stu-id="56bf1-208">Int32</span></span>|<span data-ttu-id="56bf1-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="56bf1-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="56bf1-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="56bf1-211">supersededAppCount</span></span>|<span data-ttu-id="56bf1-212">Int32</span><span class="sxs-lookup"><span data-stu-id="56bf1-212">Int32</span></span>|<span data-ttu-id="56bf1-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="56bf1-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="56bf1-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bf1-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="56bf1-215">committedContentVersion</span></span>|<span data-ttu-id="56bf1-216">String</span><span class="sxs-lookup"><span data-stu-id="56bf1-216">String</span></span>|<span data-ttu-id="56bf1-217">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="56bf1-217">The internal committed content version.</span></span> <span data-ttu-id="56bf1-218">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="56bf1-219">fileName</span><span class="sxs-lookup"><span data-stu-id="56bf1-219">fileName</span></span>|<span data-ttu-id="56bf1-220">String</span><span class="sxs-lookup"><span data-stu-id="56bf1-220">String</span></span>|<span data-ttu-id="56bf1-221">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="56bf1-221">The name of the main Lob application file.</span></span> <span data-ttu-id="56bf1-222">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="56bf1-223">size</span><span class="sxs-lookup"><span data-stu-id="56bf1-223">size</span></span>|<span data-ttu-id="56bf1-224">Int64</span><span class="sxs-lookup"><span data-stu-id="56bf1-224">Int64</span></span>|<span data-ttu-id="56bf1-225">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="56bf1-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="56bf1-226">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="56bf1-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="56bf1-227">applicableArchitectures</span></span>|[<span data-ttu-id="56bf1-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="56bf1-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="56bf1-229">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="56bf1-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="56bf1-230">继承自 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)。</span><span class="sxs-lookup"><span data-stu-id="56bf1-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="56bf1-231">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="56bf1-231">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="56bf1-232">identityName</span><span class="sxs-lookup"><span data-stu-id="56bf1-232">identityName</span></span>|<span data-ttu-id="56bf1-233">String</span><span class="sxs-lookup"><span data-stu-id="56bf1-233">String</span></span>|<span data-ttu-id="56bf1-234">标识名称。</span><span class="sxs-lookup"><span data-stu-id="56bf1-234">The Identity Name.</span></span> <span data-ttu-id="56bf1-235">继承自 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-235">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="56bf1-236">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="56bf1-236">identityPublisherHash</span></span>|<span data-ttu-id="56bf1-237">String</span><span class="sxs-lookup"><span data-stu-id="56bf1-237">String</span></span>|<span data-ttu-id="56bf1-238">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="56bf1-238">The Identity Publisher Hash.</span></span> <span data-ttu-id="56bf1-239">继承自 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-239">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="56bf1-240">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="56bf1-240">identityResourceIdentifier</span></span>|<span data-ttu-id="56bf1-241">String</span><span class="sxs-lookup"><span data-stu-id="56bf1-241">String</span></span>|<span data-ttu-id="56bf1-242">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="56bf1-242">The Identity Resource Identifier.</span></span> <span data-ttu-id="56bf1-243">继承自 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-243">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="56bf1-244">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="56bf1-244">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="56bf1-245">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="56bf1-245">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="56bf1-246">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="56bf1-246">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="56bf1-247">继承自 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-247">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="56bf1-248">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="56bf1-248">phoneProductIdentifier</span></span>|<span data-ttu-id="56bf1-249">String</span><span class="sxs-lookup"><span data-stu-id="56bf1-249">String</span></span>|<span data-ttu-id="56bf1-250">电话产品标识符。</span><span class="sxs-lookup"><span data-stu-id="56bf1-250">The Phone Product Identifier.</span></span> <span data-ttu-id="56bf1-251">继承自 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-251">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="56bf1-252">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="56bf1-252">phonePublisherId</span></span>|<span data-ttu-id="56bf1-253">String</span><span class="sxs-lookup"><span data-stu-id="56bf1-253">String</span></span>|<span data-ttu-id="56bf1-254">电话发布者 ID。继承自 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-254">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="56bf1-255">identityVersion</span><span class="sxs-lookup"><span data-stu-id="56bf1-255">identityVersion</span></span>|<span data-ttu-id="56bf1-256">String</span><span class="sxs-lookup"><span data-stu-id="56bf1-256">String</span></span>|<span data-ttu-id="56bf1-257">标识版本。</span><span class="sxs-lookup"><span data-stu-id="56bf1-257">The identity version.</span></span> <span data-ttu-id="56bf1-258">继承自 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="56bf1-258">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="56bf1-259">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="56bf1-259">appXPackageInformationList</span></span>|<span data-ttu-id="56bf1-260">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56bf1-260">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="56bf1-261">AppX 程序包信息的列表。</span><span class="sxs-lookup"><span data-stu-id="56bf1-261">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="56bf1-262">响应</span><span class="sxs-lookup"><span data-stu-id="56bf1-262">Response</span></span>
<span data-ttu-id="56bf1-263">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56bf1-263">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56bf1-264">示例</span><span class="sxs-lookup"><span data-stu-id="56bf1-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="56bf1-265">请求</span><span class="sxs-lookup"><span data-stu-id="56bf1-265">Request</span></span>
<span data-ttu-id="56bf1-266">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="56bf1-266">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2468

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
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
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="56bf1-267">响应</span><span class="sxs-lookup"><span data-stu-id="56bf1-267">Response</span></span>
<span data-ttu-id="56bf1-p131">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="56bf1-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2640

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
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
      }
    }
  ]
}
```




