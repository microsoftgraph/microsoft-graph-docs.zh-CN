---
title: 更新 androidLobApp
description: 更新 androidLobApp 对象的属性。
ms.openlocfilehash: cecfe7c1bcd5437d89b71e1b1d81e47acabc250b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043270"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="b3d87-103">更新 androidLobApp</span><span class="sxs-lookup"><span data-stu-id="b3d87-103">Update androidLobApp</span></span>

> <span data-ttu-id="b3d87-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b3d87-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3d87-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b3d87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3d87-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b3d87-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3d87-107">更新 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b3d87-107">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3d87-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b3d87-108">Prerequisites</span></span>
<span data-ttu-id="b3d87-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b3d87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3d87-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3d87-111">Permission type</span></span>|<span data-ttu-id="b3d87-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b3d87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3d87-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3d87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3d87-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3d87-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b3d87-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3d87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3d87-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3d87-116">Not supported.</span></span>|
|<span data-ttu-id="b3d87-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3d87-117">Application</span></span>|<span data-ttu-id="b3d87-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3d87-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3d87-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3d87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="b3d87-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3d87-120">Request headers</span></span>
|<span data-ttu-id="b3d87-121">标头</span><span class="sxs-lookup"><span data-stu-id="b3d87-121">Header</span></span>|<span data-ttu-id="b3d87-122">值</span><span class="sxs-lookup"><span data-stu-id="b3d87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3d87-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3d87-123">Authorization</span></span>|<span data-ttu-id="b3d87-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b3d87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3d87-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b3d87-125">Accept</span></span>|<span data-ttu-id="b3d87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3d87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3d87-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3d87-127">Request body</span></span>
<span data-ttu-id="b3d87-128">在请求正文中，提供 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3d87-128">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="b3d87-129">下表显示了创建 [androidLobApp](../resources/intune-apps-androidlobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b3d87-129">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="b3d87-130">属性</span><span class="sxs-lookup"><span data-stu-id="b3d87-130">Property</span></span>|<span data-ttu-id="b3d87-131">类型</span><span class="sxs-lookup"><span data-stu-id="b3d87-131">Type</span></span>|<span data-ttu-id="b3d87-132">说明</span><span class="sxs-lookup"><span data-stu-id="b3d87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3d87-133">id</span><span class="sxs-lookup"><span data-stu-id="b3d87-133">id</span></span>|<span data-ttu-id="b3d87-134">String</span><span class="sxs-lookup"><span data-stu-id="b3d87-134">String</span></span>|<span data-ttu-id="b3d87-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b3d87-135">Key of the entity.</span></span> <span data-ttu-id="b3d87-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3d87-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3d87-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b3d87-137">displayName</span></span>|<span data-ttu-id="b3d87-138">String</span><span class="sxs-lookup"><span data-stu-id="b3d87-138">String</span></span>|<span data-ttu-id="b3d87-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="b3d87-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b3d87-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3d87-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3d87-141">description</span><span class="sxs-lookup"><span data-stu-id="b3d87-141">description</span></span>|<span data-ttu-id="b3d87-142">String</span><span class="sxs-lookup"><span data-stu-id="b3d87-142">String</span></span>|<span data-ttu-id="b3d87-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="b3d87-143">The description of the app.</span></span> <span data-ttu-id="b3d87-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3d87-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3d87-145">publisher</span><span class="sxs-lookup"><span data-stu-id="b3d87-145">publisher</span></span>|<span data-ttu-id="b3d87-146">String</span><span class="sxs-lookup"><span data-stu-id="b3d87-146">String</span></span>|<span data-ttu-id="b3d87-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="b3d87-147">The publisher of the app.</span></span> <span data-ttu-id="b3d87-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3d87-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3d87-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b3d87-149">largeIcon</span></span>|[<span data-ttu-id="b3d87-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b3d87-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b3d87-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="b3d87-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b3d87-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3d87-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3d87-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3d87-153">createdDateTime</span></span>|<span data-ttu-id="b3d87-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3d87-154">DateTimeOffset</span></span>|<span data-ttu-id="b3d87-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b3d87-155">The date and time the app was created.</span></span> <span data-ttu-id="b3d87-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3d87-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3d87-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3d87-157">lastModifiedDateTime</span></span>|<span data-ttu-id="b3d87-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3d87-158">DateTimeOffset</span></span>|<span data-ttu-id="b3d87-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b3d87-159">The date and time the app was last modified.</span></span> <span data-ttu-id="b3d87-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3d87-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3d87-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b3d87-161">isFeatured</span></span>|<span data-ttu-id="b3d87-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3d87-162">Boolean</span></span>|<span data-ttu-id="b3d87-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3d87-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3d87-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b3d87-164">privacyInformationUrl</span></span>|<span data-ttu-id="b3d87-165">String</span><span class="sxs-lookup"><span data-stu-id="b3d87-165">String</span></span>|<span data-ttu-id="b3d87-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="b3d87-166">The privacy statement Url.</span></span> <span data-ttu-id="b3d87-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3d87-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3d87-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b3d87-168">informationUrl</span></span>|<span data-ttu-id="b3d87-169">String</span><span class="sxs-lookup"><span data-stu-id="b3d87-169">String</span></span>|<span data-ttu-id="b3d87-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="b3d87-170">The more information Url.</span></span> <span data-ttu-id="b3d87-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3d87-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3d87-172">owner</span><span class="sxs-lookup"><span data-stu-id="b3d87-172">owner</span></span>|<span data-ttu-id="b3d87-173">String</span><span class="sxs-lookup"><span data-stu-id="b3d87-173">String</span></span>|<span data-ttu-id="b3d87-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="b3d87-174">The owner of the app.</span></span> <span data-ttu-id="b3d87-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3d87-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3d87-176">developer</span><span class="sxs-lookup"><span data-stu-id="b3d87-176">developer</span></span>|<span data-ttu-id="b3d87-177">String</span><span class="sxs-lookup"><span data-stu-id="b3d87-177">String</span></span>|<span data-ttu-id="b3d87-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="b3d87-178">The developer of the app.</span></span> <span data-ttu-id="b3d87-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3d87-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3d87-180">notes</span><span class="sxs-lookup"><span data-stu-id="b3d87-180">notes</span></span>|<span data-ttu-id="b3d87-181">String</span><span class="sxs-lookup"><span data-stu-id="b3d87-181">String</span></span>|<span data-ttu-id="b3d87-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="b3d87-182">Notes for the app.</span></span> <span data-ttu-id="b3d87-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3d87-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3d87-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="b3d87-184">uploadState</span></span>|<span data-ttu-id="b3d87-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b3d87-185">Int32</span></span>|<span data-ttu-id="b3d87-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="b3d87-186">The upload state.</span></span> <span data-ttu-id="b3d87-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3d87-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3d87-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="b3d87-188">publishingState</span></span>|[<span data-ttu-id="b3d87-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b3d87-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b3d87-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="b3d87-190">The publishing state for the app.</span></span> <span data-ttu-id="b3d87-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="b3d87-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b3d87-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="b3d87-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b3d87-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="b3d87-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b3d87-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b3d87-194">committedContentVersion</span></span>|<span data-ttu-id="b3d87-195">String</span><span class="sxs-lookup"><span data-stu-id="b3d87-195">String</span></span>|<span data-ttu-id="b3d87-196">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="b3d87-196">The internal committed content version.</span></span> <span data-ttu-id="b3d87-197">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3d87-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b3d87-198">fileName</span><span class="sxs-lookup"><span data-stu-id="b3d87-198">fileName</span></span>|<span data-ttu-id="b3d87-199">String</span><span class="sxs-lookup"><span data-stu-id="b3d87-199">String</span></span>|<span data-ttu-id="b3d87-200">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="b3d87-200">The name of the main Lob application file.</span></span> <span data-ttu-id="b3d87-201">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3d87-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b3d87-202">size</span><span class="sxs-lookup"><span data-stu-id="b3d87-202">size</span></span>|<span data-ttu-id="b3d87-203">Int64</span><span class="sxs-lookup"><span data-stu-id="b3d87-203">Int64</span></span>|<span data-ttu-id="b3d87-204">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="b3d87-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="b3d87-205">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3d87-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b3d87-206">packageId</span><span class="sxs-lookup"><span data-stu-id="b3d87-206">packageId</span></span>|<span data-ttu-id="b3d87-207">String</span><span class="sxs-lookup"><span data-stu-id="b3d87-207">String</span></span>|<span data-ttu-id="b3d87-208">包标识符。</span><span class="sxs-lookup"><span data-stu-id="b3d87-208">The package identifier.</span></span>|
|<span data-ttu-id="b3d87-209">identityName</span><span class="sxs-lookup"><span data-stu-id="b3d87-209">identityName</span></span>|<span data-ttu-id="b3d87-210">String</span><span class="sxs-lookup"><span data-stu-id="b3d87-210">String</span></span>|<span data-ttu-id="b3d87-211">标识名称。</span><span class="sxs-lookup"><span data-stu-id="b3d87-211">The Identity Name.</span></span>|
|<span data-ttu-id="b3d87-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b3d87-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b3d87-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b3d87-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="b3d87-214">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="b3d87-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="b3d87-215">versionName</span><span class="sxs-lookup"><span data-stu-id="b3d87-215">versionName</span></span>|<span data-ttu-id="b3d87-216">String</span><span class="sxs-lookup"><span data-stu-id="b3d87-216">String</span></span>|<span data-ttu-id="b3d87-217">Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="b3d87-217">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b3d87-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="b3d87-218">versionCode</span></span>|<span data-ttu-id="b3d87-219">String</span><span class="sxs-lookup"><span data-stu-id="b3d87-219">String</span></span>|<span data-ttu-id="b3d87-220">Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="b3d87-220">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b3d87-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="b3d87-221">identityVersion</span></span>|<span data-ttu-id="b3d87-222">String</span><span class="sxs-lookup"><span data-stu-id="b3d87-222">String</span></span>|<span data-ttu-id="b3d87-223">标识版本。</span><span class="sxs-lookup"><span data-stu-id="b3d87-223">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="b3d87-224">响应</span><span class="sxs-lookup"><span data-stu-id="b3d87-224">Response</span></span>
<span data-ttu-id="b3d87-225">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidLobApp](../resources/intune-apps-androidlobapp.md)  对象。</span><span class="sxs-lookup"><span data-stu-id="b3d87-225">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3d87-226">示例</span><span class="sxs-lookup"><span data-stu-id="b3d87-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3d87-227">请求</span><span class="sxs-lookup"><span data-stu-id="b3d87-227">Request</span></span>
<span data-ttu-id="b3d87-228">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b3d87-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1313

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
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
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="b3d87-229">响应</span><span class="sxs-lookup"><span data-stu-id="b3d87-229">Response</span></span>
<span data-ttu-id="b3d87-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b3d87-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1473

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```





