---
title: 创建 windowsAppX
description: 创建新的 windowsAppX 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 91b7b39c8bfe1ad9218a4c1d80fbf2ad60f4e083
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139100"
---
# <a name="create-windowsappx"></a><span data-ttu-id="a0636-103">创建 windowsAppX</span><span class="sxs-lookup"><span data-stu-id="a0636-103">Create windowsAppX</span></span>

<span data-ttu-id="a0636-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0636-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0636-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a0636-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0636-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a0636-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0636-107">创建新的 [windowsAppX](../resources/intune-apps-windowsappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0636-107">Create a new [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0636-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a0636-108">Prerequisites</span></span>
<span data-ttu-id="a0636-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0636-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0636-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0636-111">Permission type</span></span>|<span data-ttu-id="a0636-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0636-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0636-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0636-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0636-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0636-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a0636-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0636-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0636-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0636-116">Not supported.</span></span>|
|<span data-ttu-id="a0636-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0636-117">Application</span></span>|<span data-ttu-id="a0636-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0636-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0636-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0636-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a0636-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0636-120">Request headers</span></span>
|<span data-ttu-id="a0636-121">标头</span><span class="sxs-lookup"><span data-stu-id="a0636-121">Header</span></span>|<span data-ttu-id="a0636-122">值</span><span class="sxs-lookup"><span data-stu-id="a0636-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0636-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0636-123">Authorization</span></span>|<span data-ttu-id="a0636-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a0636-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0636-125">接受</span><span class="sxs-lookup"><span data-stu-id="a0636-125">Accept</span></span>|<span data-ttu-id="a0636-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0636-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0636-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0636-127">Request body</span></span>
<span data-ttu-id="a0636-128">在请求正文中，提供 windowsAppX 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0636-128">In the request body, supply a JSON representation for the windowsAppX object.</span></span>

<span data-ttu-id="a0636-129">下表显示创建 windowsAppX 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a0636-129">The following table shows the properties that are required when you create the windowsAppX.</span></span>

|<span data-ttu-id="a0636-130">属性</span><span class="sxs-lookup"><span data-stu-id="a0636-130">Property</span></span>|<span data-ttu-id="a0636-131">类型</span><span class="sxs-lookup"><span data-stu-id="a0636-131">Type</span></span>|<span data-ttu-id="a0636-132">说明</span><span class="sxs-lookup"><span data-stu-id="a0636-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0636-133">id</span><span class="sxs-lookup"><span data-stu-id="a0636-133">id</span></span>|<span data-ttu-id="a0636-134">String</span><span class="sxs-lookup"><span data-stu-id="a0636-134">String</span></span>|<span data-ttu-id="a0636-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a0636-135">Key of the entity.</span></span> <span data-ttu-id="a0636-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a0636-137">displayName</span></span>|<span data-ttu-id="a0636-138">String</span><span class="sxs-lookup"><span data-stu-id="a0636-138">String</span></span>|<span data-ttu-id="a0636-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="a0636-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a0636-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-141">说明</span><span class="sxs-lookup"><span data-stu-id="a0636-141">description</span></span>|<span data-ttu-id="a0636-142">String</span><span class="sxs-lookup"><span data-stu-id="a0636-142">String</span></span>|<span data-ttu-id="a0636-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="a0636-143">The description of the app.</span></span> <span data-ttu-id="a0636-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-145">publisher</span><span class="sxs-lookup"><span data-stu-id="a0636-145">publisher</span></span>|<span data-ttu-id="a0636-146">String</span><span class="sxs-lookup"><span data-stu-id="a0636-146">String</span></span>|<span data-ttu-id="a0636-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="a0636-147">The publisher of the app.</span></span> <span data-ttu-id="a0636-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a0636-149">largeIcon</span></span>|[<span data-ttu-id="a0636-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a0636-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a0636-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="a0636-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a0636-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0636-153">createdDateTime</span></span>|<span data-ttu-id="a0636-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0636-154">DateTimeOffset</span></span>|<span data-ttu-id="a0636-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a0636-155">The date and time the app was created.</span></span> <span data-ttu-id="a0636-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0636-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a0636-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0636-158">DateTimeOffset</span></span>|<span data-ttu-id="a0636-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a0636-159">The date and time the app was last modified.</span></span> <span data-ttu-id="a0636-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a0636-161">isFeatured</span></span>|<span data-ttu-id="a0636-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0636-162">Boolean</span></span>|<span data-ttu-id="a0636-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a0636-164">privacyInformationUrl</span></span>|<span data-ttu-id="a0636-165">String</span><span class="sxs-lookup"><span data-stu-id="a0636-165">String</span></span>|<span data-ttu-id="a0636-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="a0636-166">The privacy statement Url.</span></span> <span data-ttu-id="a0636-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a0636-168">informationUrl</span></span>|<span data-ttu-id="a0636-169">String</span><span class="sxs-lookup"><span data-stu-id="a0636-169">String</span></span>|<span data-ttu-id="a0636-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="a0636-170">The more information Url.</span></span> <span data-ttu-id="a0636-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-172">owner</span><span class="sxs-lookup"><span data-stu-id="a0636-172">owner</span></span>|<span data-ttu-id="a0636-173">String</span><span class="sxs-lookup"><span data-stu-id="a0636-173">String</span></span>|<span data-ttu-id="a0636-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="a0636-174">The owner of the app.</span></span> <span data-ttu-id="a0636-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-176">developer</span><span class="sxs-lookup"><span data-stu-id="a0636-176">developer</span></span>|<span data-ttu-id="a0636-177">String</span><span class="sxs-lookup"><span data-stu-id="a0636-177">String</span></span>|<span data-ttu-id="a0636-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="a0636-178">The developer of the app.</span></span> <span data-ttu-id="a0636-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-180">notes</span><span class="sxs-lookup"><span data-stu-id="a0636-180">notes</span></span>|<span data-ttu-id="a0636-181">String</span><span class="sxs-lookup"><span data-stu-id="a0636-181">String</span></span>|<span data-ttu-id="a0636-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="a0636-182">Notes for the app.</span></span> <span data-ttu-id="a0636-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="a0636-184">uploadState</span></span>|<span data-ttu-id="a0636-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a0636-185">Int32</span></span>|<span data-ttu-id="a0636-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="a0636-186">The upload state.</span></span> <span data-ttu-id="a0636-187">可能的值是：0 - `Not Ready` 、1 - `Ready` 、2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="a0636-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="a0636-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="a0636-189">publishingState</span></span>|[<span data-ttu-id="a0636-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a0636-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a0636-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="a0636-191">The publishing state for the app.</span></span> <span data-ttu-id="a0636-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="a0636-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a0636-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="a0636-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="a0636-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="a0636-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a0636-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a0636-195">isAssigned</span></span>|<span data-ttu-id="a0636-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0636-196">Boolean</span></span>|<span data-ttu-id="a0636-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="a0636-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a0636-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a0636-199">roleScopeTagIds</span></span>|<span data-ttu-id="a0636-200">String collection</span><span class="sxs-lookup"><span data-stu-id="a0636-200">String collection</span></span>|<span data-ttu-id="a0636-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="a0636-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a0636-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="a0636-203">dependentAppCount</span></span>|<span data-ttu-id="a0636-204">Int32</span><span class="sxs-lookup"><span data-stu-id="a0636-204">Int32</span></span>|<span data-ttu-id="a0636-205">子应用具有的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="a0636-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="a0636-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="a0636-207">supersedingAppCount</span></span>|<span data-ttu-id="a0636-208">Int32</span><span class="sxs-lookup"><span data-stu-id="a0636-208">Int32</span></span>|<span data-ttu-id="a0636-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="a0636-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="a0636-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="a0636-211">supersededAppCount</span></span>|<span data-ttu-id="a0636-212">Int32</span><span class="sxs-lookup"><span data-stu-id="a0636-212">Int32</span></span>|<span data-ttu-id="a0636-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="a0636-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="a0636-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a0636-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="a0636-215">committedContentVersion</span></span>|<span data-ttu-id="a0636-216">String</span><span class="sxs-lookup"><span data-stu-id="a0636-216">String</span></span>|<span data-ttu-id="a0636-217">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="a0636-217">The internal committed content version.</span></span> <span data-ttu-id="a0636-218">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a0636-219">fileName</span><span class="sxs-lookup"><span data-stu-id="a0636-219">fileName</span></span>|<span data-ttu-id="a0636-220">String</span><span class="sxs-lookup"><span data-stu-id="a0636-220">String</span></span>|<span data-ttu-id="a0636-221">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="a0636-221">The name of the main Lob application file.</span></span> <span data-ttu-id="a0636-222">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a0636-223">size</span><span class="sxs-lookup"><span data-stu-id="a0636-223">size</span></span>|<span data-ttu-id="a0636-224">Int64</span><span class="sxs-lookup"><span data-stu-id="a0636-224">Int64</span></span>|<span data-ttu-id="a0636-225">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="a0636-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="a0636-226">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0636-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a0636-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="a0636-227">applicableArchitectures</span></span>|[<span data-ttu-id="a0636-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="a0636-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="a0636-229">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="a0636-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="a0636-230">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="a0636-230">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="a0636-231">identityName</span><span class="sxs-lookup"><span data-stu-id="a0636-231">identityName</span></span>|<span data-ttu-id="a0636-232">String</span><span class="sxs-lookup"><span data-stu-id="a0636-232">String</span></span>|<span data-ttu-id="a0636-233">标识名称。</span><span class="sxs-lookup"><span data-stu-id="a0636-233">The Identity Name.</span></span>|
|<span data-ttu-id="a0636-234">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="a0636-234">identityPublisherHash</span></span>|<span data-ttu-id="a0636-235">String</span><span class="sxs-lookup"><span data-stu-id="a0636-235">String</span></span>|<span data-ttu-id="a0636-236">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="a0636-236">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="a0636-237">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="a0636-237">identityResourceIdentifier</span></span>|<span data-ttu-id="a0636-238">String</span><span class="sxs-lookup"><span data-stu-id="a0636-238">String</span></span>|<span data-ttu-id="a0636-239">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="a0636-239">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="a0636-240">isBundle</span><span class="sxs-lookup"><span data-stu-id="a0636-240">isBundle</span></span>|<span data-ttu-id="a0636-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0636-241">Boolean</span></span>|<span data-ttu-id="a0636-242">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="a0636-242">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="a0636-243">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a0636-243">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a0636-244">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a0636-244">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="a0636-245">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="a0636-245">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="a0636-246">identityVersion</span><span class="sxs-lookup"><span data-stu-id="a0636-246">identityVersion</span></span>|<span data-ttu-id="a0636-247">String</span><span class="sxs-lookup"><span data-stu-id="a0636-247">String</span></span>|<span data-ttu-id="a0636-248">标识版本。</span><span class="sxs-lookup"><span data-stu-id="a0636-248">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="a0636-249">响应</span><span class="sxs-lookup"><span data-stu-id="a0636-249">Response</span></span>
<span data-ttu-id="a0636-250">如果成功，此方法在响应正文中返回 响应代码 `201 Created` 和 [windowsAppX](../resources/intune-apps-windowsappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0636-250">If successful, this method returns a `201 Created` response code and a [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0636-251">示例</span><span class="sxs-lookup"><span data-stu-id="a0636-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0636-252">请求</span><span class="sxs-lookup"><span data-stu-id="a0636-252">Request</span></span>
<span data-ttu-id="a0636-253">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0636-253">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="a0636-254">响应</span><span class="sxs-lookup"><span data-stu-id="a0636-254">Response</span></span>
<span data-ttu-id="a0636-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0636-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




