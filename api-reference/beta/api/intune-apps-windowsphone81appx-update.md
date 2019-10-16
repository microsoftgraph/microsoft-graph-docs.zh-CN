---
title: 更新了 windowsphone81appx
description: 更新了 windowsphone81appx 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b0a82f975500b1c41642513b9ab1be8ff088098b
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535028"
---
# <a name="update-windowsphone81appx"></a><span data-ttu-id="16889-103">更新了 windowsphone81appx</span><span class="sxs-lookup"><span data-stu-id="16889-103">Update windowsPhone81AppX</span></span>

> <span data-ttu-id="16889-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="16889-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16889-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="16889-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16889-106">更新[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="16889-106">Update the properties of a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16889-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="16889-107">Prerequisites</span></span>
<span data-ttu-id="16889-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16889-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16889-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="16889-110">Permission type</span></span>|<span data-ttu-id="16889-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="16889-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16889-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16889-112">Delegated (work or school account)</span></span>|<span data-ttu-id="16889-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16889-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="16889-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16889-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16889-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="16889-115">Not supported.</span></span>|
|<span data-ttu-id="16889-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="16889-116">Application</span></span>|<span data-ttu-id="16889-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16889-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16889-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16889-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="16889-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="16889-119">Request headers</span></span>
|<span data-ttu-id="16889-120">标头</span><span class="sxs-lookup"><span data-stu-id="16889-120">Header</span></span>|<span data-ttu-id="16889-121">值</span><span class="sxs-lookup"><span data-stu-id="16889-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16889-122">授权</span><span class="sxs-lookup"><span data-stu-id="16889-122">Authorization</span></span>|<span data-ttu-id="16889-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="16889-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16889-124">接受</span><span class="sxs-lookup"><span data-stu-id="16889-124">Accept</span></span>|<span data-ttu-id="16889-125">application/json</span><span class="sxs-lookup"><span data-stu-id="16889-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16889-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="16889-126">Request body</span></span>
<span data-ttu-id="16889-127">在请求正文中，提供[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16889-127">In the request body, supply a JSON representation for the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

<span data-ttu-id="16889-128">下表显示创建[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="16889-128">The following table shows the properties that are required when you create the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span>

|<span data-ttu-id="16889-129">属性</span><span class="sxs-lookup"><span data-stu-id="16889-129">Property</span></span>|<span data-ttu-id="16889-130">类型</span><span class="sxs-lookup"><span data-stu-id="16889-130">Type</span></span>|<span data-ttu-id="16889-131">说明</span><span class="sxs-lookup"><span data-stu-id="16889-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16889-132">id</span><span class="sxs-lookup"><span data-stu-id="16889-132">id</span></span>|<span data-ttu-id="16889-133">字符串</span><span class="sxs-lookup"><span data-stu-id="16889-133">String</span></span>|<span data-ttu-id="16889-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="16889-134">Key of the entity.</span></span> <span data-ttu-id="16889-135">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="16889-136">displayName</span><span class="sxs-lookup"><span data-stu-id="16889-136">displayName</span></span>|<span data-ttu-id="16889-137">字符串</span><span class="sxs-lookup"><span data-stu-id="16889-137">String</span></span>|<span data-ttu-id="16889-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="16889-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="16889-139">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="16889-140">说明</span><span class="sxs-lookup"><span data-stu-id="16889-140">description</span></span>|<span data-ttu-id="16889-141">字符串</span><span class="sxs-lookup"><span data-stu-id="16889-141">String</span></span>|<span data-ttu-id="16889-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="16889-142">The description of the app.</span></span> <span data-ttu-id="16889-143">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="16889-144">publisher</span><span class="sxs-lookup"><span data-stu-id="16889-144">publisher</span></span>|<span data-ttu-id="16889-145">字符串</span><span class="sxs-lookup"><span data-stu-id="16889-145">String</span></span>|<span data-ttu-id="16889-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="16889-146">The publisher of the app.</span></span> <span data-ttu-id="16889-147">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="16889-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="16889-148">largeIcon</span></span>|[<span data-ttu-id="16889-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="16889-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="16889-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="16889-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="16889-151">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="16889-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16889-152">createdDateTime</span></span>|<span data-ttu-id="16889-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16889-153">DateTimeOffset</span></span>|<span data-ttu-id="16889-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="16889-154">The date and time the app was created.</span></span> <span data-ttu-id="16889-155">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="16889-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16889-156">lastModifiedDateTime</span></span>|<span data-ttu-id="16889-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16889-157">DateTimeOffset</span></span>|<span data-ttu-id="16889-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="16889-158">The date and time the app was last modified.</span></span> <span data-ttu-id="16889-159">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="16889-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="16889-160">isFeatured</span></span>|<span data-ttu-id="16889-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="16889-161">Boolean</span></span>|<span data-ttu-id="16889-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="16889-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="16889-163">privacyInformationUrl</span></span>|<span data-ttu-id="16889-164">字符串</span><span class="sxs-lookup"><span data-stu-id="16889-164">String</span></span>|<span data-ttu-id="16889-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="16889-165">The privacy statement Url.</span></span> <span data-ttu-id="16889-166">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="16889-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="16889-167">informationUrl</span></span>|<span data-ttu-id="16889-168">字符串</span><span class="sxs-lookup"><span data-stu-id="16889-168">String</span></span>|<span data-ttu-id="16889-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="16889-169">The more information Url.</span></span> <span data-ttu-id="16889-170">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="16889-171">owner</span><span class="sxs-lookup"><span data-stu-id="16889-171">owner</span></span>|<span data-ttu-id="16889-172">String</span><span class="sxs-lookup"><span data-stu-id="16889-172">String</span></span>|<span data-ttu-id="16889-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="16889-173">The owner of the app.</span></span> <span data-ttu-id="16889-174">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="16889-175">developer</span><span class="sxs-lookup"><span data-stu-id="16889-175">developer</span></span>|<span data-ttu-id="16889-176">字符串</span><span class="sxs-lookup"><span data-stu-id="16889-176">String</span></span>|<span data-ttu-id="16889-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="16889-177">The developer of the app.</span></span> <span data-ttu-id="16889-178">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="16889-179">notes</span><span class="sxs-lookup"><span data-stu-id="16889-179">notes</span></span>|<span data-ttu-id="16889-180">字符串</span><span class="sxs-lookup"><span data-stu-id="16889-180">String</span></span>|<span data-ttu-id="16889-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="16889-181">Notes for the app.</span></span> <span data-ttu-id="16889-182">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="16889-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="16889-183">uploadState</span></span>|<span data-ttu-id="16889-184">Int32</span><span class="sxs-lookup"><span data-stu-id="16889-184">Int32</span></span>|<span data-ttu-id="16889-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="16889-185">The upload state.</span></span> <span data-ttu-id="16889-186">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="16889-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="16889-187">publishingState</span></span>|[<span data-ttu-id="16889-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="16889-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="16889-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="16889-189">The publishing state for the app.</span></span> <span data-ttu-id="16889-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="16889-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="16889-191">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="16889-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="16889-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="16889-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="16889-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="16889-193">isAssigned</span></span>|<span data-ttu-id="16889-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="16889-194">Boolean</span></span>|<span data-ttu-id="16889-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="16889-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="16889-196">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="16889-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="16889-197">roleScopeTagIds</span></span>|<span data-ttu-id="16889-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="16889-198">String collection</span></span>|<span data-ttu-id="16889-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="16889-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="16889-200">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="16889-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="16889-201">dependentAppCount</span></span>|<span data-ttu-id="16889-202">Int32</span><span class="sxs-lookup"><span data-stu-id="16889-202">Int32</span></span>|<span data-ttu-id="16889-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="16889-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="16889-204">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="16889-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="16889-205">committedContentVersion</span></span>|<span data-ttu-id="16889-206">字符串</span><span class="sxs-lookup"><span data-stu-id="16889-206">String</span></span>|<span data-ttu-id="16889-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="16889-207">The internal committed content version.</span></span> <span data-ttu-id="16889-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="16889-209">fileName</span><span class="sxs-lookup"><span data-stu-id="16889-209">fileName</span></span>|<span data-ttu-id="16889-210">字符串</span><span class="sxs-lookup"><span data-stu-id="16889-210">String</span></span>|<span data-ttu-id="16889-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="16889-211">The name of the main Lob application file.</span></span> <span data-ttu-id="16889-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="16889-213">size</span><span class="sxs-lookup"><span data-stu-id="16889-213">size</span></span>|<span data-ttu-id="16889-214">Int64</span><span class="sxs-lookup"><span data-stu-id="16889-214">Int64</span></span>|<span data-ttu-id="16889-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="16889-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="16889-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="16889-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="16889-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="16889-217">applicableArchitectures</span></span>|[<span data-ttu-id="16889-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="16889-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="16889-219">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="16889-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="16889-220">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="16889-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="16889-221">identityName</span><span class="sxs-lookup"><span data-stu-id="16889-221">identityName</span></span>|<span data-ttu-id="16889-222">字符串</span><span class="sxs-lookup"><span data-stu-id="16889-222">String</span></span>|<span data-ttu-id="16889-223">标识名称。</span><span class="sxs-lookup"><span data-stu-id="16889-223">The Identity Name.</span></span>|
|<span data-ttu-id="16889-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="16889-224">identityPublisherHash</span></span>|<span data-ttu-id="16889-225">String</span><span class="sxs-lookup"><span data-stu-id="16889-225">String</span></span>|<span data-ttu-id="16889-226">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="16889-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="16889-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="16889-227">identityResourceIdentifier</span></span>|<span data-ttu-id="16889-228">字符串</span><span class="sxs-lookup"><span data-stu-id="16889-228">String</span></span>|<span data-ttu-id="16889-229">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="16889-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="16889-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="16889-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="16889-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="16889-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="16889-232">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="16889-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="16889-233">将 phoneproductidentifier</span><span class="sxs-lookup"><span data-stu-id="16889-233">phoneProductIdentifier</span></span>|<span data-ttu-id="16889-234">字符串</span><span class="sxs-lookup"><span data-stu-id="16889-234">String</span></span>|<span data-ttu-id="16889-235">电话产品标识符。</span><span class="sxs-lookup"><span data-stu-id="16889-235">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="16889-236">将 phonepublisherid</span><span class="sxs-lookup"><span data-stu-id="16889-236">phonePublisherId</span></span>|<span data-ttu-id="16889-237">字符串</span><span class="sxs-lookup"><span data-stu-id="16889-237">String</span></span>|<span data-ttu-id="16889-238">电话发布者 Id。</span><span class="sxs-lookup"><span data-stu-id="16889-238">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="16889-239">identityVersion</span><span class="sxs-lookup"><span data-stu-id="16889-239">identityVersion</span></span>|<span data-ttu-id="16889-240">String</span><span class="sxs-lookup"><span data-stu-id="16889-240">String</span></span>|<span data-ttu-id="16889-241">标识版本。</span><span class="sxs-lookup"><span data-stu-id="16889-241">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="16889-242">响应</span><span class="sxs-lookup"><span data-stu-id="16889-242">Response</span></span>
<span data-ttu-id="16889-243">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)对象。</span><span class="sxs-lookup"><span data-stu-id="16889-243">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16889-244">示例</span><span class="sxs-lookup"><span data-stu-id="16889-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="16889-245">请求</span><span class="sxs-lookup"><span data-stu-id="16889-245">Request</span></span>
<span data-ttu-id="16889-246">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="16889-246">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1513

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
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
    "v10_1903": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="16889-247">响应</span><span class="sxs-lookup"><span data-stu-id="16889-247">Response</span></span>
<span data-ttu-id="16889-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="16889-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1685

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
    "v10_1903": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```






