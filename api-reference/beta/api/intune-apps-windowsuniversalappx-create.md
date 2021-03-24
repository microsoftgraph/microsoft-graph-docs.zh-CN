---
title: 创建 windowsUniversalAppX
description: 创建新的 windowsUniversalAppX 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a6141bda710051ff85460204257cb3edc1b50e99
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128542"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="ff25a-103">创建 windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="ff25a-103">Create windowsUniversalAppX</span></span>

<span data-ttu-id="ff25a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff25a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff25a-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff25a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff25a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff25a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff25a-107">创建新的 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ff25a-107">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff25a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ff25a-108">Prerequisites</span></span>
<span data-ttu-id="ff25a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff25a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff25a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff25a-111">Permission type</span></span>|<span data-ttu-id="ff25a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ff25a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff25a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff25a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff25a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff25a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ff25a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff25a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff25a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff25a-116">Not supported.</span></span>|
|<span data-ttu-id="ff25a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff25a-117">Application</span></span>|<span data-ttu-id="ff25a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff25a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff25a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff25a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ff25a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff25a-120">Request headers</span></span>
|<span data-ttu-id="ff25a-121">标头</span><span class="sxs-lookup"><span data-stu-id="ff25a-121">Header</span></span>|<span data-ttu-id="ff25a-122">值</span><span class="sxs-lookup"><span data-stu-id="ff25a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff25a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff25a-123">Authorization</span></span>|<span data-ttu-id="ff25a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ff25a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff25a-125">接受</span><span class="sxs-lookup"><span data-stu-id="ff25a-125">Accept</span></span>|<span data-ttu-id="ff25a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff25a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff25a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff25a-127">Request body</span></span>
<span data-ttu-id="ff25a-128">在请求正文中，提供 windowsUniversalAppX 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff25a-128">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="ff25a-129">下表显示创建 windowsUniversalAppX 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ff25a-129">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="ff25a-130">属性</span><span class="sxs-lookup"><span data-stu-id="ff25a-130">Property</span></span>|<span data-ttu-id="ff25a-131">类型</span><span class="sxs-lookup"><span data-stu-id="ff25a-131">Type</span></span>|<span data-ttu-id="ff25a-132">说明</span><span class="sxs-lookup"><span data-stu-id="ff25a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff25a-133">id</span><span class="sxs-lookup"><span data-stu-id="ff25a-133">id</span></span>|<span data-ttu-id="ff25a-134">String</span><span class="sxs-lookup"><span data-stu-id="ff25a-134">String</span></span>|<span data-ttu-id="ff25a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ff25a-135">Key of the entity.</span></span> <span data-ttu-id="ff25a-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ff25a-137">displayName</span></span>|<span data-ttu-id="ff25a-138">String</span><span class="sxs-lookup"><span data-stu-id="ff25a-138">String</span></span>|<span data-ttu-id="ff25a-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="ff25a-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ff25a-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-141">说明</span><span class="sxs-lookup"><span data-stu-id="ff25a-141">description</span></span>|<span data-ttu-id="ff25a-142">String</span><span class="sxs-lookup"><span data-stu-id="ff25a-142">String</span></span>|<span data-ttu-id="ff25a-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="ff25a-143">The description of the app.</span></span> <span data-ttu-id="ff25a-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ff25a-145">publisher</span></span>|<span data-ttu-id="ff25a-146">String</span><span class="sxs-lookup"><span data-stu-id="ff25a-146">String</span></span>|<span data-ttu-id="ff25a-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="ff25a-147">The publisher of the app.</span></span> <span data-ttu-id="ff25a-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ff25a-149">largeIcon</span></span>|[<span data-ttu-id="ff25a-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ff25a-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ff25a-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="ff25a-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ff25a-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff25a-153">createdDateTime</span></span>|<span data-ttu-id="ff25a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff25a-154">DateTimeOffset</span></span>|<span data-ttu-id="ff25a-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ff25a-155">The date and time the app was created.</span></span> <span data-ttu-id="ff25a-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff25a-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ff25a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff25a-158">DateTimeOffset</span></span>|<span data-ttu-id="ff25a-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ff25a-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ff25a-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ff25a-161">isFeatured</span></span>|<span data-ttu-id="ff25a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff25a-162">Boolean</span></span>|<span data-ttu-id="ff25a-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ff25a-164">privacyInformationUrl</span></span>|<span data-ttu-id="ff25a-165">String</span><span class="sxs-lookup"><span data-stu-id="ff25a-165">String</span></span>|<span data-ttu-id="ff25a-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="ff25a-166">The privacy statement Url.</span></span> <span data-ttu-id="ff25a-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ff25a-168">informationUrl</span></span>|<span data-ttu-id="ff25a-169">String</span><span class="sxs-lookup"><span data-stu-id="ff25a-169">String</span></span>|<span data-ttu-id="ff25a-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="ff25a-170">The more information Url.</span></span> <span data-ttu-id="ff25a-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-172">owner</span><span class="sxs-lookup"><span data-stu-id="ff25a-172">owner</span></span>|<span data-ttu-id="ff25a-173">String</span><span class="sxs-lookup"><span data-stu-id="ff25a-173">String</span></span>|<span data-ttu-id="ff25a-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="ff25a-174">The owner of the app.</span></span> <span data-ttu-id="ff25a-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-176">developer</span><span class="sxs-lookup"><span data-stu-id="ff25a-176">developer</span></span>|<span data-ttu-id="ff25a-177">String</span><span class="sxs-lookup"><span data-stu-id="ff25a-177">String</span></span>|<span data-ttu-id="ff25a-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="ff25a-178">The developer of the app.</span></span> <span data-ttu-id="ff25a-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-180">notes</span><span class="sxs-lookup"><span data-stu-id="ff25a-180">notes</span></span>|<span data-ttu-id="ff25a-181">String</span><span class="sxs-lookup"><span data-stu-id="ff25a-181">String</span></span>|<span data-ttu-id="ff25a-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="ff25a-182">Notes for the app.</span></span> <span data-ttu-id="ff25a-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ff25a-184">uploadState</span></span>|<span data-ttu-id="ff25a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ff25a-185">Int32</span></span>|<span data-ttu-id="ff25a-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="ff25a-186">The upload state.</span></span> <span data-ttu-id="ff25a-187">可能的值是：0 - `Not Ready` 、1 - `Ready` 、2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="ff25a-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="ff25a-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="ff25a-189">publishingState</span></span>|[<span data-ttu-id="ff25a-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ff25a-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ff25a-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="ff25a-191">The publishing state for the app.</span></span> <span data-ttu-id="ff25a-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="ff25a-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ff25a-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="ff25a-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ff25a-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="ff25a-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ff25a-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ff25a-195">isAssigned</span></span>|<span data-ttu-id="ff25a-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff25a-196">Boolean</span></span>|<span data-ttu-id="ff25a-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="ff25a-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ff25a-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ff25a-199">roleScopeTagIds</span></span>|<span data-ttu-id="ff25a-200">String collection</span><span class="sxs-lookup"><span data-stu-id="ff25a-200">String collection</span></span>|<span data-ttu-id="ff25a-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="ff25a-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ff25a-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="ff25a-203">dependentAppCount</span></span>|<span data-ttu-id="ff25a-204">Int32</span><span class="sxs-lookup"><span data-stu-id="ff25a-204">Int32</span></span>|<span data-ttu-id="ff25a-205">子应用具有的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="ff25a-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ff25a-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="ff25a-207">supersedingAppCount</span></span>|<span data-ttu-id="ff25a-208">Int32</span><span class="sxs-lookup"><span data-stu-id="ff25a-208">Int32</span></span>|<span data-ttu-id="ff25a-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="ff25a-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="ff25a-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="ff25a-211">supersededAppCount</span></span>|<span data-ttu-id="ff25a-212">Int32</span><span class="sxs-lookup"><span data-stu-id="ff25a-212">Int32</span></span>|<span data-ttu-id="ff25a-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="ff25a-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="ff25a-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff25a-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ff25a-215">committedContentVersion</span></span>|<span data-ttu-id="ff25a-216">String</span><span class="sxs-lookup"><span data-stu-id="ff25a-216">String</span></span>|<span data-ttu-id="ff25a-217">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="ff25a-217">The internal committed content version.</span></span> <span data-ttu-id="ff25a-218">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ff25a-219">fileName</span><span class="sxs-lookup"><span data-stu-id="ff25a-219">fileName</span></span>|<span data-ttu-id="ff25a-220">String</span><span class="sxs-lookup"><span data-stu-id="ff25a-220">String</span></span>|<span data-ttu-id="ff25a-221">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="ff25a-221">The name of the main Lob application file.</span></span> <span data-ttu-id="ff25a-222">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ff25a-223">size</span><span class="sxs-lookup"><span data-stu-id="ff25a-223">size</span></span>|<span data-ttu-id="ff25a-224">Int64</span><span class="sxs-lookup"><span data-stu-id="ff25a-224">Int64</span></span>|<span data-ttu-id="ff25a-225">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="ff25a-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="ff25a-226">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff25a-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ff25a-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="ff25a-227">applicableArchitectures</span></span>|[<span data-ttu-id="ff25a-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="ff25a-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="ff25a-229">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="ff25a-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="ff25a-230">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="ff25a-230">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="ff25a-231">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="ff25a-231">applicableDeviceTypes</span></span>|[<span data-ttu-id="ff25a-232">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="ff25a-232">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="ff25a-233">可运行此应用的 Windows 设备类型。</span><span class="sxs-lookup"><span data-stu-id="ff25a-233">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="ff25a-234">可取值为：`none`、`desktop`、`mobile`、`holographic`、`team`。</span><span class="sxs-lookup"><span data-stu-id="ff25a-234">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="ff25a-235">identityName</span><span class="sxs-lookup"><span data-stu-id="ff25a-235">identityName</span></span>|<span data-ttu-id="ff25a-236">String</span><span class="sxs-lookup"><span data-stu-id="ff25a-236">String</span></span>|<span data-ttu-id="ff25a-237">标识名称。</span><span class="sxs-lookup"><span data-stu-id="ff25a-237">The Identity Name.</span></span>|
|<span data-ttu-id="ff25a-238">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="ff25a-238">identityPublisherHash</span></span>|<span data-ttu-id="ff25a-239">String</span><span class="sxs-lookup"><span data-stu-id="ff25a-239">String</span></span>|<span data-ttu-id="ff25a-240">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="ff25a-240">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="ff25a-241">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ff25a-241">identityResourceIdentifier</span></span>|<span data-ttu-id="ff25a-242">String</span><span class="sxs-lookup"><span data-stu-id="ff25a-242">String</span></span>|<span data-ttu-id="ff25a-243">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="ff25a-243">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="ff25a-244">isBundle</span><span class="sxs-lookup"><span data-stu-id="ff25a-244">isBundle</span></span>|<span data-ttu-id="ff25a-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff25a-245">Boolean</span></span>|<span data-ttu-id="ff25a-246">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="ff25a-246">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="ff25a-247">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ff25a-247">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ff25a-248">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ff25a-248">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="ff25a-249">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="ff25a-249">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ff25a-250">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ff25a-250">identityVersion</span></span>|<span data-ttu-id="ff25a-251">String</span><span class="sxs-lookup"><span data-stu-id="ff25a-251">String</span></span>|<span data-ttu-id="ff25a-252">标识版本。</span><span class="sxs-lookup"><span data-stu-id="ff25a-252">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ff25a-253">响应</span><span class="sxs-lookup"><span data-stu-id="ff25a-253">Response</span></span>
<span data-ttu-id="ff25a-254">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ff25a-254">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff25a-255">示例</span><span class="sxs-lookup"><span data-stu-id="ff25a-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff25a-256">请求</span><span class="sxs-lookup"><span data-stu-id="ff25a-256">Request</span></span>
<span data-ttu-id="ff25a-257">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ff25a-257">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1564

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "applicableDeviceTypes": "desktop",
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

### <a name="response"></a><span data-ttu-id="ff25a-258">响应</span><span class="sxs-lookup"><span data-stu-id="ff25a-258">Response</span></span>
<span data-ttu-id="ff25a-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ff25a-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1736

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableDeviceTypes": "desktop",
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




