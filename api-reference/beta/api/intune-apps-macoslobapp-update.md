---
title: 更新 macOSLobApp
description: 更新 macOSLobApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4337230a11568d8c1a021ae88726a8833fda38a6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148830"
---
# <a name="update-macoslobapp"></a><span data-ttu-id="f045b-103">更新 macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="f045b-103">Update macOSLobApp</span></span>

> <span data-ttu-id="f045b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f045b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f045b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f045b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f045b-106">更新[macOSLobApp](../resources/intune-apps-macoslobapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f045b-106">Update the properties of a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f045b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f045b-107">Prerequisites</span></span>
<span data-ttu-id="f045b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f045b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f045b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f045b-110">Permission type</span></span>|<span data-ttu-id="f045b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f045b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f045b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f045b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f045b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f045b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f045b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f045b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f045b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f045b-115">Not supported.</span></span>|
|<span data-ttu-id="f045b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f045b-116">Application</span></span>|<span data-ttu-id="f045b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f045b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f045b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f045b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f045b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f045b-119">Request headers</span></span>
|<span data-ttu-id="f045b-120">标头</span><span class="sxs-lookup"><span data-stu-id="f045b-120">Header</span></span>|<span data-ttu-id="f045b-121">值</span><span class="sxs-lookup"><span data-stu-id="f045b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f045b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f045b-122">Authorization</span></span>|<span data-ttu-id="f045b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f045b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f045b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f045b-124">Accept</span></span>|<span data-ttu-id="f045b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f045b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f045b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f045b-126">Request body</span></span>
<span data-ttu-id="f045b-127">在请求正文中, 提供[macOSLobApp](../resources/intune-apps-macoslobapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f045b-127">In the request body, supply a JSON representation for the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

<span data-ttu-id="f045b-128">下表显示创建[macOSLobApp](../resources/intune-apps-macoslobapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f045b-128">The following table shows the properties that are required when you create the [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span></span>

|<span data-ttu-id="f045b-129">属性</span><span class="sxs-lookup"><span data-stu-id="f045b-129">Property</span></span>|<span data-ttu-id="f045b-130">类型</span><span class="sxs-lookup"><span data-stu-id="f045b-130">Type</span></span>|<span data-ttu-id="f045b-131">说明</span><span class="sxs-lookup"><span data-stu-id="f045b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f045b-132">id</span><span class="sxs-lookup"><span data-stu-id="f045b-132">id</span></span>|<span data-ttu-id="f045b-133">字串符号</span><span class="sxs-lookup"><span data-stu-id="f045b-133">String</span></span>|<span data-ttu-id="f045b-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f045b-134">Key of the entity.</span></span> <span data-ttu-id="f045b-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f045b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f045b-136">displayName</span></span>|<span data-ttu-id="f045b-137">字符串</span><span class="sxs-lookup"><span data-stu-id="f045b-137">String</span></span>|<span data-ttu-id="f045b-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="f045b-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f045b-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f045b-140">description</span><span class="sxs-lookup"><span data-stu-id="f045b-140">description</span></span>|<span data-ttu-id="f045b-141">字符串</span><span class="sxs-lookup"><span data-stu-id="f045b-141">String</span></span>|<span data-ttu-id="f045b-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="f045b-142">The description of the app.</span></span> <span data-ttu-id="f045b-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f045b-144">publisher</span><span class="sxs-lookup"><span data-stu-id="f045b-144">publisher</span></span>|<span data-ttu-id="f045b-145">字符串</span><span class="sxs-lookup"><span data-stu-id="f045b-145">String</span></span>|<span data-ttu-id="f045b-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="f045b-146">The publisher of the app.</span></span> <span data-ttu-id="f045b-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f045b-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f045b-148">largeIcon</span></span>|[<span data-ttu-id="f045b-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f045b-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f045b-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="f045b-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f045b-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f045b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f045b-152">createdDateTime</span></span>|<span data-ttu-id="f045b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f045b-153">DateTimeOffset</span></span>|<span data-ttu-id="f045b-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f045b-154">The date and time the app was created.</span></span> <span data-ttu-id="f045b-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f045b-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f045b-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f045b-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f045b-157">DateTimeOffset</span></span>|<span data-ttu-id="f045b-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f045b-158">The date and time the app was last modified.</span></span> <span data-ttu-id="f045b-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f045b-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f045b-160">isFeatured</span></span>|<span data-ttu-id="f045b-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f045b-161">Boolean</span></span>|<span data-ttu-id="f045b-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f045b-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f045b-163">privacyInformationUrl</span></span>|<span data-ttu-id="f045b-164">字符串</span><span class="sxs-lookup"><span data-stu-id="f045b-164">String</span></span>|<span data-ttu-id="f045b-165">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="f045b-165">The privacy statement Url.</span></span> <span data-ttu-id="f045b-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f045b-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f045b-167">informationUrl</span></span>|<span data-ttu-id="f045b-168">字符串</span><span class="sxs-lookup"><span data-stu-id="f045b-168">String</span></span>|<span data-ttu-id="f045b-169">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="f045b-169">The more information Url.</span></span> <span data-ttu-id="f045b-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f045b-171">owner</span><span class="sxs-lookup"><span data-stu-id="f045b-171">owner</span></span>|<span data-ttu-id="f045b-172">字符串</span><span class="sxs-lookup"><span data-stu-id="f045b-172">String</span></span>|<span data-ttu-id="f045b-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="f045b-173">The owner of the app.</span></span> <span data-ttu-id="f045b-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f045b-175">developer</span><span class="sxs-lookup"><span data-stu-id="f045b-175">developer</span></span>|<span data-ttu-id="f045b-176">字符串</span><span class="sxs-lookup"><span data-stu-id="f045b-176">String</span></span>|<span data-ttu-id="f045b-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="f045b-177">The developer of the app.</span></span> <span data-ttu-id="f045b-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f045b-179">notes</span><span class="sxs-lookup"><span data-stu-id="f045b-179">notes</span></span>|<span data-ttu-id="f045b-180">字符串</span><span class="sxs-lookup"><span data-stu-id="f045b-180">String</span></span>|<span data-ttu-id="f045b-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="f045b-181">Notes for the app.</span></span> <span data-ttu-id="f045b-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f045b-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="f045b-183">uploadState</span></span>|<span data-ttu-id="f045b-184">Int32</span><span class="sxs-lookup"><span data-stu-id="f045b-184">Int32</span></span>|<span data-ttu-id="f045b-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="f045b-185">The upload state.</span></span> <span data-ttu-id="f045b-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f045b-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="f045b-187">publishingState</span></span>|[<span data-ttu-id="f045b-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f045b-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f045b-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="f045b-189">The publishing state for the app.</span></span> <span data-ttu-id="f045b-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="f045b-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f045b-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="f045b-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f045b-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="f045b-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f045b-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f045b-193">isAssigned</span></span>|<span data-ttu-id="f045b-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f045b-194">Boolean</span></span>|<span data-ttu-id="f045b-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="f045b-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f045b-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f045b-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f045b-197">roleScopeTagIds</span></span>|<span data-ttu-id="f045b-198">String collection</span><span class="sxs-lookup"><span data-stu-id="f045b-198">String collection</span></span>|<span data-ttu-id="f045b-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="f045b-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f045b-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f045b-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f045b-201">committedContentVersion</span></span>|<span data-ttu-id="f045b-202">String</span><span class="sxs-lookup"><span data-stu-id="f045b-202">String</span></span>|<span data-ttu-id="f045b-203">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="f045b-203">The internal committed content version.</span></span> <span data-ttu-id="f045b-204">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f045b-205">fileName</span><span class="sxs-lookup"><span data-stu-id="f045b-205">fileName</span></span>|<span data-ttu-id="f045b-206">字符串</span><span class="sxs-lookup"><span data-stu-id="f045b-206">String</span></span>|<span data-ttu-id="f045b-207">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="f045b-207">The name of the main Lob application file.</span></span> <span data-ttu-id="f045b-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f045b-209">size</span><span class="sxs-lookup"><span data-stu-id="f045b-209">size</span></span>|<span data-ttu-id="f045b-210">Int64</span><span class="sxs-lookup"><span data-stu-id="f045b-210">Int64</span></span>|<span data-ttu-id="f045b-211">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="f045b-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="f045b-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f045b-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f045b-213">bundleId</span><span class="sxs-lookup"><span data-stu-id="f045b-213">bundleId</span></span>|<span data-ttu-id="f045b-214">字符串</span><span class="sxs-lookup"><span data-stu-id="f045b-214">String</span></span>|<span data-ttu-id="f045b-215">捆绑包 id。</span><span class="sxs-lookup"><span data-stu-id="f045b-215">The bundle id.</span></span>|
|<span data-ttu-id="f045b-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f045b-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f045b-217">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f045b-217">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="f045b-218">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="f045b-218">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f045b-219">buildNumber</span><span class="sxs-lookup"><span data-stu-id="f045b-219">buildNumber</span></span>|<span data-ttu-id="f045b-220">字符串</span><span class="sxs-lookup"><span data-stu-id="f045b-220">String</span></span>|<span data-ttu-id="f045b-221">MacOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="f045b-221">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f045b-222">versionNumber</span><span class="sxs-lookup"><span data-stu-id="f045b-222">versionNumber</span></span>|<span data-ttu-id="f045b-223">字符串</span><span class="sxs-lookup"><span data-stu-id="f045b-223">String</span></span>|<span data-ttu-id="f045b-224">MacOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="f045b-224">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f045b-225">childApps</span><span class="sxs-lookup"><span data-stu-id="f045b-225">childApps</span></span>|<span data-ttu-id="f045b-226">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="f045b-226">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="f045b-227">此捆绑包包中的应用程序列表</span><span class="sxs-lookup"><span data-stu-id="f045b-227">The app list in this bundle package</span></span>|
|<span data-ttu-id="f045b-228">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f045b-228">identityVersion</span></span>|<span data-ttu-id="f045b-229">String</span><span class="sxs-lookup"><span data-stu-id="f045b-229">String</span></span>|<span data-ttu-id="f045b-230">标识版本。</span><span class="sxs-lookup"><span data-stu-id="f045b-230">The identity version.</span></span>|
|<span data-ttu-id="f045b-231">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="f045b-231">md5HashChunkSize</span></span>|<span data-ttu-id="f045b-232">Int32</span><span class="sxs-lookup"><span data-stu-id="f045b-232">Int32</span></span>|<span data-ttu-id="f045b-233">MD5 哈希的块大小</span><span class="sxs-lookup"><span data-stu-id="f045b-233">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="f045b-234">md5Hash</span><span class="sxs-lookup"><span data-stu-id="f045b-234">md5Hash</span></span>|<span data-ttu-id="f045b-235">String collection</span><span class="sxs-lookup"><span data-stu-id="f045b-235">String collection</span></span>|<span data-ttu-id="f045b-236">MD5 哈希代码</span><span class="sxs-lookup"><span data-stu-id="f045b-236">The MD5 hash codes</span></span>|
|<span data-ttu-id="f045b-237">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="f045b-237">ignoreVersionDetection</span></span>|<span data-ttu-id="f045b-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="f045b-238">Boolean</span></span>|<span data-ttu-id="f045b-239">控制应用的版本是否将用于检测安装在设备上的应用的布尔值。</span><span class="sxs-lookup"><span data-stu-id="f045b-239">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="f045b-240">对于使用自我更新功能的 macOS 业务线 (LoB) 应用, 请将此设置为 true。</span><span class="sxs-lookup"><span data-stu-id="f045b-240">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="f045b-241">响应</span><span class="sxs-lookup"><span data-stu-id="f045b-241">Response</span></span>
<span data-ttu-id="f045b-242">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[macOSLobApp](../resources/intune-apps-macoslobapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f045b-242">If successful, this method returns a `200 OK` response code and an updated [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f045b-243">示例</span><span class="sxs-lookup"><span data-stu-id="f045b-243">Example</span></span>

### <a name="request"></a><span data-ttu-id="f045b-244">请求</span><span class="sxs-lookup"><span data-stu-id="f045b-244">Request</span></span>
<span data-ttu-id="f045b-245">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f045b-245">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1547

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
    "v10_13": true
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

### <a name="response"></a><span data-ttu-id="f045b-246">响应</span><span class="sxs-lookup"><span data-stu-id="f045b-246">Response</span></span>
<span data-ttu-id="f045b-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f045b-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1719

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
    "v10_13": true
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




