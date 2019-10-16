---
title: 创建 iosLobApp
description: 创建新的 iosLobApp 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ad0df70f908c42084d8f9769c1b01bf8d65929aa
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535434"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="1272f-103">创建 iosLobApp</span><span class="sxs-lookup"><span data-stu-id="1272f-103">Create iosLobApp</span></span>

> <span data-ttu-id="1272f-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1272f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1272f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1272f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1272f-106">创建新的 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1272f-106">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1272f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1272f-107">Prerequisites</span></span>
<span data-ttu-id="1272f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1272f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1272f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1272f-110">Permission type</span></span>|<span data-ttu-id="1272f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1272f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1272f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1272f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1272f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1272f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1272f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1272f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1272f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1272f-115">Not supported.</span></span>|
|<span data-ttu-id="1272f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1272f-116">Application</span></span>|<span data-ttu-id="1272f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1272f-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1272f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1272f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1272f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1272f-119">Request headers</span></span>
|<span data-ttu-id="1272f-120">标头</span><span class="sxs-lookup"><span data-stu-id="1272f-120">Header</span></span>|<span data-ttu-id="1272f-121">值</span><span class="sxs-lookup"><span data-stu-id="1272f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1272f-122">授权</span><span class="sxs-lookup"><span data-stu-id="1272f-122">Authorization</span></span>|<span data-ttu-id="1272f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1272f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1272f-124">接受</span><span class="sxs-lookup"><span data-stu-id="1272f-124">Accept</span></span>|<span data-ttu-id="1272f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1272f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1272f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1272f-126">Request body</span></span>
<span data-ttu-id="1272f-127">在请求正文中，提供 iosLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1272f-127">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="1272f-128">下表显示了创建 iosLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1272f-128">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="1272f-129">属性</span><span class="sxs-lookup"><span data-stu-id="1272f-129">Property</span></span>|<span data-ttu-id="1272f-130">类型</span><span class="sxs-lookup"><span data-stu-id="1272f-130">Type</span></span>|<span data-ttu-id="1272f-131">说明</span><span class="sxs-lookup"><span data-stu-id="1272f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1272f-132">id</span><span class="sxs-lookup"><span data-stu-id="1272f-132">id</span></span>|<span data-ttu-id="1272f-133">字符串</span><span class="sxs-lookup"><span data-stu-id="1272f-133">String</span></span>|<span data-ttu-id="1272f-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1272f-134">Key of the entity.</span></span> <span data-ttu-id="1272f-135">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1272f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1272f-136">displayName</span></span>|<span data-ttu-id="1272f-137">字符串</span><span class="sxs-lookup"><span data-stu-id="1272f-137">String</span></span>|<span data-ttu-id="1272f-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="1272f-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1272f-139">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1272f-140">说明</span><span class="sxs-lookup"><span data-stu-id="1272f-140">description</span></span>|<span data-ttu-id="1272f-141">字符串</span><span class="sxs-lookup"><span data-stu-id="1272f-141">String</span></span>|<span data-ttu-id="1272f-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="1272f-142">The description of the app.</span></span> <span data-ttu-id="1272f-143">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1272f-144">publisher</span><span class="sxs-lookup"><span data-stu-id="1272f-144">publisher</span></span>|<span data-ttu-id="1272f-145">字符串</span><span class="sxs-lookup"><span data-stu-id="1272f-145">String</span></span>|<span data-ttu-id="1272f-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="1272f-146">The publisher of the app.</span></span> <span data-ttu-id="1272f-147">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1272f-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1272f-148">largeIcon</span></span>|[<span data-ttu-id="1272f-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1272f-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1272f-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="1272f-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1272f-151">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1272f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1272f-152">createdDateTime</span></span>|<span data-ttu-id="1272f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1272f-153">DateTimeOffset</span></span>|<span data-ttu-id="1272f-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1272f-154">The date and time the app was created.</span></span> <span data-ttu-id="1272f-155">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1272f-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1272f-156">lastModifiedDateTime</span></span>|<span data-ttu-id="1272f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1272f-157">DateTimeOffset</span></span>|<span data-ttu-id="1272f-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1272f-158">The date and time the app was last modified.</span></span> <span data-ttu-id="1272f-159">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1272f-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1272f-160">isFeatured</span></span>|<span data-ttu-id="1272f-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="1272f-161">Boolean</span></span>|<span data-ttu-id="1272f-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1272f-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1272f-163">privacyInformationUrl</span></span>|<span data-ttu-id="1272f-164">字符串</span><span class="sxs-lookup"><span data-stu-id="1272f-164">String</span></span>|<span data-ttu-id="1272f-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="1272f-165">The privacy statement Url.</span></span> <span data-ttu-id="1272f-166">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1272f-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1272f-167">informationUrl</span></span>|<span data-ttu-id="1272f-168">字符串</span><span class="sxs-lookup"><span data-stu-id="1272f-168">String</span></span>|<span data-ttu-id="1272f-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="1272f-169">The more information Url.</span></span> <span data-ttu-id="1272f-170">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1272f-171">owner</span><span class="sxs-lookup"><span data-stu-id="1272f-171">owner</span></span>|<span data-ttu-id="1272f-172">String</span><span class="sxs-lookup"><span data-stu-id="1272f-172">String</span></span>|<span data-ttu-id="1272f-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="1272f-173">The owner of the app.</span></span> <span data-ttu-id="1272f-174">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1272f-175">developer</span><span class="sxs-lookup"><span data-stu-id="1272f-175">developer</span></span>|<span data-ttu-id="1272f-176">字符串</span><span class="sxs-lookup"><span data-stu-id="1272f-176">String</span></span>|<span data-ttu-id="1272f-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="1272f-177">The developer of the app.</span></span> <span data-ttu-id="1272f-178">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1272f-179">notes</span><span class="sxs-lookup"><span data-stu-id="1272f-179">notes</span></span>|<span data-ttu-id="1272f-180">字符串</span><span class="sxs-lookup"><span data-stu-id="1272f-180">String</span></span>|<span data-ttu-id="1272f-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="1272f-181">Notes for the app.</span></span> <span data-ttu-id="1272f-182">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1272f-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="1272f-183">uploadState</span></span>|<span data-ttu-id="1272f-184">Int32</span><span class="sxs-lookup"><span data-stu-id="1272f-184">Int32</span></span>|<span data-ttu-id="1272f-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="1272f-185">The upload state.</span></span> <span data-ttu-id="1272f-186">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1272f-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="1272f-187">publishingState</span></span>|[<span data-ttu-id="1272f-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1272f-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1272f-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="1272f-189">The publishing state for the app.</span></span> <span data-ttu-id="1272f-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="1272f-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1272f-191">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="1272f-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="1272f-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="1272f-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1272f-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1272f-193">isAssigned</span></span>|<span data-ttu-id="1272f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="1272f-194">Boolean</span></span>|<span data-ttu-id="1272f-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="1272f-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1272f-196">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1272f-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1272f-197">roleScopeTagIds</span></span>|<span data-ttu-id="1272f-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="1272f-198">String collection</span></span>|<span data-ttu-id="1272f-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="1272f-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1272f-200">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1272f-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="1272f-201">dependentAppCount</span></span>|<span data-ttu-id="1272f-202">Int32</span><span class="sxs-lookup"><span data-stu-id="1272f-202">Int32</span></span>|<span data-ttu-id="1272f-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="1272f-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="1272f-204">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1272f-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1272f-205">committedContentVersion</span></span>|<span data-ttu-id="1272f-206">字符串</span><span class="sxs-lookup"><span data-stu-id="1272f-206">String</span></span>|<span data-ttu-id="1272f-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="1272f-207">The internal committed content version.</span></span> <span data-ttu-id="1272f-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1272f-209">fileName</span><span class="sxs-lookup"><span data-stu-id="1272f-209">fileName</span></span>|<span data-ttu-id="1272f-210">字符串</span><span class="sxs-lookup"><span data-stu-id="1272f-210">String</span></span>|<span data-ttu-id="1272f-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="1272f-211">The name of the main Lob application file.</span></span> <span data-ttu-id="1272f-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1272f-213">size</span><span class="sxs-lookup"><span data-stu-id="1272f-213">size</span></span>|<span data-ttu-id="1272f-214">Int64</span><span class="sxs-lookup"><span data-stu-id="1272f-214">Int64</span></span>|<span data-ttu-id="1272f-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="1272f-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="1272f-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1272f-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1272f-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="1272f-217">bundleId</span></span>|<span data-ttu-id="1272f-218">String</span><span class="sxs-lookup"><span data-stu-id="1272f-218">String</span></span>|<span data-ttu-id="1272f-219">标识名称。</span><span class="sxs-lookup"><span data-stu-id="1272f-219">The Identity Name.</span></span>|
|<span data-ttu-id="1272f-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="1272f-220">applicableDeviceType</span></span>|[<span data-ttu-id="1272f-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="1272f-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="1272f-222">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="1272f-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="1272f-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1272f-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1272f-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1272f-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="1272f-225">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="1272f-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="1272f-226">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1272f-226">expirationDateTime</span></span>|<span data-ttu-id="1272f-227">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1272f-227">DateTimeOffset</span></span>|<span data-ttu-id="1272f-228">过期时间。</span><span class="sxs-lookup"><span data-stu-id="1272f-228">The expiration time.</span></span>|
|<span data-ttu-id="1272f-229">versionNumber</span><span class="sxs-lookup"><span data-stu-id="1272f-229">versionNumber</span></span>|<span data-ttu-id="1272f-230">字符串</span><span class="sxs-lookup"><span data-stu-id="1272f-230">String</span></span>|<span data-ttu-id="1272f-231">iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="1272f-231">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="1272f-232">buildNumber</span><span class="sxs-lookup"><span data-stu-id="1272f-232">buildNumber</span></span>|<span data-ttu-id="1272f-233">字符串</span><span class="sxs-lookup"><span data-stu-id="1272f-233">String</span></span>|<span data-ttu-id="1272f-234">iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="1272f-234">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="1272f-235">identityVersion</span><span class="sxs-lookup"><span data-stu-id="1272f-235">identityVersion</span></span>|<span data-ttu-id="1272f-236">String</span><span class="sxs-lookup"><span data-stu-id="1272f-236">String</span></span>|<span data-ttu-id="1272f-237">标识版本。</span><span class="sxs-lookup"><span data-stu-id="1272f-237">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="1272f-238">响应</span><span class="sxs-lookup"><span data-stu-id="1272f-238">Response</span></span>
<span data-ttu-id="1272f-239">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1272f-239">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1272f-240">示例</span><span class="sxs-lookup"><span data-stu-id="1272f-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="1272f-241">请求</span><span class="sxs-lookup"><span data-stu-id="1272f-241">Request</span></span>
<span data-ttu-id="1272f-242">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1272f-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1411

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
    "v12_0": true,
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="1272f-243">响应</span><span class="sxs-lookup"><span data-stu-id="1272f-243">Response</span></span>
<span data-ttu-id="1272f-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1272f-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1583

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
    "v12_0": true,
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```






