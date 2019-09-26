---
title: 创建 macOSLobApp
description: 创建新的 macOSLobApp 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1c8cad5efba5848bf7208d0777292cfa2d7d9d9f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37173407"
---
# <a name="create-macoslobapp"></a><span data-ttu-id="b4b11-103">创建 macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="b4b11-103">Create macOSLobApp</span></span>

> <span data-ttu-id="b4b11-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b4b11-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4b11-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4b11-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4b11-106">创建新的[macOSLobApp](../resources/intune-apps-macoslobapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b4b11-106">Create a new [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4b11-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b4b11-107">Prerequisites</span></span>
<span data-ttu-id="b4b11-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4b11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4b11-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4b11-110">Permission type</span></span>|<span data-ttu-id="b4b11-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b4b11-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4b11-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4b11-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b4b11-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4b11-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b4b11-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4b11-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4b11-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4b11-115">Not supported.</span></span>|
|<span data-ttu-id="b4b11-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4b11-116">Application</span></span>|<span data-ttu-id="b4b11-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4b11-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4b11-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4b11-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b4b11-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4b11-119">Request headers</span></span>
|<span data-ttu-id="b4b11-120">标头</span><span class="sxs-lookup"><span data-stu-id="b4b11-120">Header</span></span>|<span data-ttu-id="b4b11-121">值</span><span class="sxs-lookup"><span data-stu-id="b4b11-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4b11-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4b11-122">Authorization</span></span>|<span data-ttu-id="b4b11-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b4b11-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4b11-124">接受</span><span class="sxs-lookup"><span data-stu-id="b4b11-124">Accept</span></span>|<span data-ttu-id="b4b11-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b4b11-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4b11-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4b11-126">Request body</span></span>
<span data-ttu-id="b4b11-127">在请求正文中，提供 macOSLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4b11-127">In the request body, supply a JSON representation for the macOSLobApp object.</span></span>

<span data-ttu-id="b4b11-128">下表显示创建 macOSLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b4b11-128">The following table shows the properties that are required when you create the macOSLobApp.</span></span>

|<span data-ttu-id="b4b11-129">属性</span><span class="sxs-lookup"><span data-stu-id="b4b11-129">Property</span></span>|<span data-ttu-id="b4b11-130">类型</span><span class="sxs-lookup"><span data-stu-id="b4b11-130">Type</span></span>|<span data-ttu-id="b4b11-131">说明</span><span class="sxs-lookup"><span data-stu-id="b4b11-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4b11-132">id</span><span class="sxs-lookup"><span data-stu-id="b4b11-132">id</span></span>|<span data-ttu-id="b4b11-133">字符串</span><span class="sxs-lookup"><span data-stu-id="b4b11-133">String</span></span>|<span data-ttu-id="b4b11-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b4b11-134">Key of the entity.</span></span> <span data-ttu-id="b4b11-135">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4b11-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b4b11-136">displayName</span></span>|<span data-ttu-id="b4b11-137">String</span><span class="sxs-lookup"><span data-stu-id="b4b11-137">String</span></span>|<span data-ttu-id="b4b11-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="b4b11-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b4b11-139">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4b11-140">说明</span><span class="sxs-lookup"><span data-stu-id="b4b11-140">description</span></span>|<span data-ttu-id="b4b11-141">字符串</span><span class="sxs-lookup"><span data-stu-id="b4b11-141">String</span></span>|<span data-ttu-id="b4b11-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="b4b11-142">The description of the app.</span></span> <span data-ttu-id="b4b11-143">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4b11-144">publisher</span><span class="sxs-lookup"><span data-stu-id="b4b11-144">publisher</span></span>|<span data-ttu-id="b4b11-145">String</span><span class="sxs-lookup"><span data-stu-id="b4b11-145">String</span></span>|<span data-ttu-id="b4b11-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="b4b11-146">The publisher of the app.</span></span> <span data-ttu-id="b4b11-147">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4b11-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b4b11-148">largeIcon</span></span>|[<span data-ttu-id="b4b11-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b4b11-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b4b11-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="b4b11-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b4b11-151">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4b11-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4b11-152">createdDateTime</span></span>|<span data-ttu-id="b4b11-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4b11-153">DateTimeOffset</span></span>|<span data-ttu-id="b4b11-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b4b11-154">The date and time the app was created.</span></span> <span data-ttu-id="b4b11-155">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4b11-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4b11-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b4b11-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4b11-157">DateTimeOffset</span></span>|<span data-ttu-id="b4b11-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b4b11-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b4b11-159">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4b11-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b4b11-160">isFeatured</span></span>|<span data-ttu-id="b4b11-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4b11-161">Boolean</span></span>|<span data-ttu-id="b4b11-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4b11-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b4b11-163">privacyInformationUrl</span></span>|<span data-ttu-id="b4b11-164">String</span><span class="sxs-lookup"><span data-stu-id="b4b11-164">String</span></span>|<span data-ttu-id="b4b11-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="b4b11-165">The privacy statement Url.</span></span> <span data-ttu-id="b4b11-166">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4b11-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b4b11-167">informationUrl</span></span>|<span data-ttu-id="b4b11-168">String</span><span class="sxs-lookup"><span data-stu-id="b4b11-168">String</span></span>|<span data-ttu-id="b4b11-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="b4b11-169">The more information Url.</span></span> <span data-ttu-id="b4b11-170">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4b11-171">owner</span><span class="sxs-lookup"><span data-stu-id="b4b11-171">owner</span></span>|<span data-ttu-id="b4b11-172">String</span><span class="sxs-lookup"><span data-stu-id="b4b11-172">String</span></span>|<span data-ttu-id="b4b11-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="b4b11-173">The owner of the app.</span></span> <span data-ttu-id="b4b11-174">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4b11-175">developer</span><span class="sxs-lookup"><span data-stu-id="b4b11-175">developer</span></span>|<span data-ttu-id="b4b11-176">String</span><span class="sxs-lookup"><span data-stu-id="b4b11-176">String</span></span>|<span data-ttu-id="b4b11-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="b4b11-177">The developer of the app.</span></span> <span data-ttu-id="b4b11-178">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4b11-179">notes</span><span class="sxs-lookup"><span data-stu-id="b4b11-179">notes</span></span>|<span data-ttu-id="b4b11-180">String</span><span class="sxs-lookup"><span data-stu-id="b4b11-180">String</span></span>|<span data-ttu-id="b4b11-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="b4b11-181">Notes for the app.</span></span> <span data-ttu-id="b4b11-182">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4b11-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="b4b11-183">uploadState</span></span>|<span data-ttu-id="b4b11-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b4b11-184">Int32</span></span>|<span data-ttu-id="b4b11-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="b4b11-185">The upload state.</span></span> <span data-ttu-id="b4b11-186">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4b11-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="b4b11-187">publishingState</span></span>|[<span data-ttu-id="b4b11-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b4b11-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b4b11-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="b4b11-189">The publishing state for the app.</span></span> <span data-ttu-id="b4b11-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="b4b11-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b4b11-191">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="b4b11-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="b4b11-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="b4b11-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b4b11-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b4b11-193">isAssigned</span></span>|<span data-ttu-id="b4b11-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4b11-194">Boolean</span></span>|<span data-ttu-id="b4b11-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="b4b11-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b4b11-196">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4b11-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b4b11-197">roleScopeTagIds</span></span>|<span data-ttu-id="b4b11-198">String collection</span><span class="sxs-lookup"><span data-stu-id="b4b11-198">String collection</span></span>|<span data-ttu-id="b4b11-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="b4b11-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b4b11-200">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4b11-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="b4b11-201">dependentAppCount</span></span>|<span data-ttu-id="b4b11-202">Int32</span><span class="sxs-lookup"><span data-stu-id="b4b11-202">Int32</span></span>|<span data-ttu-id="b4b11-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="b4b11-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b4b11-204">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4b11-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b4b11-205">committedContentVersion</span></span>|<span data-ttu-id="b4b11-206">String</span><span class="sxs-lookup"><span data-stu-id="b4b11-206">String</span></span>|<span data-ttu-id="b4b11-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="b4b11-207">The internal committed content version.</span></span> <span data-ttu-id="b4b11-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b4b11-209">fileName</span><span class="sxs-lookup"><span data-stu-id="b4b11-209">fileName</span></span>|<span data-ttu-id="b4b11-210">String</span><span class="sxs-lookup"><span data-stu-id="b4b11-210">String</span></span>|<span data-ttu-id="b4b11-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="b4b11-211">The name of the main Lob application file.</span></span> <span data-ttu-id="b4b11-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b4b11-213">size</span><span class="sxs-lookup"><span data-stu-id="b4b11-213">size</span></span>|<span data-ttu-id="b4b11-214">Int64</span><span class="sxs-lookup"><span data-stu-id="b4b11-214">Int64</span></span>|<span data-ttu-id="b4b11-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="b4b11-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="b4b11-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4b11-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b4b11-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="b4b11-217">bundleId</span></span>|<span data-ttu-id="b4b11-218">String</span><span class="sxs-lookup"><span data-stu-id="b4b11-218">String</span></span>|<span data-ttu-id="b4b11-219">捆绑包 id。</span><span class="sxs-lookup"><span data-stu-id="b4b11-219">The bundle id.</span></span>|
|<span data-ttu-id="b4b11-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b4b11-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b4b11-221">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b4b11-221">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="b4b11-222">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="b4b11-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="b4b11-223">buildNumber</span><span class="sxs-lookup"><span data-stu-id="b4b11-223">buildNumber</span></span>|<span data-ttu-id="b4b11-224">String</span><span class="sxs-lookup"><span data-stu-id="b4b11-224">String</span></span>|<span data-ttu-id="b4b11-225">MacOS 业务线（LoB）应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="b4b11-225">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b4b11-226">versionNumber</span><span class="sxs-lookup"><span data-stu-id="b4b11-226">versionNumber</span></span>|<span data-ttu-id="b4b11-227">String</span><span class="sxs-lookup"><span data-stu-id="b4b11-227">String</span></span>|<span data-ttu-id="b4b11-228">MacOS 业务线（LoB）应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="b4b11-228">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b4b11-229">childApps</span><span class="sxs-lookup"><span data-stu-id="b4b11-229">childApps</span></span>|<span data-ttu-id="b4b11-230">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="b4b11-230">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="b4b11-231">此捆绑包包中的应用程序列表</span><span class="sxs-lookup"><span data-stu-id="b4b11-231">The app list in this bundle package</span></span>|
|<span data-ttu-id="b4b11-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="b4b11-232">identityVersion</span></span>|<span data-ttu-id="b4b11-233">String</span><span class="sxs-lookup"><span data-stu-id="b4b11-233">String</span></span>|<span data-ttu-id="b4b11-234">标识版本。</span><span class="sxs-lookup"><span data-stu-id="b4b11-234">The identity version.</span></span>|
|<span data-ttu-id="b4b11-235">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="b4b11-235">md5HashChunkSize</span></span>|<span data-ttu-id="b4b11-236">Int32</span><span class="sxs-lookup"><span data-stu-id="b4b11-236">Int32</span></span>|<span data-ttu-id="b4b11-237">MD5 哈希的块大小</span><span class="sxs-lookup"><span data-stu-id="b4b11-237">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="b4b11-238">md5Hash</span><span class="sxs-lookup"><span data-stu-id="b4b11-238">md5Hash</span></span>|<span data-ttu-id="b4b11-239">String collection</span><span class="sxs-lookup"><span data-stu-id="b4b11-239">String collection</span></span>|<span data-ttu-id="b4b11-240">MD5 哈希代码</span><span class="sxs-lookup"><span data-stu-id="b4b11-240">The MD5 hash codes</span></span>|
|<span data-ttu-id="b4b11-241">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="b4b11-241">ignoreVersionDetection</span></span>|<span data-ttu-id="b4b11-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4b11-242">Boolean</span></span>|<span data-ttu-id="b4b11-243">控制应用的版本是否将用于检测安装在设备上的应用的布尔值。</span><span class="sxs-lookup"><span data-stu-id="b4b11-243">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="b4b11-244">对于使用自我更新功能的 macOS 业务线（LoB）应用，请将此设置为 true。</span><span class="sxs-lookup"><span data-stu-id="b4b11-244">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="b4b11-245">响应</span><span class="sxs-lookup"><span data-stu-id="b4b11-245">Response</span></span>
<span data-ttu-id="b4b11-246">如果成功，此方法在响应`201 Created`正文中返回响应代码和[macOSLobApp](../resources/intune-apps-macoslobapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b4b11-246">If successful, this method returns a `201 Created` response code and a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4b11-247">示例</span><span class="sxs-lookup"><span data-stu-id="b4b11-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4b11-248">请求</span><span class="sxs-lookup"><span data-stu-id="b4b11-248">Request</span></span>
<span data-ttu-id="b4b11-249">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4b11-249">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1616

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true,
    "v10_14": true,
    "v10_15": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="b4b11-250">响应</span><span class="sxs-lookup"><span data-stu-id="b4b11-250">Response</span></span>
<span data-ttu-id="b4b11-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b4b11-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1788

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
  "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true,
    "v10_14": true,
    "v10_15": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```




