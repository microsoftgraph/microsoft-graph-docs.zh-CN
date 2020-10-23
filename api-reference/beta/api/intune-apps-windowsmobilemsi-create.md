---
title: 创建 windowsMobileMSI
description: 创建新的 windowsMobileMSI 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4bc5f1a768fd6de1a036227ce973e1f061bef668
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708695"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="d4797-103">创建 windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="d4797-103">Create windowsMobileMSI</span></span>

<span data-ttu-id="d4797-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4797-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4797-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d4797-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4797-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4797-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4797-107">创建新的 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d4797-107">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4797-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d4797-108">Prerequisites</span></span>
<span data-ttu-id="d4797-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4797-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4797-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4797-111">Permission type</span></span>|<span data-ttu-id="d4797-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d4797-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4797-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4797-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4797-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4797-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d4797-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4797-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4797-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4797-116">Not supported.</span></span>|
|<span data-ttu-id="d4797-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4797-117">Application</span></span>|<span data-ttu-id="d4797-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4797-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4797-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4797-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d4797-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4797-120">Request headers</span></span>
|<span data-ttu-id="d4797-121">标头</span><span class="sxs-lookup"><span data-stu-id="d4797-121">Header</span></span>|<span data-ttu-id="d4797-122">值</span><span class="sxs-lookup"><span data-stu-id="d4797-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4797-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4797-123">Authorization</span></span>|<span data-ttu-id="d4797-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d4797-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4797-125">接受</span><span class="sxs-lookup"><span data-stu-id="d4797-125">Accept</span></span>|<span data-ttu-id="d4797-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4797-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4797-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4797-127">Request body</span></span>
<span data-ttu-id="d4797-128">在请求正文中，提供 windowsMobileMSI 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4797-128">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="d4797-129">下表显示创建 windowsMobileMSI 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d4797-129">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="d4797-130">属性</span><span class="sxs-lookup"><span data-stu-id="d4797-130">Property</span></span>|<span data-ttu-id="d4797-131">类型</span><span class="sxs-lookup"><span data-stu-id="d4797-131">Type</span></span>|<span data-ttu-id="d4797-132">说明</span><span class="sxs-lookup"><span data-stu-id="d4797-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4797-133">id</span><span class="sxs-lookup"><span data-stu-id="d4797-133">id</span></span>|<span data-ttu-id="d4797-134">String</span><span class="sxs-lookup"><span data-stu-id="d4797-134">String</span></span>|<span data-ttu-id="d4797-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d4797-135">Key of the entity.</span></span> <span data-ttu-id="d4797-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d4797-137">displayName</span></span>|<span data-ttu-id="d4797-138">String</span><span class="sxs-lookup"><span data-stu-id="d4797-138">String</span></span>|<span data-ttu-id="d4797-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="d4797-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d4797-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-141">说明</span><span class="sxs-lookup"><span data-stu-id="d4797-141">description</span></span>|<span data-ttu-id="d4797-142">String</span><span class="sxs-lookup"><span data-stu-id="d4797-142">String</span></span>|<span data-ttu-id="d4797-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="d4797-143">The description of the app.</span></span> <span data-ttu-id="d4797-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-145">publisher</span><span class="sxs-lookup"><span data-stu-id="d4797-145">publisher</span></span>|<span data-ttu-id="d4797-146">String</span><span class="sxs-lookup"><span data-stu-id="d4797-146">String</span></span>|<span data-ttu-id="d4797-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="d4797-147">The publisher of the app.</span></span> <span data-ttu-id="d4797-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d4797-149">largeIcon</span></span>|[<span data-ttu-id="d4797-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d4797-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d4797-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="d4797-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d4797-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4797-153">createdDateTime</span></span>|<span data-ttu-id="d4797-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4797-154">DateTimeOffset</span></span>|<span data-ttu-id="d4797-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d4797-155">The date and time the app was created.</span></span> <span data-ttu-id="d4797-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4797-157">lastModifiedDateTime</span></span>|<span data-ttu-id="d4797-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4797-158">DateTimeOffset</span></span>|<span data-ttu-id="d4797-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d4797-159">The date and time the app was last modified.</span></span> <span data-ttu-id="d4797-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d4797-161">isFeatured</span></span>|<span data-ttu-id="d4797-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4797-162">Boolean</span></span>|<span data-ttu-id="d4797-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d4797-164">privacyInformationUrl</span></span>|<span data-ttu-id="d4797-165">String</span><span class="sxs-lookup"><span data-stu-id="d4797-165">String</span></span>|<span data-ttu-id="d4797-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="d4797-166">The privacy statement Url.</span></span> <span data-ttu-id="d4797-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d4797-168">informationUrl</span></span>|<span data-ttu-id="d4797-169">String</span><span class="sxs-lookup"><span data-stu-id="d4797-169">String</span></span>|<span data-ttu-id="d4797-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="d4797-170">The more information Url.</span></span> <span data-ttu-id="d4797-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-172">owner</span><span class="sxs-lookup"><span data-stu-id="d4797-172">owner</span></span>|<span data-ttu-id="d4797-173">String</span><span class="sxs-lookup"><span data-stu-id="d4797-173">String</span></span>|<span data-ttu-id="d4797-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="d4797-174">The owner of the app.</span></span> <span data-ttu-id="d4797-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-176">developer</span><span class="sxs-lookup"><span data-stu-id="d4797-176">developer</span></span>|<span data-ttu-id="d4797-177">String</span><span class="sxs-lookup"><span data-stu-id="d4797-177">String</span></span>|<span data-ttu-id="d4797-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="d4797-178">The developer of the app.</span></span> <span data-ttu-id="d4797-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-180">notes</span><span class="sxs-lookup"><span data-stu-id="d4797-180">notes</span></span>|<span data-ttu-id="d4797-181">String</span><span class="sxs-lookup"><span data-stu-id="d4797-181">String</span></span>|<span data-ttu-id="d4797-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="d4797-182">Notes for the app.</span></span> <span data-ttu-id="d4797-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="d4797-184">uploadState</span></span>|<span data-ttu-id="d4797-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d4797-185">Int32</span></span>|<span data-ttu-id="d4797-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="d4797-186">The upload state.</span></span> <span data-ttu-id="d4797-187">可能的值包括： 0- `Not Ready` 、1- `Ready` 、2- `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="d4797-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="d4797-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="d4797-189">publishingState</span></span>|[<span data-ttu-id="d4797-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d4797-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d4797-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="d4797-191">The publishing state for the app.</span></span> <span data-ttu-id="d4797-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="d4797-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d4797-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="d4797-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="d4797-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="d4797-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d4797-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d4797-195">isAssigned</span></span>|<span data-ttu-id="d4797-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4797-196">Boolean</span></span>|<span data-ttu-id="d4797-197">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="d4797-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d4797-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d4797-199">roleScopeTagIds</span></span>|<span data-ttu-id="d4797-200">String collection</span><span class="sxs-lookup"><span data-stu-id="d4797-200">String collection</span></span>|<span data-ttu-id="d4797-201">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="d4797-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d4797-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="d4797-203">dependentAppCount</span></span>|<span data-ttu-id="d4797-204">Int32</span><span class="sxs-lookup"><span data-stu-id="d4797-204">Int32</span></span>|<span data-ttu-id="d4797-205">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="d4797-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="d4797-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="d4797-207">supersedingAppCount</span></span>|<span data-ttu-id="d4797-208">Int32</span><span class="sxs-lookup"><span data-stu-id="d4797-208">Int32</span></span>|<span data-ttu-id="d4797-209">此应用程序直接或间接取代的应用程序总数量。</span><span class="sxs-lookup"><span data-stu-id="d4797-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="d4797-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="d4797-211">supersededAppCount</span></span>|<span data-ttu-id="d4797-212">Int32</span><span class="sxs-lookup"><span data-stu-id="d4797-212">Int32</span></span>|<span data-ttu-id="d4797-213">此应用程序直接或间接取代的应用程序总数量。</span><span class="sxs-lookup"><span data-stu-id="d4797-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="d4797-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4797-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d4797-215">committedContentVersion</span></span>|<span data-ttu-id="d4797-216">String</span><span class="sxs-lookup"><span data-stu-id="d4797-216">String</span></span>|<span data-ttu-id="d4797-217">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="d4797-217">The internal committed content version.</span></span> <span data-ttu-id="d4797-218">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d4797-219">fileName</span><span class="sxs-lookup"><span data-stu-id="d4797-219">fileName</span></span>|<span data-ttu-id="d4797-220">String</span><span class="sxs-lookup"><span data-stu-id="d4797-220">String</span></span>|<span data-ttu-id="d4797-221">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="d4797-221">The name of the main Lob application file.</span></span> <span data-ttu-id="d4797-222">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d4797-223">size</span><span class="sxs-lookup"><span data-stu-id="d4797-223">size</span></span>|<span data-ttu-id="d4797-224">Int64</span><span class="sxs-lookup"><span data-stu-id="d4797-224">Int64</span></span>|<span data-ttu-id="d4797-225">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="d4797-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="d4797-226">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4797-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d4797-227">commandLine</span><span class="sxs-lookup"><span data-stu-id="d4797-227">commandLine</span></span>|<span data-ttu-id="d4797-228">String</span><span class="sxs-lookup"><span data-stu-id="d4797-228">String</span></span>|<span data-ttu-id="d4797-229">命令行。</span><span class="sxs-lookup"><span data-stu-id="d4797-229">The command line.</span></span>|
|<span data-ttu-id="d4797-230">productCode</span><span class="sxs-lookup"><span data-stu-id="d4797-230">productCode</span></span>|<span data-ttu-id="d4797-231">String</span><span class="sxs-lookup"><span data-stu-id="d4797-231">String</span></span>|<span data-ttu-id="d4797-232">产品代码。</span><span class="sxs-lookup"><span data-stu-id="d4797-232">The product code.</span></span>|
|<span data-ttu-id="d4797-233">productVersion</span><span class="sxs-lookup"><span data-stu-id="d4797-233">productVersion</span></span>|<span data-ttu-id="d4797-234">String</span><span class="sxs-lookup"><span data-stu-id="d4797-234">String</span></span>|<span data-ttu-id="d4797-235">Windows Mobile MSI 业务线 (LoB) 应用的产品版本。</span><span class="sxs-lookup"><span data-stu-id="d4797-235">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d4797-236">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="d4797-236">ignoreVersionDetection</span></span>|<span data-ttu-id="d4797-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4797-237">Boolean</span></span>|<span data-ttu-id="d4797-238">控制应用的版本是否将用于检测安装在设备上的应用的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d4797-238">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="d4797-239">对于使用自更新功能的 Windows Mobile MSI 业务线 (LoB) 应用，将此值设置为 true。</span><span class="sxs-lookup"><span data-stu-id="d4797-239">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="d4797-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="d4797-240">identityVersion</span></span>|<span data-ttu-id="d4797-241">String</span><span class="sxs-lookup"><span data-stu-id="d4797-241">String</span></span>|<span data-ttu-id="d4797-242">标识版本。</span><span class="sxs-lookup"><span data-stu-id="d4797-242">The identity version.</span></span>|
|<span data-ttu-id="d4797-243">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="d4797-243">useDeviceContext</span></span>|<span data-ttu-id="d4797-244">布尔值</span><span class="sxs-lookup"><span data-stu-id="d4797-244">Boolean</span></span>|<span data-ttu-id="d4797-245">指示是否在设备上下文中安装双模式 MSI。</span><span class="sxs-lookup"><span data-stu-id="d4797-245">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="d4797-246">如果为 true，则将为所有用户安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="d4797-246">If true, app will be installed for all users.</span></span> <span data-ttu-id="d4797-247">如果为 false，将按用户安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="d4797-247">If false, app will be installed per-user.</span></span> <span data-ttu-id="d4797-248">如果为 null，服务将使用 MSI 包的默认安装上下文。</span><span class="sxs-lookup"><span data-stu-id="d4797-248">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="d4797-249">在双模式 MSI 的情况下，此默认值将为每个用户。</span><span class="sxs-lookup"><span data-stu-id="d4797-249">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="d4797-250">不能为非双重模式的应用程序进行设置。</span><span class="sxs-lookup"><span data-stu-id="d4797-250">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="d4797-251">在首次创建应用程序后，不能更改。</span><span class="sxs-lookup"><span data-stu-id="d4797-251">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="d4797-252">响应</span><span class="sxs-lookup"><span data-stu-id="d4797-252">Response</span></span>
<span data-ttu-id="d4797-253">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d4797-253">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4797-254">示例</span><span class="sxs-lookup"><span data-stu-id="d4797-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4797-255">请求</span><span class="sxs-lookup"><span data-stu-id="d4797-255">Request</span></span>
<span data-ttu-id="d4797-256">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d4797-256">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1123

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="d4797-257">响应</span><span class="sxs-lookup"><span data-stu-id="d4797-257">Response</span></span>
<span data-ttu-id="d4797-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d4797-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1295

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```





